---


manager: soliver
ms.date: 3/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c90bc0c-03a4-48c3-80f9-e8f974edb8c6
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
<td align="left"># File Element (DeploymentManifest - SPFileVersionCollection)</td>
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

Represents a versioned instance of a SharePoint Foundation 2010 file
(<span sdata="cer" target="T:Microsoft.SharePoint.SPFile"><span
class="nolink">SPFile</span></span>) object.

<span codelanguage="other"></span>
<table>
<colgroup>
<col width="100%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><pre><code>DECLARATION
<xs:element name="File" 
        type="SPFile" 
        minOccurs="1" maxOccurs="unbounded" 
/>

USAGE
<Versions>
        <File
                Name="xs:string"
                Id="Guid"
                Url="xs:string"
                ListItemIntId="xs:int"
                ParentWebId="Guid"
                ParentWebUrl="xs:string"
                ParentId="Guid"
                ListId="Guid"
                FileValue="xs:string"
                CheckinComment="xs:string"
                Version="xs:string"
                Author="xs:string"
                ModifiedBy="xs:string"
                TimeCreated="xs:dateTime"
                TimeLastModified="xs:dateTime"
                FailureMessage="xs:string"
                IsGhosted="xs:boolean"
                SetupPath="Guid"
                SetupPathUser="xs:string"
                SetupPathVersion="xs:byte"
                    <Properties />
                        <Versions />
                        <WebParts />
                        <Personalizations />
                        <Links />
                        <EventReceivers />
        />
</Versions></code></pre></td>
</tr>
</tbody>
</table>


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<span sdata="cer" target="T:Microsoft.SharePoint.SPFile"><span
class="nolink">SPFile</span></span>


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
<td align="left"><p>**Name**</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional. Name of the file.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**Id**</p></td>
<td align="left"><p><span sdata="link"><a href="guid-simple-type-deploymentmanifest.md">Guid Simple Type (DeploymentManifest)</a></span></p></td>
<td align="left"><p>Optional. Unique identifier of the file.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**Url**</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional. The Web site-relative URL of the file.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**ListItemIntId**</p></td>
<td align="left"><p>xs:int</p></td>
<td align="left"><p>Optional. Integer identifier specifying the list item relative to position in a document library.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**ParentWebId**</p></td>
<td align="left"><p><span sdata="link"><a href="guid-simple-type-deploymentmanifest.md">Guid Simple Type (DeploymentManifest)</a></span></p></td>
<td align="left"><p>Optional. Unique identifier of parent Web site.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**ParentWebUrl**</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional. URL of the parent Web site.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**ParentId**</p></td>
<td align="left"><p><span sdata="link"><a href="guid-simple-type-deploymentmanifest.md">Guid Simple Type (DeploymentManifest)</a></span></p></td>
<td align="left"><p>Optional. Unique identifier of the parent folder for the file.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**ListId**</p></td>
<td align="left"><p><span sdata="link"><a href="guid-simple-type-deploymentmanifest.md">Guid Simple Type (DeploymentManifest)</a></span></p></td>
<td align="left"><p>Optional. Unique identifier of the list in which the file exists. **ListId</span> values must match values for the **Versions** attribute.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**FileValue**</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional. Specifies the location of the file on disk.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**CheckinComment**</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional. Comments provided on file checkin.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**Versions**</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional. Represents a collection of file version objects that specify file versions.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**Author**</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional. The user who created or uploaded the file.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**ModifiedBy**</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional. The user who last modified the file.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**TimeCreated**</p></td>
<td align="left"><p>xs:dateTime</p></td>
<td align="left"><p>Optional. Date-time value representing the time the file was created or uploaded.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**TimeLastModified**</p></td>
<td align="left"><p>xs:dateTime</p></td>
<td align="left"><p>Optional. Date-time value representing the time the file was last modified.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**FailureMessage**</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional. Message represented on failure at export or import.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**IsGhosted**</p></td>
<td align="left"><p>xs:boolean</p></td>
<td align="left"><p>Optional. Specifies whether the file exists on the front end (and not in the database), and therefore does not require a roundtrip to the database server.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**SetupPath**</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional. Path to the front-end file location in cases where the **IsGhosted</span> attribute is **true**.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**SetupPathUser**</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional. Person who initially created the list in the document library.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**SetupPathVersion**</p></td>
<td align="left"><p>xs:byte</p></td>
<td align="left"><p>Optional. Specifies Microsoft SharePoint Foundation version. The value **2</span> specifies Windows SharePoint Services 2.0; the value **3** specifies Windows SharePoint Services 3.0.</p></td>
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
<td align="left"><p><span sdata="link"><a href="eventreceivers-element-deploymentmanifestspfile.md">EventReceivers Element (DeploymentManifest - SPFile)</a></span></p></td>
</tr>
<tr class="even">
<td align="left"><p><span sdata="link"><a href="links-element-deploymentmanifestspfile.md">Links Element (DeploymentManifest - SPFile)</a></span></p></td>
</tr>
<tr class="odd">
<td align="left"><p><span sdata="link"><a href="personalizations-element-deploymentmanifest.md">Personalizations Element (DeploymentManifest)</a></span></p></td>
</tr>
<tr class="even">
<td align="left"><p><span sdata="link"><a href="properties-element-deploymentmanifestspfile.md">Properties Element (DeploymentManifest - SPFile)</a></span></p></td>
</tr>
<tr class="odd">
<td align="left"><p><span sdata="link"><a href="versions-element-deploymentmanifestspfile.md">Versions Element (DeploymentManifest - SPFile)</a></span></p></td>
</tr>
<tr class="even">
<td align="left"><p><span sdata="link"><a href="webparts-element-deploymentmanifest.md">WebParts Element (DeploymentManifest)</a></span></p></td>
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
<td align="left"><p><span sdata="link"><a href="versions-element-deploymentmanifestspfile.md">Versions Element (DeploymentManifest - SPFile)</a></span></p></td>
</tr>
</tbody>
</table>


-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

#### Reference

<span sdata="cer" target="T:Microsoft.SharePoint.SPFile"><span
class="nolink">SPFile</span></span>

#### Concepts

[DeploymentManifest
Schema](deploymentmanifest-schema.md)</span>








