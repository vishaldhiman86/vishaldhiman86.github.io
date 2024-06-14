# Mulesoft applications deploy

NOTE: I have screenshots of the steps and will add them here soon.

  - Login to Mulesoft Anypoint Portal:
    <https://anypoint.mulesoft.com/login/domain/allegiant>
    
      - Select "Continue with PingFederate SSO
    
      - Sign in with AD credentials
    
      - Sign in with RSA token

  - First time login: check that your profile reflects AllegiantIT in
    Active Business Group

  - 
  - Click on the top left menu and select "Runtime Manager"

  - Select environment clicking on the top left button which does
    identify the current selected environment.

  - Select desired environment from the list.

  - Once environment is switched it will identify the selected
    environment in the top left corner.

  - Use the search bar and search for the application name. At this
    point there is one application named "comms-exp-api".

  - Click on the link named after the application from the list below.

  - Click on "Choose file" drop down menu and select "Import file from
    Exchange"

  - In the new popup window use the search bar and search for
    "comms-exp-api-impl" (the actual artifact name).

  - Click on the artifact name and then select the desired version from
    the drop down menu below, then click on the "Select" button.

  - On the next screen locate a blue button "Apply changes", this will
    trigger the deploy of the artifact.

  - Then there will be a link on the top center of the page "View
    progress", you can click on it and watch the progress.

  - Once the deploy does complete (it takes few minutes for the app to
    deploy) you will see status "success" or "failed"

  - Failed deploy will require review of logs and or manually login to
    the cluster and check the PODs (need to add more details for
    troubleshooting).

# Mulesoft - disable DT log enrichment for any new app deployed

1\. Login to DT

2\. Go to
<https://gah29713.live.dynatrace.com/ui/entity/list/CONTAINER_GROUP?gtf=-2h&gf=all&sessionId=i1fmb7P2IpZ0jF3A>

3\. Filter by [K8s.container.name](http://K8s.container.name) = 'app'
and k8s.namespace = ENV\_NAMESPACE

4\. CLick on the desired application

5\. Scroll down to the "Process group" section

6\. Select the group Name

7\. Click on top right "Settings" button

8\. Go to "OneAgent features" from the menu

9\. Click on "Add override"

10\. Select "Java - Trace/span context enrichment for logs"

11\. Select "Java - Trace/span context enrichment for unstructured logs"

12\. The override will have the swithch turned "off" by default

13\. Klick "save shanges" on bottom left

14\. Login to Anypoint Runtime Manager

15\. Select the desired environment

16\. Select the application, clicking on the app name

17\. Click "Stop" button top right

18\. Wait for a message "Desired configuration applied successfully (At
this point the Application status should be 'NOT RUNNING')

19\. Start the app, click on "Enable" button top right (Wait for the
'Desired configuration applied successfully' message)
