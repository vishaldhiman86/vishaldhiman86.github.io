Date: Mon, 10 Jun 2024 02:21:29 -0700 (PDT)

Message-ID:
\<1337379652.41.1718011289795@vswcrpcnfap02.crp.allegiantair.com\>

Subject: Exported From Confluence

MIME-Version: 1.0

Content-Type: multipart/related;

boundary="----=\_Part\_40\_1516775522.1718011289795"

\------=\_Part\_40\_1516775522.1718011289795

Content-Type: text/html; charset=UTF-8

Content-Transfer-Encoding: quoted-printable

Content-Location: file:///C:/exported.html

\<html xmlns:o=3D'urn:schemas-microsoft-com:office:office'

xmlns:w=3D'urn:schemas-microsoft-com:office:word'

xmlns:v=3D'urn:schemas-microsoft-com:vml'

xmlns=3D'urn:w3-org-ns:HTML'\>

\<head\>

\<meta http-equiv=3D"Content-Type" content=3D"text/html;
charset=3Dutf-8=

"\>

\<title\>Mulesoft Monitoring - Install DynaTrace\</title\>

\<\!--\[if gte mso 9\]\>

\<xml\>

\<o:OfficeDocumentSettings\>

\<o:TargetScreenSize\>1024x640\</o:TargetScreenSize\>

\<o:PixelsPerInch\>72\</o:PixelsPerInch\>

\<o:AllowPNG/\>

\</o:OfficeDocumentSettings\>

\<w:WordDocument\>

\<w:View\>Print\</w:View\>

\<w:Zoom\>90\</w:Zoom\>

\<w:DoNotOptimizeForBrowser/\>

\</w:WordDocument\>

\</xml\>

\<\!\[endif\]--\>

\<style\>

\<\!--

@page Section1 {

size: 8.5in 11.0in;

margin: 1.0in;

mso-header-margin: .5in;

mso-footer-margin: .5in;

mso-paper-source: 0;

}

table {

border: solid 1px;

border-collapse: collapse;

}

table td, table th {

border: solid 1px;

padding: 5px;

}

td {

page-break-inside: avoid;

}

tr {

page-break-after: avoid;

}

div.Section1 {

page: Section1;

}

/\* Confluence print stylesheet. Common to all themes for print medi=

a \*/

/\* Full of \!important until we improve batching for print CSS \*/

@media print {

\#main {

padding-bottom: 1em \!important; /\* The default padding of 6em is to=

o much for printouts \*/

}

body {

font-family: Arial, Helvetica, FreeSans, sans-serif;

font-size: 10pt;

line-height: 1.2;

}

body, \#full-height-container, \#main, \#page, \#content,
.has-personal-sid=

ebar \#content {

background: \#fff \!important;

color: \#000 \!important;

border: 0 \!important;

width: 100% \!important;

height: auto \!important;

min-height: auto \!important;

margin: 0 \!important;

padding: 0 \!important;

display: block \!important;

}

a, a:link, a:visited, a:focus, a:hover, a:active {

color: \#000;

}

\#content h1,

\#content h2,

\#content h3,

\#content h4,

\#content h5,

\#content h6 {

font-family: Arial, Helvetica, FreeSans, sans-serif;

page-break-after: avoid;

}

pre {

font-family: Monaco, "Courier New", monospace;

}

\#header,

.aui-header-inner,

\#navigation,

\#sidebar,

.sidebar,

\#personal-info-sidebar,

.ia-fixed-sidebar,

.page-actions,

.navmenu,

.ajs-menu-bar,

.noprint,

.inline-control-link,

.inline-control-link a,

a.show-labels-editor,

.global-comment-actions,

.comment-actions,

.quick-comment-container,

\#addcomment {

display: none \!important;

}

/\* CONF-28544 cannot print multiple pages in IE \*/

\#splitter-content {

position: relative \!important;

}

.comment .date::before {

content: none \!important; /\* remove middot for print view \*/

}

h1.pagetitle img {

height: auto;

width: auto;

}

.print-only {

display: block;

}

\#footer {

position: relative \!important; /\* CONF-17506 Place the footer at en=

d of the content \*/

margin: 0;

padding: 0;

background: none;

clear: both;

}

\#poweredby {

border-top: none;

background: none;

}

\#poweredby li.print-only {

display: list-item;

font-style: italic;

}

\#poweredby li.noprint {

display: none;

}

/\* no width controls in print \*/

.wiki-content .table-wrap,

.wiki-content p,

.panel .codeContent,

.panel .codeContent pre,

.image-wrap {

overflow: visible \!important;

}

/\* TODO - should this work? \*/

\#children-section,

\#comments-section .comment,

\#comments-section .comment .comment-body,

\#comments-section .comment .comment-content,

\#comments-section .comment p {

page-break-inside: avoid;

}

\#page-children a {

text-decoration: none;

}

/\*\*

hide twixies

the specificity here is a hack because print styles

are getting loaded before the base styles. \*/

\#comments-section.pageSection .section-header,

\#comments-section.pageSection .section-title,

\#children-section.pageSection .section-header,

\#children-section.pageSection .section-title,

.children-show-hide {

padding-left: 0;

margin-left: 0;

}

.children-show-hide.icon {

display: none;

}

/\* personal sidebar \*/

.has-personal-sidebar \#content {

margin-right: 0px;

}

.has-personal-sidebar \#content .pageSection {

margin-right: 0px;

}

.no-print, .no-print \* {

display: none \!important;

}

}

\--\>

\</style\>

\</head\>

\<body\>

\<h1\>Mulesoft Monitoring - Install DynaTrace\</h1\>

\<div class=3D"Section1"\>

\<ul\>

\<li\>\<h1
id=3D"MulesoftMonitoringInstallDynaTrace-Requirements"\>Requirements=

\</h1\>

\<ul\>

\<li\>\<h2
id=3D"MulesoftMonitoringInstallDynaTrace-Firewall"\>Firewall\</h2\>

\<ul\>

\<li\>Outbound access from the Mulesoft RTF cluster IP space to
54.198.108.77=

, 54.227.190.204, 50.17.238.238 IPs on port 443/tcp\</li\>

\<li\>The FQDN is: gah29713.live.dynatrace.com\</li\>

\</ul\>\</li\>

\<li\>\<h2
id=3D"MulesoftMonitoringInstallDynaTrace-Accesstointernetonthehosty=

ouarerunningtheinstalloralocalcopyofthefilesneededfromGIT"\>Access to
intern=

et on the host you are running the install or a local copy of the files
nee=

ded from GIT\</h2\>

\<ul\>

\<li\>\<a class=3D"external-link"
href=3D"https://github.com/Dynatrace/dynatra=

ce-operator/releases/download/v0.10.0/kubernetes.yaml"
rel=3D"nofollow"\>htt=

ps://github.com/Dynatrace/dynatrace-operator/releases/download/v0.10.0/kube=

rnetes.yaml\</a\>\</li\>

\<li\>\<a class=3D"external-link"
href=3D"https://github.com/Dynatrace/dynatra=

ce-operator/releases/download/v0.10.0/kubernetes-csi.yaml"
rel=3D"nofollow"=

\>https://github.com/Dynatrace/dynatrace-operator/releases/download/v0.10.0/=

kubernetes-csi.yaml\</a\>\</li\>

\<li\>\<a class=3D"external-link"
href=3D"https://raw.githubusercontent.com/Dy=

natrace/dynatrace-operator/v0.10.0/assets/samples/cloudNativeFullStack.yaml=

"
rel=3D"nofollow"\>https://raw.githubusercontent.com/Dynatrace/dynatrace-op=

erator/v0.10.0/assets/samples/cloudNativeFullStack.yaml\</a\> ( you will
need=

to edit this file before the installation)\</li\>

\</ul\>\</li\>

\<li\>\<h2
id=3D"MulesoftMonitoringInstallDynaTrace-AccesstotheMulesoftenviron=

ment"\>Access to the Mulesoft environment\</h2\>

\<ul\>

\<li\>kubectl installed, awsauth etc. you can follow \<a
href=3D"/display/SEL/=

Setup+access+to+Mulesoft+kubernetes+environments"\>Setup access to
Mulesoft =

kubernetes environments\</a\>\</li\>

\</ul\>\</li\>

\</ul\>\</li\>

\</ul\>

\<p\>\<br\>\</p\>

\<ul\>

\<li\>\<h1
id=3D"MulesoftMonitoringInstallDynaTrace-InstallationofDynaTraceclo=

udNativeFullStack"\>Installation of DynaTrace
\<code\>cloudNativeFullStack\</co=

de\>\</h1\>

\<ul\>

\<li\>Checkout the documentation: \<a class=3D"external-link"
href=3D"https://=

www.dynatrace.com/support/help/shortlink/full-stack-dto-k8\#manual"
rel=3D"n=

ofollow"\>https://www.dynatrace.com/support/help/shortlink/full-stack-dto-k8=

\#manual\</a\>\</li\>

\<li\>\<p class=3D"auto-cursor-target"\>Create dynatrace namespace\</p\>

\<div class=3D"code panel pdl" style=3D"border-width: 1px;"\>

\<div class=3D"codeContent panelContent pdl"\>=20

\<pre class=3D"syntaxhighlighter-pre"
data-syntaxhighlighter-params=3D"brush=

: bash; gutter: false; theme: Emacs" data-theme=3D"Emacs"\>kubectl
create na=

mespace dynatrace\</pre\>=20

\</div\>

\</div\>\</li\>

\<li\>\<p class=3D"auto-cursor-target"\>Install kubernetes DT operatior
( if yo=

ur system doesn't have access to WWW, like the jumphost, then download
the =

file and rsync it to the jumphost or the host you are operation on
).\</p\>

\<div class=3D"code panel pdl" style=3D"border-width: 1px;"\>

\<div class=3D"codeContent panelContent pdl"\>=20

\<pre class=3D"syntaxhighlighter-pre"
data-syntaxhighlighter-params=3D"brush=

: bash; gutter: false; theme: Emacs" data-theme=3D"Emacs"\>kubectl apply
-f =

https://github.com/Dynatrace/dynatrace-operator/releases/download/v0.10.0/k=

ubernetes.yaml\</pre\>=20

\</div\>

\</div\>\</li\>

\<li\>\<p class=3D"auto-cursor-target"\>Expected output\</p\>

\<div class=3D"code panel pdl" style=3D"border-width: 1px;"\>

\<div class=3D"codeContent panelContent pdl"\>=20

\<pre class=3D"syntaxhighlighter-pre"
data-syntaxhighlighter-params=3D"brush=

: bash; gutter: false; theme: Emacs"
data-theme=3D"Emacs"\>poddisruptionbudg=

et.policy/dynatrace-webhook created

serviceaccount/dynatrace-activegate created

serviceaccount/dynatrace-kubernetes-monitoring created

serviceaccount/dynatrace-dynakube-oneagent-privileged created

serviceaccount/dynatrace-dynakube-oneagent-unprivileged created

serviceaccount/dynatrace-operator created

serviceaccount/dynatrace-webhook created

customresourcedefinition.apiextensions.k8s.io/dynakubes.dynatrace.com
creat=

ed

clusterrole.rbac.authorization.k8s.io/dynatrace-kubernetes-monitoring
creat=

ed

clusterrole.rbac.authorization.k8s.io/dynatrace-operator created

clusterrole.rbac.authorization.k8s.io/dynatrace-webhook created

clusterrolebinding.rbac.authorization.k8s.io/dynatrace-kubernetes-monitorin=

g created

clusterrolebinding.rbac.authorization.k8s.io/dynatrace-operator created

clusterrolebinding.rbac.authorization.k8s.io/dynatrace-webhook created

role.rbac.authorization.k8s.io/dynatrace-operator created

role.rbac.authorization.k8s.io/dynatrace-webhook created

rolebinding.rbac.authorization.k8s.io/dynatrace-operator created

rolebinding.rbac.authorization.k8s.io/dynatrace-webhook created

service/dynatrace-webhook created

deployment.apps/dynatrace-operator created

deployment.apps/dynatrace-webhook created

mutatingwebhookconfiguration.admissionregistration.k8s.io/dynatrace-webhook=

created

validatingwebhookconfiguration.admissionregistration.k8s.io/dynatrace-webho=

ok created\</pre\>=20

\</div\>

\</div\>\</li\>

\<li\>\<p class=3D"auto-cursor-target"\>Install kubernetes DT operatior
CSI age=

nt ( if your system doesn't have access to WWW, like the jumphost, then
dow=

nload the file and rsync it to the jumphost or the host you are
operation o=

n).\</p\>

\<div class=3D"code panel pdl" style=3D"border-width: 1px;"\>

\<div class=3D"codeContent panelContent pdl"\>=20

\<pre class=3D"syntaxhighlighter-pre"
data-syntaxhighlighter-params=3D"brush=

: bash; gutter: false; theme: Emacs" data-theme=3D"Emacs"\>kubectl apply
-f =

https://github.com/Dynatrace/dynatrace-operator/releases/download/v0.10.0/k=

ubernetes-csi.yaml\</pre\>=20

\</div\>

\</div\>\</li\>

\<li\>\<p class=3D"auto-cursor-target"\>Expected output\</p\>

\<div class=3D"code panel pdl" style=3D"border-width: 1px;"\>

\<div class=3D"codeContent panelContent pdl"\>=20

\<pre class=3D"syntaxhighlighter-pre"
data-syntaxhighlighter-params=3D"brush=

: bash; gutter: false; theme: Emacs"
data-theme=3D"Emacs"\>serviceaccount/dy=

natrace-oneagent-csi-driver created

clusterrole.rbac.authorization.k8s.io/dynatrace-oneagent-csi-driver
created

clusterrolebinding.rbac.authorization.k8s.io/dynatrace-oneagent-csi-driver
=

created

role.rbac.authorization.k8s.io/dynatrace-oneagent-csi-driver created

rolebinding.rbac.authorization.k8s.io/dynatrace-oneagent-csi-driver
created

daemonset.apps/dynatrace-oneagent-csi-driver created

csidriver.storage.k8s.io/csi.oneagent.dynatrace.com created

priorityclass.scheduling.k8s.io/dynatrace-high-priority
created\</pre\>=20

\</div\>

\</div\>\</li\>

\<li\>\<p class=3D"auto-cursor-target"\>Validate the installation so
far\</p\>

\<div class=3D"code panel pdl" style=3D"border-width: 1px;"\>

\<div class=3D"codeContent panelContent pdl"\>=20

\<pre class=3D"syntaxhighlighter-pre"
data-syntaxhighlighter-params=3D"brush=

: bash; gutter: false; theme: Emacs" data-theme=3D"Emacs"\>kubectl -n
dynatr=

ace wait pod --for=3Dcondition=3Dready
--selector=3Dapp.kubernetes.io/name=

\=3Ddynatrace-operator,app.kubernetes.io/component=3Dwebhook
--timeout=3D300=

s\</pre\>=20

\</div\>

\</div\>\</li\>

\<li\>\<p class=3D"auto-cursor-target"\>Expected output ( the trailing
hash wil=

l be different ).\</p\>

\<div class=3D"code panel pdl" style=3D"border-width: 1px;"\>

\<div class=3D"codeContent panelContent pdl"\>=20

\<pre class=3D"syntaxhighlighter-pre"
data-syntaxhighlighter-params=3D"brush=

: bash; gutter: false; theme: Emacs"
data-theme=3D"Emacs"\>pod/dynatrace-web=

hook-5c67d77f4c-57rvq condition met

pod/dynatrace-webhook-5c67d77f4c-tscqz condition met\</pre\>=20

\</div\>

\</div\>\</li\>

\<li\>Login to DynaTrace UI

\<ul\>

\<li\>Manage / DynaTrace Hub\</li\>

\<li\>TODO - missing the point where the tokens are generated\</li\>

\</ul\>\</li\>

\<li\>\<p class=3D"auto-cursor-target"\>For
\<strong\>cloudNativeFullStack\</stron=

g\> and applicationMonitoring, create a secret named dynakube holding
both t=

he API token and the dataIngestToken, see Tokens and permissions
required. =

Be sure to replace the placeholders (\&lt;...\&gt;) with your own
values.\</p\>

\<div class=3D"code panel pdl" style=3D"border-width: 1px;"\>

\<div class=3D"codeContent panelContent pdl"\>=20

\<pre class=3D"syntaxhighlighter-pre"
data-syntaxhighlighter-params=3D"brush=

: bash; gutter: false; theme: Emacs" data-theme=3D"Emacs"\>kubectl -n
dynatr=

ace create secret generic dynakube
--from-literal=3D"apiToken=3D\&lt;API\_TOK=

EN\&gt;"
--from-literal=3D"dataIngestToken=3D\&lt;DATA\_INGEST\_TOKEN\&gt;"\</pre=

\>=20

\</div\>

\</div\>\</li\>

\<li\>\<p class=3D"auto-cursor-target"\>Download the custom config of
DynaKube\<=

/p\>

\<div class=3D"code panel pdl" style=3D"border-width: 1px;"\>

\<div class=3D"codeContent panelContent pdl"\>=20

\<pre class=3D"syntaxhighlighter-pre"
data-syntaxhighlighter-params=3D"brush=

: bash; gutter: false; theme: Emacs" data-theme=3D"Emacs"\>wget
https://raw.=

githubusercontent.com/Dynatrace/dynatrace-operator/v0.10.0/assets/samples/c=

loudNativeFullStack.yaml\</pre\>=20

\</div\>

\</div\>\</li\>

\<li\>\<p class=3D"auto-cursor-target"\>Edit the downloaded file and
adjust the=

first few lines to look like this, MAKE SURE you give it metadata/name
as =

you wish to appear in Infrastructure/Kubernetes. This will be used as a
fil=

ter for all workloads/pods etc. Also make sure the tokens: are set to
"dyna=

kube"\</p\>

\<div class=3D"code panel pdl" style=3D"border-width: 1px;"\>

\<div class=3D"codeContent panelContent pdl"\>=20

\<pre class=3D"syntaxhighlighter-pre"
data-syntaxhighlighter-params=3D"brush=

: bash; gutter: false; theme: Emacs" data-theme=3D"Emacs"\>apiVersion:
dynat=

race.com/v1beta1

kind: DynaKube

metadata:

name: mule-stg-rtf

namespace: dynatrace

spec:

\# Dynatrace apiUrl including the \`/api\` path at the end.

\# For SaaS, set \`YOUR\_ENVIRONMENT\_ID\` to your environment ID.

\# For Managed, change the apiUrl address.

\# For instructions on how to determine the environment ID and how to
conf=

igure the apiUrl address, see
https://www.dynatrace.com/support/help/refere=

nce/dynatrace-concepts/environment-id/.

apiUrl: https://gah29713.live.dynatrace.com/api

\# Optional: Name of the secret holding the credentials required to
connec=

t to the Dynatrace tenant

\# If unset, the name of this custom resource is used

\#

tokens: "dynakube"

\</pre\>=20

\</div\>

\</div\>\</li\>

\<li\>\<p class=3D"auto-cursor-target"\>Install the DynaKube\</p\>

\<div class=3D"code panel pdl" style=3D"border-width: 1px;"\>

\<div class=3D"codeContent panelContent pdl"\>=20

\<pre class=3D"syntaxhighlighter-pre"
data-syntaxhighlighter-params=3D"brush=

: bash; gutter: false; theme: Emacs" data-theme=3D"Emacs"\>kubectl apply
-f =

cloudNativeFullStack.yaml\</pre\>=20

\</div\>

\</div\>\</li\>

\<li\>\<p class=3D"auto-cursor-target"\>Expected output\</p\>

\<div class=3D"code panel pdl" style=3D"border-width: 1px;"\>

\<div class=3D"codeContent panelContent pdl"\>=20

\<pre class=3D"syntaxhighlighter-pre"
data-syntaxhighlighter-params=3D"brush=

: bash; gutter: false; theme: Emacs"
data-theme=3D"Emacs"\>dynakube.dynatrac=

e.com/mule-stg-rtf created\</pre\>=20

\</div\>

\</div\>\</li\>

\<li\>\<p class=3D"auto-cursor-target"\>Pull the cluster ID as you will
need it=

to manually connect it in the Dynatrace UI\</p\>

\<div class=3D"code panel pdl" style=3D"border-width: 1px;"\>

\<div class=3D"codeContent panelContent pdl"\>=20

\<pre class=3D"syntaxhighlighter-pre"
data-syntaxhighlighter-params=3D"brush=

: bash; gutter: false; theme: Emacs" data-theme=3D"Emacs"\>kubectl get
names=

pace kube-system -o jsonpath=3D'{.metadata.uid}'\</pre\>=20

\</div\>

\</div\>\</li\>

\<li\>Login to Dynatrace UI\</li\>

\<li\>Checkout this documentation \<a class=3D"external-link"
href=3D"https://=

www.dynatrace.com/support/help/shortlink/deploy-ag-dynatrace-op\#local"
rel=

\=3D"nofollow"\>https://www.dynatrace.com/support/help/shortlink/deploy-ag-dy=

natrace-op\#local\</a\> , We'll use connect manually method\</li\>

\<li\>\<h4 class=3D"heading h4"
id=3D"MulesoftMonitoringInstallDynaTrace-Provi=

detheKubernetesclusterIDintheDynatracewebUI"\>Provide the Kubernetes
cluster=

ID in the Dynatrace web UI\</h4\>

\<ol class=3D"list list--ordered list"\>

\<li\>In the \<a class=3D"external-link"
href=3D"https://www.dynatrace.com/sup=

port/help/get-started/navigation" rel=3D"nofollow" title=3D"Learn about
usi=

ng the Dynatrace menu."\>Dynatrace menu\</a\>, go to
\<strong\>Kubernetes\</stron=

g\>.\</li\>

\<li\>Select \<strong\>Connect manually\</strong\>.\</li\>

\<li\>On the Kubernetes cluster monitoring settings page, provide a
\<strong\>N=

ame\</strong\>, and then turn on \<strong\>Connect containerized
ActiveGate to =

local Kubernetes API endpoint\</strong\>.\</li\>

\<li\>For \<strong\>Kubernetes cluster ID\</strong\>, enter the UID
obtained earl=

ier.\</li\>

\<li\>Select \<strong\>Save changes\</strong\> to save your
configuration. \<stron=

g\>Note:\</strong\> You can save your configuration even if the
ActiveGate isn=

't ready to connect, and finish the configuration later. To verify if
it's =

ready, select \<strong\>Test configuration\</strong\>.\</li\>

\</ol\>\</li\>

\<li\>Give it few minutes, when you navigate to
Infrastructure/Kubernetes you=

should see a new entry mule-rtf-stg.\</li\>

\<li\>Go to settings and enable "Events"\</li\>

\</ul\>\</li\>

\</ul\>

\<p\>\<br\>\</p\>

\<p\>\<br\>\</p\>

\</div\>

\</body\>

\</html\>

\------=\_Part\_40\_1516775522.1718011289795--