---


manager: arnek
ms.date: 3/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fce44c4e-eaab-e94b-bff7-c08795fb5cc1
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
<td align="left"># Source complexType (SPS15XSDSearchSet1)</td>
</tr>
<tr class="odd">
<td align="left"><span id="headfeedbackarea" class="feedbackhead"><a href="javascript:SubmitFeedback(&#39;docthis@Microsoft.com&#39;,&#39;&#39;,&#39;&#39;,&#39;&#39;,&#39;1.0.18082.1225&#39;,&#39;%0\dThank%20you%20for%20your%20feedback.%20The%20developer%20writing%20teams%20use%20your%20feedback%20to%20improve%20documentation.%20While%20we%20are%20reviewing%20your%20feedback,%20we%20may%20send%20you%20e-mail%20to%20ask%20for%20clarification%20or%20feedback%20on%20a%20solution.%20We%20do%20not%20use%20your%20e-mail%20address%20for%20any%20other%20purpose%20and%20we%20delete%20it%20after%20we%20finish%20our%20review.%0\AFor%20further%20information%20about%20the%20privacy%20policies%20of%20Microsoft,%20please%20see%20http://privacy.microsoft.com/en-us/default.aspx.%0\A%0\d&#39;,&#39;Customer%20feedback&#39;);">Send feedback</a></span></td>
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

**Applies to**: SharePoint Server 2013


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><p><span class="label">Namespace</span></p></td>
<td align="left"><p>http://schemas.datacontract.org/2004/07/Microsoft.Office.Server.Search.Administration.Query</p></td>
</tr>
<tr class="even">
<td align="left"><p><span class="label">Schema file</span></p></td>
<td align="left"><p>schema_Microsoft.Office.Server.Search.Administration.Query.xsd</p></td>
</tr>
<tr class="odd">
<td align="left"><p><span class="label">Extension base</span></p></td>
<td align="left"><p>None</p></td>
</tr>
</tbody>
</table>


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Definition
XML 
<span class="copyCode" onclick="CopyCode(this)"
onkeypress="CopyCode_CheckKey(this, event)"
onmouseover="ChangeCopyCodeIcon(this)"
onmouseout="ChangeCopyCodeIcon(this)" tabindex="0">![Copy
code] "Copy code")Copy code</span>
    <xs:complexType name="Source">
        <xs:sequence>
            <xs:element name="Active" type="xs:boolean" minOccurs="0"></xs:element>
            <xs:element name="AuthInfo" type="q1:AuthenticationInformation" minOccurs="0"></xs:element>
            <xs:element name="BuiltIn" type="xs:boolean" minOccurs="0"></xs:element>
            <xs:element name="ConnectionTimeout" type="xs:int" minOccurs="0"></xs:element>
            <xs:element name="ConnectionUrlTemplate" type="xs:string" minOccurs="0"></xs:element>
            <xs:element name="CreatedDate" type="xs:dateTime" minOccurs="0"></xs:element>
            <xs:element name="Description" type="xs:string" minOccurs="0"></xs:element>
            <xs:element name="HasPermissionToReadAuthInfo" type="xs:boolean" minOccurs="0"></xs:element>
            <xs:element name="Id" type="ser:guid" minOccurs="0"></xs:element>
            <xs:element name="IndexOffset" type="xs:int" minOccurs="0"></xs:element>
            <xs:element name="LastModifiedDate" type="xs:dateTime" minOccurs="0"></xs:element>
            <xs:element name="MaximumResponseLength" type="xs:int" minOccurs="0"></xs:element>
            <xs:element name="Name" type="xs:string" minOccurs="0"></xs:element>
            <xs:element name="Owner" type="q2:SearchObjectOwner" minOccurs="0"></xs:element>
            <xs:element name="ProviderId" type="ser:guid" minOccurs="0"></xs:element>
            <xs:element name="QueryTransform" type="q3:QueryTransform" minOccurs="0"></xs:element>
        </xs:sequence>
    </xs:complexType>


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

If the schema defines specific requirements, such as **sequence**, **minOccurs**, **maxOccurs**, and **choice**, see the definition section.
## Elements and attributes class="keyword">sequence</span>, **minOccurs**,
**maxOccurs**, and <span
class="keyword">choice</span>, see the definition section.

### Child elements

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th align="left"><p>Element</p></th>
<th align="left"><p>Type</p></th>
<th align="left"><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p><a href="active-element-source-complextypesps15xsdsearchset1.md">Active</a></p></td>
<td align="left"><p>xs:boolean</p></td>
<td align="left"><p></p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="authinfo-element-source-complextypesps15xsdsearchset1.md">AuthInfo</a></p></td>
<td align="left"><p>q1:AuthenticationInformation</p></td>
<td align="left"><p></p></td>
</tr>
<tr class="odd">
<td align="left"><p><a href="builtin-element-source-complextypesps15xsdsearchset1.md">BuiltIn</a></p></td>
<td align="left"><p>xs:boolean</p></td>
<td align="left"><p></p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="connectiontimeout-element-source-complextypesps15xsdsearchset1.md">ConnectionTimeout</a></p></td>
<td align="left"><p>xs:int</p></td>
<td align="left"><p></p></td>
</tr>
<tr class="odd">
<td align="left"><p><a href="connectionurltemplate-element-source-complextypesps15xsdsearchset1.md">ConnectionUrlTemplate</a></p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p></p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="createddate-element-source-complextypesps15xsdsearchset1.md">CreatedDate</a></p></td>
<td align="left"><p>xs:dateTime</p></td>
<td align="left"><p></p></td>
</tr>
<tr class="odd">
<td align="left"><p><a href="description-element-source-complextypesps15xsdsearchset1.md">Description</a></p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p></p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="haspermissiontoreadauthinfo-element-source-complextypesps15xsdsearchset1.md">HasPermissionToReadAuthInfo</a></p></td>
<td align="left"><p>xs:boolean</p></td>
<td align="left"><p></p></td>
</tr>
<tr class="odd">
<td align="left"><p><a href="id-element-source-complextypesps15xsdsearchset1.md">Id</a></p></td>
<td align="left"><p>ser:guid</p></td>
<td align="left"><p></p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="indexoffset-element-source-complextypesps15xsdsearchset1.md">IndexOffset</a></p></td>
<td align="left"><p>xs:int</p></td>
<td align="left"><p></p></td>
</tr>
<tr class="odd">
<td align="left"><p><a href="lastmodifieddate-element-source-complextypesps15xsdsearchset1.md">LastModifiedDate</a></p></td>
<td align="left"><p>xs:dateTime</p></td>
<td align="left"><p></p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="maximumresponselength-element-source-complextypesps15xsdsearchset1.md">MaximumResponseLength</a></p></td>
<td align="left"><p>xs:int</p></td>
<td align="left"><p></p></td>
</tr>
<tr class="odd">
<td align="left"><p><a href="name-element-source-complextypesps15xsdsearchset1.md">Name</a></p></td>
<td align="left"><p>xs:string</p></td>
<td align="left"><p></p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="owner-element-source-complextypesps15xsdsearchset1.md">Owner</a></p></td>
<td align="left"><p>q2:SearchObjectOwner</p></td>
<td align="left"><p></p></td>
</tr>
<tr class="odd">
<td align="left"><p><a href="providerid-element-source-complextypesps15xsdsearchset1.md">ProviderId</a></p></td>
<td align="left"><p>ser:guid</p></td>
<td align="left"><p></p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="querytransform-element-source-complextypesps15xsdsearchset1.md">QueryTransform</a></p></td>
<td align="left"><p>q3:QueryTransform</p></td>
<td align="left"><p></p></td>
</tr>
</tbody>
</table>

### Attributes

None.








