# Mulesoft Monitoring - Install DynaTrace

  - # Requirements
    
      - ## Firewall
        
          - Outbound access from the Mulesoft RTF cluster IP space to
            54.198.108.77, 54.227.190.204, 50.17.238.238 IPs on port
            443/tcp
        
          - The FQDN is: gah29713.live.dynatrace.com
    
      - ## Access to internet on the host you are running the install or a local copy of the files needed from GIT
        
          - <https://github.com/Dynatrace/dynatrace-operator/releases/download/v0.10.0/kubernetes.yaml>
        
          - <https://github.com/Dynatrace/dynatrace-operator/releases/download/v0.10.0/kubernetes-csi.yaml>
        
          - <https://raw.githubusercontent.com/Dynatrace/dynatrace-operator/v0.10.0/assets/samples/cloudNativeFullStack.yaml>
            ( you will need to edit this file before the installation)
    
      - ## Access to the Mulesoft environment
        
          - kubectl installed, awsauth etc. you can follow [Setup access
            to Mulesoft kubernetes
            environments](https://ltimindtree-my.sharepoint.com/display/SEL/Setup+access+to+Mulesoft+kubernetes+environments)

<!-- end list -->

  - # Installation of DynaTrace cloudNativeFullStack
    
      - Checkout the documentation:
        <https://www.dynatrace.com/support/help/shortlink/full-stack-dto-k8#manual>
    
      - Create dynatrace namespace

> kubectl create namespace dynatrace

  - Install kubernetes DT operatior ( if your system doesn't have access
    to WWW, like the jumphost, then download the file and rsync it to
    the jumphost or the host you are operation on ).

> kubectl apply -f
> https://github.com/Dynatrace/dynatrace-operator/releases/download/v0.10.0/kubernetes.yaml

  - Expected output

  - poddisruptionbudget.policy/dynatrace-webhook created

  - serviceaccount/dynatrace-activegate created

  - serviceaccount/dynatrace-kubernetes-monitoring created

  - serviceaccount/dynatrace-dynakube-oneagent-privileged created

  - serviceaccount/dynatrace-dynakube-oneagent-unprivileged created

  - serviceaccount/dynatrace-operator created

  - serviceaccount/dynatrace-webhook created

  - customresourcedefinition.apiextensions.k8s.io/dynakubes.dynatrace.com
    created

  - clusterrole.rbac.authorization.k8s.io/dynatrace-kubernetes-monitoring
    created

  - clusterrole.rbac.authorization.k8s.io/dynatrace-operator created

  - clusterrole.rbac.authorization.k8s.io/dynatrace-webhook created

  - clusterrolebinding.rbac.authorization.k8s.io/dynatrace-kubernetes-monitoring
    created

  - clusterrolebinding.rbac.authorization.k8s.io/dynatrace-operator
    created

  - clusterrolebinding.rbac.authorization.k8s.io/dynatrace-webhook
    created

  - role.rbac.authorization.k8s.io/dynatrace-operator created

  - role.rbac.authorization.k8s.io/dynatrace-webhook created

  - rolebinding.rbac.authorization.k8s.io/dynatrace-operator created

  - rolebinding.rbac.authorization.k8s.io/dynatrace-webhook created

  - service/dynatrace-webhook created

  - deployment.apps/dynatrace-operator created

  - deployment.apps/dynatrace-webhook created

  - mutatingwebhookconfiguration.admissionregistration.k8s.io/dynatrace-webhook
    created

> validatingwebhookconfiguration.admissionregistration.k8s.io/dynatrace-webhook
> created

  - Install kubernetes DT operatior CSI agent ( if your system doesn't
    have access to WWW, like the jumphost, then download the file and
    rsync it to the jumphost or the host you are operation on).

> kubectl apply -f
> https://github.com/Dynatrace/dynatrace-operator/releases/download/v0.10.0/kubernetes-csi.yaml

  - Expected output

  - serviceaccount/dynatrace-oneagent-csi-driver created

  - clusterrole.rbac.authorization.k8s.io/dynatrace-oneagent-csi-driver
    created

  - clusterrolebinding.rbac.authorization.k8s.io/dynatrace-oneagent-csi-driver
    created

  - role.rbac.authorization.k8s.io/dynatrace-oneagent-csi-driver created

  - rolebinding.rbac.authorization.k8s.io/dynatrace-oneagent-csi-driver
    created

  - daemonset.apps/dynatrace-oneagent-csi-driver created

  - csidriver.storage.k8s.io/csi.oneagent.dynatrace.com created

> priorityclass.scheduling.k8s.io/dynatrace-high-priority created

  - Validate the installation so far

> kubectl -n dynatrace wait pod --for=condition=ready
> --selector=app.kubernetes.io/name=dynatrace-operator,app.kubernetes.io/component=webhook
> --timeout=300s

  - Expected output ( the trailing hash will be different ).

  - pod/dynatrace-webhook-5c67d77f4c-57rvq condition met

> pod/dynatrace-webhook-5c67d77f4c-tscqz condition met

  - Login to DynaTrace UI
    
      - Manage / DynaTrace Hub
    
      - TODO - missing the point where the tokens are generated

  - For **cloudNativeFullStack** and applicationMonitoring, create a
    secret named dynakube holding both the API token and the
    dataIngestToken, see Tokens and permissions required. Be sure to
    replace the placeholders (\<...\>) with your own values.

> kubectl -n dynatrace create secret generic dynakube
> --from-literal="apiToken=\<API\_TOKEN\>"
> --from-literal="dataIngestToken=\<DATA\_INGEST\_TOKEN\>"

  - Download the custom config of DynaKube

> wget
> https://raw.githubusercontent.com/Dynatrace/dynatrace-operator/v0.10.0/assets/samples/cloudNativeFullStack.yaml

  - Edit the downloaded file and adjust the first few lines to look like
    this, MAKE SURE you give it metadata/name as you wish to appear in
    Infrastructure/Kubernetes. This will be used as a filter for all
    workloads/pods etc. Also make sure the tokens: are set to "dynakube"

  - apiVersion: dynatrace.com/v1beta1

  - kind: DynaKube

  - metadata:

  - name: mule-stg-rtf

  - namespace: dynatrace

  - spec:

  - \# Dynatrace apiUrl including the \`/api\` path at the end.

  - \# For SaaS, set \`YOUR\_ENVIRONMENT\_ID\` to your environment ID.

  - \# For Managed, change the apiUrl address.

  - \# For instructions on how to determine the environment ID and how
    to configure the apiUrl address, see
    https://www.dynatrace.com/support/help/reference/dynatrace-concepts/environment-id/.

  - apiUrl: https://gah29713.live.dynatrace.com/api

  - 
  - \# Optional: Name of the secret holding the credentials required to
    connect to the Dynatrace tenant

  - \# If unset, the name of this custom resource is used

  - \#

  - tokens: "dynakube"

  - 
  - Install the DynaKube

> kubectl apply -f cloudNativeFullStack.yaml

  - Expected output

> dynakube.dynatrace.com/mule-stg-rtf created

  - Pull the cluster ID as you will need it to manually connect it in
    the Dynatrace UI

> kubectl get namespace kube-system -o jsonpath='{.metadata.uid}'

  - Login to Dynatrace UI

  - Checkout this documentation
    <https://www.dynatrace.com/support/help/shortlink/deploy-ag-dynatrace-op#local>
    , We'll use connect manually method

  - #### Provide the Kubernetes cluster ID in the Dynatrace web UI
    
      - > In the [Dynatrace
        > menu](https://www.dynatrace.com/support/help/get-started/navigation),
        > go to **Kubernetes**.
    
      - > Select **Connect manually**.
    
      - > On the Kubernetes cluster monitoring settings page, provide a
        > **Name**, and then turn on **Connect containerized ActiveGate
        > to local Kubernetes API endpoint**.
    
      - > For **Kubernetes cluster ID**, enter the UID obtained earlier.
    
      - > Select **Save changes** to save your configuration. **Note:**
        > You can save your configuration even if the ActiveGate isn't
        > ready to connect, and finish the configuration later. To
        > verify if it's ready, select **Test configuration**.

  - Give it few minutes, when you navigate to Infrastructure/Kubernetes
    you should see a new entry mule-rtf-stg.

  - Go to settings and enable "Events"
