---


manager: soliver
ms.date: 3/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AlertTemplates schema
api_type:
- schema
ms.assetid: d4bdd815-8bbd-40d2-821c-926aa3128ad1
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
<td align="left"># Properties Element (AlertTemplates)</td>
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

Excludes fields from the list that is displayed in the alert message.

<span codelanguage="other"></span>
<table>
<colgroup>
<col width="100%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><pre><code><Properties>
  [<ImmediateNotificationExcludedFields>
    ...
  </ImmediateNotificationExcludedFields>]  [<DigestNotificationExcludedFields>
    ...
  </DigestNotificationExcludedFields>]
  [<NotificationHandlerAssembly>
  </NotificationHandlerAssembly>]  [<NotificationHandlerClassName>
  </NotificationHandlerClassName>]
  [<UpdateHandlerAssembly>
  </UpdateHandlerAssembly>]  [<UpdateHandlerClassName>
  </UpdateHandlerClassName>]
</Properties></code></pre></td>
</tr>
</tbody>
</table>


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

None


---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<table>
<colgroup>
<col width="100%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><p><a href="immediatenotificationexcludedfields-element-alerttemplates.md">ImmediateNotificationExcludedFields</a></p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="digestnotificationexcludedfields-element-alerttemplates.md">DigestNotificationExcludedFields</a></p></td>
</tr>
<tr class="odd">
<td align="left"><p><a href="notificationhandlerassembly-element-alert-templates.md">NotificationHandlerAssembly</a></p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="notificationhandlerclassname-element-alerttemplates.md">NotificationHandlerClassName</a></p></td>
</tr>
<tr class="odd">
<td align="left"><p><a href="updatehandlerassembly-element-alerttemplates.md">UpdateHandlerAssembly</a></p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="updatehandlerclassname-element-alerttemplates.md">UpdateHandlerClassName</a></p></td>
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
<td align="left"><p><a href="alerttemplate-element-alerttemplates.md">AlertTemplate</a></p></td>
</tr>
</tbody>
</table>


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<span codelanguage="xmlLang"></span>
XML 
<span class="copyCode" onclick="CopyCode(this)"
onkeypress="CopyCode_CheckKey(this, event)"
onmouseover="ChangeCopyCodeIcon(this)"
onmouseout="ChangeCopyCodeIcon(this)" tabindex="0">![Copy
code] "Copy code")Copy code</span>
    <Properties>
       <ImmediateNotificationExcludedFields>
          ID;Author;Editor;Modified_x0020_By;Created_x0020_By;
          _UIVersionString;ContentType;TaskGroup;IsCurrent;Attachments;
          NumComments;
       </ImmediateNotificationExcludedFields>
       <DigestNotificationExcludedFields>
          ID;Author;Editor;Modified_x0020_By;Created_x0020_By;
          _UIVersionString;ContentType;TaskGroup;IsCurrent;Attachments;
          NumComments;
       </DigestNotificationExcludedFields>
    </Properties>








