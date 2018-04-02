---


manager: soliver
ms.date: 3/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c78cfef-9a58-42ae-a7ca-a5f2e61668ac
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
<td align="left"># Attachment Element (DeploymentManifest)</td>
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

Represents an instance of a Windows SharePoint Services 3.0 attachment
object (**SPAttachment**).

<span codelanguage="other"></span>
<table>
<colgroup>
<col width="100%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><pre><code>DELCARATION
<xs:element name="Attachment" 
      type="SPAttachment" 
      minOccurs="0" maxOccurs="unbounded" 
/>

USAGE
<ListItem>
        <Attachments>
                <Attachment>
                        Name="xs:string"
                        DirName="xs:string"
                        Url="xs:string"
                        Id="Guid"
                        ParentWebId="Guid"
                        FileValue="xs:string"
                        MetaInfo="xs:string"
                        Author="xs:string"
                        ModifiedBy="xs:string"
                        TimeCreated="xs:dateTime"
                        TimeLastModified="xs:dateTime"
                        FailureMessage="xs:string"
                                <Properties />
                </Attachment>
        </Attachments>
</ListItem></code></pre></td>
</tr>
</tbody>
</table>


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**SPAttachement**


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
<td align="left"><p>Required. Attachment file name.</p></td>
</tr>
<tr class="even">
<td align="left"><p>DirName</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional. Url to the directory in which the attachment file is located.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>Url</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional. Web-relative URL to the attachment file (DirName plus file name).</p></td>
</tr>
<tr class="even">
<td align="left"><p>Id</p></td>
<td align="left"><p>Guid</p></td>
<td align="left"><p>Optional. Unique identifier of the attachment file.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>ParentWebId</p></td>
<td align="left"><p>Guid</p></td>
<td align="left"><p>Optional. Unique identifier of the parent Web.</p></td>
</tr>
<tr class="even">
<td align="left"><p>FileValue</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Required. Identifier of the attachment file as maintained by the export package.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>MetaInfo</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional. Property bag values for the attachment file.</p></td>
</tr>
<tr class="even">
<td align="left"><p>Author</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional. User who created or uploaded the attachment file.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>ModifiedBy</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional. Any user who modified the attachment file.</p></td>
</tr>
<tr class="even">
<td align="left"><p>TimeCreated</p></td>
<td align="left"><p>xs:dateTime</p></td>
<td align="left"><p>Optional. Time the attachment file was created or uploaded.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>TimeLastModified</p></td>
<td align="left"><p>xs:dateTime</p></td>
<td align="left"><p>Optional. Time the file was last modified.</p></td>
</tr>
<tr class="even">
<td align="left"><p>FailureMessage</p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p>Optional. Export failure message.</p></td>
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
<td align="left"><p><span sdata="link"><a href="properties-element-deploymentmanifestspattachment.md">Properties Element (DeploymentManifest - SPAttachment)</a></span></p></td>
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
<td align="left"><p><span sdata="link"><a href="attachments-element-deploymentmanifest.md">Attachments Element (DeploymentManifest)</a></span></p></td>
</tr>
</tbody>
</table>


----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Attachments are available for any list items that are not part of a
document library.


-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

#### Reference

<span sdata="cer"
target="T:Microsoft.SharePoint.SPAttachmentCollection"><span
class="nolink">SPAttachmentCollection</span></span>

#### Concepts

[DeploymentManifest
Schema](deploymentmanifest-schema.md)</span>








