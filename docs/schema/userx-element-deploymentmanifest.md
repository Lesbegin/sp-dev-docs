---


manager: soliver
ms.date: 3/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ac4e829e-699c-4856-87a3-a3c534edd861
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
<td align="left"># UserX Element (DeploymentManifest)</td>
</tr>
<tr class="odd">
<td align="left"><a href="#seeAlsoToggle">See also</a>  <span id="headfeedbackarea" class="feedbackhead"><a href="javascript:SubmitFeedback(&#39;docthis@Microsoft.com&#39;,&#39;&#39;,&#39;&#39;,&#39;&#39;,&#39;1.0.18082.1225&#39;,&#39;%0\dThank%20you%20for%20your%20feedback.%20The%20developer%20writing%20teams%20use%20your%20feedback%20to%20improve%20documentation.%20While%20we%20are%20reviewing%20your%20feedback,%20we%20may%20send%20you%20e-mail%20to%20ask%20for%20clarification%20or%20feedback%20on%20a%20solution.%20We%20do%20not%20use%20your%20e-mail%20address%20for%20any%20other%20purpose%20and%20we%20delete%20it%20after%20we%20finish%20our%20review.%0\AFor%20further%20information%20about%20the%20privacy%20policies%20of%20Microsoft,%20please%20see%20http://privacy.microsoft.com/en-us/default.aspx.%0\A%0\d&#39;,&#39;Customer%20feedback&#39;);">Send feedback</a></span></td>
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

Represents incremental changes to an <span sdata="cer"
target="T:Microsoft.SharePoint.SPUser"><span
class="nolink">SPUser</span></span> object defintion during an
incremental deployment.

<span codelanguage="other"></span>
<table>
<colgroup>
<col width="100%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><pre><code>DECLARATION
<xs:element name="UserX" type="DeploymentUserX" />

USAGE
<SPObject>
        <UserX
                Operation="SecurityModificationType"
                Id="xs:string"
                Name="xs:string"
                Login="xs:string"
                Email="xs:string"
                SystemId="xs:string"
                IsDomainGroup="xs:boolean"
                IsSiteAdmin="xs:boolean"
                IsDeleted="xs:boolean"
        />
</SPObject></code></pre></td>
</tr>
</tbody>
</table>


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**DeploymentUserX** (based on <span sdata="cer"
target="T:Microsoft.SharePoint.SPUser"><span
class="nolink">SPUser</span></span>)


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th align="left"><p>Attribute</p></th>
<th align="left"><p>Type</p></th>
<th align="left"><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>**Email**</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional. Provides the e-mail address of the user.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**Id**</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Required. Provides the member ID for the user.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**IsDeleted**</p></td>
<td align="left"><p>xs:boolean</p></td>
<td align="left"><p>Optional.Specifies whether the user has been deleted.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**IsDomainGroup**</p></td>
<td align="left"><p>xs:boolean</p></td>
<td align="left"><p>Optional. Specifies whether the user is a domain group; **true</span> if the user is a domain group, otherwise **false**.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**IsSiteAdmin**</p></td>
<td align="left"><p>xs:boolean</p></td>
<td align="left"><p>Optional. Specifies whether the user is a site collection administrator; **true</span> if the user is a site collection administrator, otherwise **false**.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**Login**</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional. Provides the user name of the user.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**Name**</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Required. Provides the display name of the user.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**Operation**</p></td>
<td align="left"><p><span sdata="link"><a href="securitymodificationtype-simple-type-deploymentmanifest.md">SecurityModificationType Simple Type (DeploymentManifest)</a></span></p></td>
<td align="left"><p>Required. Enumeration type that provides values to specify which security modifications are allowed.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**SystemId**</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional.</p></td>
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
<td align="left"><p>None</p></td>
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
<td align="left"><p><span sdata="link"><a href="spobject-element-deploymentmanifest.md">SPObject Element (DeploymentManifest)</a></span></p></td>
</tr>
</tbody>
</table>


-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

#### Reference

<span sdata="cer" target="T:Microsoft.SharePoint.SPUser"><span
class="nolink">SPUser</span></span>

#### Concepts

[DeploymentManifest
Schema](deploymentmanifest-schema.md)</span>








