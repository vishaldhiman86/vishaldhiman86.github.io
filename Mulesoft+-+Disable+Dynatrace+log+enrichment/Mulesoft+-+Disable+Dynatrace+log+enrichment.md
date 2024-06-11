Date: Mon, 10 Jun 2024 02:24:06 -0700 (PDT)

Message-ID:
\<1889093415.45.1718011446259@vswcrpcnfap02.crp.allegiantair.com\>

Subject: Exported From Confluence

MIME-Version: 1.0

Content-Type: multipart/related;

boundary="----=\_Part\_44\_1911085740.1718011446258"

\------=\_Part\_44\_1911085740.1718011446258

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

\<title\>Mulesoft - Disable Dynatrace log enrichment\</title\>

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

\<h1\>Mulesoft - Disable Dynatrace log enrichment\</h1\>

\<div class=3D"Section1"\>

\<p style=3D""\>Having 'Java' trace id's pollutes app logs making it =

difficult to analyze and troubleshoot. Each newly deployed app needs to
hav=

e 'Java trace id'' logs disabled to make it easier for the developers to
an=

alyze the logs. We do this by adding overrides in DynaTrace User
Interface.=

\</p\>

\<p style=3D""\>\<br\>\</p\>

\<p style=3D""\>1. Login to DT\</p\>

\<p style=3D""\>2. Go to\<span\>\&nbsp;\</span\>\<a
class=3D"external-link" href=3D=

"https://gah29713.live.dynatrace.com/ui/entity/list/CONTAINER\_GROUP?gtf=3D-=

2h\&amp;gf=3Dall\&amp;sessionId=3Di1fmb7P2IpZ0jF3A" rel=3D"nofollow"
style=3D=

""\>https://gah29713.live.dynatrace.com/ui/entity/list/CONTAINER\_GROUP?gtf=

\=3D-2h\&amp;gf=3Dall\&amp;sessionId=3Di1fmb7P2IpZ0jF3A\</a\>\&nbsp;
(This should=

take you to the container groups section)\</p\>

\<p style=3D""\>3. Filter by\<span\>\&nbsp;\</span\>\<a
class=3D"external-link" hre=

f=3D"http://k8s.container.name/" rel=3D"nofollow"
style=3D""\>K8s.container.=

name\</a\>\<span\>\&nbsp;\</span\>=3D 'app' and k8s.namespace =3D
ENV\_NAMESPACE\</p=

\>

\<p style=3D""\>4. Click on the desired application\</p\>

\<p style=3D""\>5. Scroll down to the "Process group" section\</p\>

\<p style=3D""\>6. Select the group Name\</p\>

\<p style=3D""\>7. Click on top right "Settings" button\</p\>

\<p style=3D""\>8. Go to "OneAgent features" from the menu\</p\>

\<p style=3D""\>9. Click on "Add override"\</p\>

\<p style=3D""\>10. Select "Java - Trace/span context enrichment for
logs"\</p=

\>

\<p style=3D""\>11. Select "Java - Trace/span context enrichment for
unstruct=

ured logs"\</p\>

\<p style=3D""\>12. The override will have the switch turned "off" by
default=

\</p\>

\<p style=3D""\>13. Click "save changes" on bottom left\</p\>

\<p style=3D""\>\<u\>\<strong\>\*\* NOTE : THE FOLLOWING STEPS WILL PUT
THE SELECTE=

D APPLICATION IN DOWNTIME AND WILL CAUSE AN
OUTAGE\&nbsp;\*\*\</strong\>\</u\>\</p\>

\<p style=3D""\>14. Login to AnyPoint Runtime Manager \<a
class=3D"external-li=

nk" href=3D"https://anypoint.mulesoft.com/login/"
rel=3D"nofollow"\>https://=

anypoint.mulesoft.com/login/\</a\>\&nbsp; \&nbsp; \&nbsp;(Using custom
domain "A=

llegiant")\</p\>

\<p style=3D""\>15. Click the hamburger menu on the top left and
selecting Ru=

ntime Manager\</p\>

\<p style=3D""\>16. Select the desired environment\</p\>

\<p style=3D""\>17. Select the application, clicking on the app
name\</p\>

\<p style=3D""\>18. Click "Stop" button top right\</p\>

\<p style=3D""\>19. Wait for a message "Desired configuration applied
success=

fully (At this point the Application status should be 'NOT
RUNNING')\</p\>

\<p style=3D""\>20. Start the app, click on "Enable" button top right
(Wait f=

or the 'Desired configuration applied successfully' message)\</p\>

\<p style=3D""\>\<strong\>\*\* Above mentioned steps are needed for the
changes t=

o take place \*\*\</strong\>\</p\>

\</div\>

\</body\>

\</html\>

\------=\_Part\_44\_1911085740.1718011446258--
