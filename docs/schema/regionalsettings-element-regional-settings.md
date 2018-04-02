---


manager: soliver
ms.date: 3/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Regional Settings schema
api_type:
- schema
ms.assetid: d0d3ccfc-881f-4c50-8811-dd875b9555c9
---

![Collapse
section]![Expand
section] "Expand section")![]()![])![]![]()![Copy
code] "Copy code")![Copy code
hover]
<table>
<tbody>
<tr class="odd">
<td align="left"></td>
</tr>
</tbody>
</table>

Visual Basic  
C\#  
C++  
JavaScript  

<table>
<tbody>
<tr class="odd">
<td align="left"><span id="runningHeaderText"></span></td>
</tr>
<tr class="even">
<td align="left"># RegionalSettings Element (Regional Settings)</td>
</tr>
<tr class="odd">
<td align="left"><a href="#exampleToggle">Example</a>  <span id="headfeedbackarea" class="feedbackhead"><a href="javascript:SubmitFeedback(&#39;docthis@Microsoft.com&#39;,&#39;&#39;,&#39;&#39;,&#39;&#39;,&#39;1.0.18082.1225&#39;,&#39;%0\dThank%20you%20for%20your%20feedback.%20The%20developer%20writing%20teams%20use%20your%20feedback%20to%20improve%20documentation.%20While%20we%20are%20reviewing%20your%20feedback,%20we%20may%20send%20you%20e-mail%20to%20ask%20for%20clarification%20or%20feedback%20on%20a%20solution.%20We%20do%20not%20use%20your%20e-mail%20address%20for%20any%20other%20purpose%20and%20we%20delete%20it%20after%20we%20finish%20our%20review.%0\AFor%20further%20information%20about%20the%20privacy%20policies%20of%20Microsoft,%20please%20see%20http://privacy.microsoft.com/en-us/default.aspx.%0\A%0\d&#39;,&#39;Customer%20feedback&#39;);">Send feedback</a></span></td>
</tr>
</tbody>
</table>

<table>
<colgroup>
<col width="100%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"></td>
</tr>
</tbody>
</table>

**Last modified:** March 09, 2015

**Applies to**: SharePoint 2016 | SharePoint Foundation 2013 |
SharePoint Online | SharePoint Server 2013

Contains the regional settings for currency, language, locale, and time
zone that are used in the deployment of Microsoft SharePoint Foundation.
Used in TIMEZONE.XML (%ProgramFiles%\\Common Files\\Microsoft
Shared\\web server extensions\\15\\CONFIG). and RGNLSTNG.XML
(%ProgramFiles%\\Common Files\\Microsoft Shared\\web server
extensions\\15\\TEMPLATE\\1033\\XML).

<span codelanguage="other"></span>
<table>
<colgroup>
<col width="100%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><pre><code><RegionalSettings>
</RegionalSettings></code></pre></td>
</tr>
</tbody>
</table>


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th align="left"><p>Attribute</p></th>
<th align="left"><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>None</p></td>
<td align="left"><p>N/A</p></td>
</tr>
</tbody>
</table>


---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<table>
<colgroup>
<col width="100%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><p><a href="currencies-element-regional-settings.md">Currencies</a>, <a href="languages-element-regional-settings.md">Languages</a>, <a href="locales-element-regional-settings.md">Locales</a>, <a href="timezones-element-regional-settings.md">TimeZones</a></p></td>
</tr>
</tbody>
</table>


----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<table>
<colgroup>
<col width="100%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><p>None</p></td>
</tr>
</tbody>
</table>


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<table>
<colgroup>
<col width="100%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><p>Minimum: 0</p>
<p>Maximum: 1</p></td>
</tr>
</tbody>
</table>


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

The following example outlines the structure of the file TIMEZONE.XML.

<span codelanguage="xmlLang"></span>
XML 
<span class="copyCode" onclick="CopyCode(this)"
onkeypress="CopyCode_CheckKey(this, event)"
onmouseover="ChangeCopyCodeIcon(this)"
onmouseout="ChangeCopyCodeIcon(this)" tabindex="0">![Copy
code] "Copy code")Copy code</span>
    <RegionalSettings>
      <TimeZones>
      ...
        <TimeZone ID="13" Name="(GMT-08:00) Pacific Time (US and Canada); 
          Tijuana" Hidden="FALSE">
          <Bias>480</Bias>
          <StandardTime>
            <Bias>0</Bias>
            <Date>
              <Month>10</Month>
               <Day>5</Day>
               <Hour>2</Hour>
             </Date>
           </StandardTime>
           <DaylightTime>
             <Bias>-60</Bias>
             <Date>
               <Month>4</Month>
               <Day>1</Day>
               <Hour>2</Hour>
              </Date>
            </DaylightTime>
          </TimeZone>
          <TimeZone ID="14" Name="(GMT-09:00) Alaska" Hidden="FALSE">
            <Bias>540</Bias>
            <StandardTime>
              <Bias>0</Bias>
              <Date>
                <Month>10</Month>
                <Day>5</Day>
                <Hour>2</Hour>
              </Date>
            </StandardTime>
            <DaylightTime>
              <Bias>-60</Bias>
              <Date>
                <Month>4</Month>
                <Day>1</Day>
                <Hour>2</Hour>
              </Date>
            </DaylightTime>
          </TimeZone>
          ...
      </TimeZones>
    </RegionalSettings>








