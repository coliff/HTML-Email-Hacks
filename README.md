 HTML-Email-Hacks
================

A series of HTML hacks for all those lovely Email clients out there

This repo is a place to put all of the HTML Email hacks we all depend on so much to get our campaigns looking and feeling sweet and spiffy. 

---

##Click To Tap:
####   Change button text responsivly
	
>@media screen and (max-width:600px) {<br>
>span[class=click] {display: none !important; max-height: 0 !important;}<br>
>span[class=tap]:after {content:”Tap”;}<br><br>

><a href=”#”&gt;<span class=”tap”&gt;<span class=”click”&gt;Click</span&gt;</span&gt; here</a&gt;
  
##Kill Gmail App Zooming:
####	  Stop Gmail app from zooming text
	  
>style=”min-width:600px;”
	 
##Target Webkit Clients:
####	  Webkit support is best support
	  
>@media screen and (-webkit-min-device-pixel-ratio:0) { }
  
##Margins and Float in Outlook:
####	  Use a capital “M” or “F”
	  
>style=”Margin: 20px; Float: left”

##Interactive Email in Gmail:
####	No Class or ID selector support

Use lang as selector with "x-" prefix<br>
>\* [lang~="x-selector"] { }<br>
><div lang="x-selector"&gt;

##Interactive Email con’t - Hover!:
####   Hover effect works on these clients:

Gmail: >* [lang~="x-selector"]:hover { }<br>
Outlook Web: >.class:hover<br>
Yahoo! Web: >.class:hover

##Outlook “View in Browser”:
#### 	Forces Outlook to provide a “view in browser link”

>\#outlook a {padding: 0;}

##Images in Outlook 2013:
#### 	Fix broken images in Outlook 2013

><td style=”line-height: 13px;”&gt;
	 <img src=”img.jpg”&gt;
></td&gt;

##Remove autolink styling in iOS:
#### 	Fix automatic styling of phone numbers, etc.

Use a span:
><span class=”appleLinksBlack”&gt;866-787-7030</span&gt;

##Stop some clients from stripping class:
#### 	Some clients strip any lines starting with “.”

Use a space before any class styleing
> .selector { }

##Hide content in Office 365 (incl GM Webmail):
#### 	Office 365 strips display, mso-hide, mso conditional

Set font-size in containing cell to “0px”<br>
><td style=”font-size: 0px; display: none;&gt;

##Good formatting for bulleted list:
#### 	Stops bullet from sitting between two lines

><table&gt;  
>&nbsp;&nbsp;&nbsp;&nbsp;  <tr&gt;  
>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;      <td valign=”top”&gt;&amp;bull;</td&gt;  
>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;      <td&gt;Prolongs oil life</td&gt;  
>&nbsp;&nbsp;&nbsp;&nbsp;  </tr&gt;  
></table&gt;
