Date: Mon, 10 Jun 2024 02:24:35 -0700 (PDT)

Message-ID:
\<1377868537.57.1718011475701@vswcrpcnfap02.crp.allegiantair.com\>

Subject: Exported From Confluence

MIME-Version: 1.0

Content-Type: multipart/related;

boundary="----=\_Part\_56\_702431809.1718011475700"

\------=\_Part\_56\_702431809.1718011475700

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

\<title\>Mulesoft SSL certificates matrix\</title\>

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

\<h1\>Mulesoft SSL certificates matrix\</h1\>

\<div class=3D"Section1"\>

\<p\>\<br\>\</p\>

\<div class=3D"table-wrap"\>

\<table class=3D"wrapped confluenceTable"\>

\<colgroup\>

\<col\>

\<col\>

\<col\>

\<col\>

\</colgroup\>

\<tbody\>

\<tr\>

\<th class=3D"confluenceTh"\>ENV\</th\>

\<th class=3D"confluenceTh"\>EXT/INT CN\</th\>

\<th class=3D"confluenceTh"\>current cert EXP date\</th\>

\<th class=3D"confluenceTh"\>Authority\</th\>

\</tr\>

\<tr\>

\<td class=3D"confluenceTd"\>DEV-EXT\</td\>

\<td class=3D"confluenceTd"\>\<p\>\<a class=3D"external-link"
href=3D"http://ext=

.dev.api.aws.allegiantair.com"
rel=3D"nofollow"\>ext.dev.api.aws.allegiantai=

r.com\</a\>\</p\>\</td\>

\<td class=3D"confluenceTd"\>\<span class=3D"info" title=3D"6/5/2024,
8:40:32 =

AM (Pacific Daylight Time)"\>Wed, 05 Jun 2024 15:40:32
GMT\</span\>\</td\>

\<td class=3D"confluenceTd"\>GoDaddy\</td\>

\</tr\>

\<tr\>

\<td class=3D"confluenceTd"\>DEV-INT\</td\>

\<td class=3D"confluenceTd"\>\<a class=3D"external-link"
href=3D"http://dev.ap=

i.aws.allegiantair.com"
rel=3D"nofollow"\>dev.api.aws.allegiantair.com\</a\>\</=

td\>

\<td class=3D"confluenceTd"\>\<span class=3D"info" title=3D"9/19/2024,
10:27:0=

2 AM (Pacific Daylight Time)"\>Thu, 19 Sep 2024 17:27:02
GMT\</span\>\</td\>

\<td class=3D"confluenceTd"\>GoDaddy\</td\>

\</tr\>

\<tr\>

\<td class=3D"confluenceTd"\>QA-EXT\</td\>

\<td class=3D"confluenceTd"\>\<a class=3D"external-link"
href=3D"http://ext.de=

v.api.aws.allegiantair.com"
rel=3D"nofollow"\>ext.qa.api.aws.allegiantair.co=

m\</a\>\</td\>

\<td class=3D"confluenceTd"\>\<span class=3D"info" title=3D"6/5/2024,
8:26:17 =

AM (Pacific Daylight Time)"\>Wed, 05 Jun 2024 15:26:17
GMT\</span\>\</td\>

\<td class=3D"confluenceTd"\>GoDaddy\</td\>

\</tr\>

\<tr\>

\<td colspan=3D"1" class=3D"confluenceTd"\>QA-INT\</td\>

\<td colspan=3D"1" class=3D"confluenceTd"\>\<a class=3D"external-link"
href=3D=

"http://qa.api.aws.allegiantair.com"
rel=3D"nofollow"\>qa.api.aws.allegianta=

ir.com\</a\>\</td\>

\<td colspan=3D"1" class=3D"confluenceTd"\>\<span class=3D"info"
title=3D"9/28=

/2024, 9:24:21 AM (Pacific Daylight Time)"\>Sat, 28 Sep 2024 16:24:21
GMT\</s=

pan\>\</td\>

\<td colspan=3D"1" class=3D"confluenceTd"\>GoDaddy\</td\>

\</tr\>

\<tr\>

\<td colspan=3D"1" class=3D"confluenceTd"\>STG-EXT\</td\>

\<td colspan=3D"1" class=3D"confluenceTd"\>\<a class=3D"external-link"
href=3D=

"http://ext.qa.api.aws.allegiantair.com"
rel=3D"nofollow"\>ext.stg.api.aws.a=

llegiantair.com\</a\>\</td\>

\<td colspan=3D"1" class=3D"confluenceTd"\>Wed, 26 Jun 2024 18:27:18
GMT\</td\>

\<td colspan=3D"1" class=3D"confluenceTd"\>GoDaddy\</td\>

\</tr\>

\<tr\>

\<td colspan=3D"1" class=3D"confluenceTd"\>STG-INT\</td\>

\<td colspan=3D"1" class=3D"confluenceTd"\>\<a class=3D"external-link"
href=3D=

"http://ext.stg.api.aws.allegiantair.com"
rel=3D"nofollow"\>stg.api.aws.alle=

giantair.com\</a\>\</td\>

\<td colspan=3D"1" class=3D"confluenceTd"\>\<span class=3D"info"
title=3D"6/26=

/2024, 11:27:16 AM (Pacific Daylight Time)"\>Wed, 26 Jun 2024 18:27:16
GMT\</=

span\>\</td\>

\<td colspan=3D"1" class=3D"confluenceTd"\>GoDaddy\</td\>

\</tr\>

\<tr\>

\<td colspan=3D"1" class=3D"confluenceTd"\>PRD-EXT\</td\>

\<td colspan=3D"1" class=3D"confluenceTd"\>\<a class=3D"external-link"
href=3D=

"http://ext.api.aws.allegiantair.com"
rel=3D"nofollow"\>ext.api.aws.allegian=

tair.com\</a\>\</td\>

\<td colspan=3D"1" class=3D"confluenceTd"\>June 27, 2024 at 7:04:55
AM\</td\>

\<td colspan=3D"1" class=3D"confluenceTd"\>GoDaddy\</td\>

\</tr\>

\<tr\>

\<td colspan=3D"1" class=3D"confluenceTd"\>PRD-INT\</td\>

\<td colspan=3D"1" class=3D"confluenceTd"\>\<a class=3D"external-link"
href=3D=

"http://ext.api.aws.allegiantair.com"
rel=3D"nofollow"\>api.aws.allegiantair=

.com\</a\>\</td\>

\<td colspan=3D"1" class=3D"confluenceTd"\>\<p\>June 23, 2024 at 7:10:13
AM\</p\>=

\</td\>

\<td colspan=3D"1" class=3D"confluenceTd"\>GoDaddy\</td\>

\</tr\>

\</tbody\>

\</table\>

\</div\>

\</div\>

\</body\>

\</html\>

\------=\_Part\_56\_702431809.1718011475700--