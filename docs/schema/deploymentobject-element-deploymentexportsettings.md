---


manager: soliver
ms.date: 3/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 128f7174-b2d1-4150-a966-c1abfc0e1bf8
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
<td align="left"># DeploymentObject Element (DeploymentExportSettings)</td>
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

Represents a deployment object or objects (<span sdata="cer"
target="T:Microsoft.SharePoint.Deployment.SPExportObject"><span
class="nolink">SPExportObject</span></span>) marked for export to the
content migration package.

<span codelanguage="other"></span>
<table>
<colgroup>
<col width="100%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><pre><code>DECLARATION
<xs:element
        name="DeploymentObject" type="SPExportObject"
        minOccurs="0" maxOccurs="unbounded" 
/>

USAGE
<DeploymentObject
        <!-- SPDeploymentObject -->
        <xs:attribute name="Id" type="Guid" />
        <xs:attribute name="Type" type="SPDeploymentObjectType" />
        <xs:attribute name="ParentId" type="Guid" />

        <!-- SPExportObject -->
        <xs:attribute name="Url" type="xs:string" />
        <xs:attribute name="ExcludeChildren" type="xs:boolean" />
        <xs:attribute name="IncludeDescendants" type="SPIncludeDescendants" />
        <xs:attribute name="ExportChangeToken" type="xs:string" />
/></code></pre></td>
</tr>
</tbody>
</table>


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<span sdata="cer"
target="T:Microsoft.SharePoint.Deployment.SPExportObject"><span
class="nolink">SPExportObject</span></span>


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
<td align="left"><p>**Id**</p></td>
<td align="left"><p><span sdata="link"><a href="guid-simple-type-deploymentexportsettings.md">Guid Simple Type (DeploymentExportSettings)</a></span></p></td>
<td align="left"><p>Optional. Unique identifier of the export object.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**Type**</p></td>
<td align="left"><p><span sdata="link"><a href="spdeploymentobjecttype-simple-type-deploymentexportsettings.md">SPDeploymentObjectType Simple Type (DeploymentExportSettings)</a></span></p></td>
<td align="left"><p>Optional. Enumeration providing values to specify the object type.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**ParentId**</p></td>
<td align="left"><p><span sdata="link"><a href="guid-simple-type-deploymentexportsettings.md">Guid Simple Type (DeploymentExportSettings)</a></span></p></td>
<td align="left"><p>Optional. Unique identifier of the object's parent site.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**Url**</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional. URL to the location of the export object.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**ExcludeChildren**</p></td>
<td align="left"><p>xs:boolean</p></td>
<td align="left"><p>Optional. Specifies whether to exclude child objects (descendants). The value is **true</span> if children are excluded. The default is **false**.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**IncludeDescendants**</p></td>
<td align="left"><p><span sdata="link"><a href="spincludedescendents-simple-type-deploymentexportsettings.md">SPIncludeDescendents Simple Type (DeploymentExportSettings)</a></span></p></td>
<td align="left"><p>Optional. Enumeration providing values to specify which descendents, if any, to include in the content migration package.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**ExportChangeToken**</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional. Specifies the change token to use when exporting incremental changes based on changes since the last export.</p></td>
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
<td align="left"><p><span sdata="link"><a href="exportobjects-element-deploymentexportsettings.md">ExportObjects Element (DeploymentExportSettings)</a></span></p></td>
</tr>
</tbody>
</table>


-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

#### Reference

<span sdata="cer"
target="T:Microsoft.SharePoint.Deployment.SPExportObject"><span
class="nolink">SPExportObject</span></span>

#### Concepts

[DeploymentExportSettings
Schema](deploymentexportsettings-schema.md)</span>








