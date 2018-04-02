---


manager: soliver
ms.date: 3/9/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- VS.SharePointTools.BDC.AssociationReference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e32c5267-53b0-9ff0-6e9a-1cb00d9f1d57
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
<td align="left"># AssociationReference Element in AssociationGroup (BDCMetadata Schema)</td>
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

**Applies to**: SharePoint 2016 | SharePoint Foundation 2013 |
SharePoint Online | SharePoint Server 2013

Specifies an **AssociationReference** in an
**AssociationGroup**.

**Namespace**:
http://schemas.microsoft.com/windows/2007/BusinessDataCatalog

**Schema**: BDCMetadata

<span codelanguage="xmlLang"></span>
<table>
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">XML</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><pre><code><AssociationReference EntityNamespace = "String" EntityName = "String" AssociationName = "String" Reverse = "Boolean"> </AssociationReference></code></pre></td>
</tr>
</tbody>
</table>


--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

The following sections describe attributes, child elements, and parent
elements.

#### Attributes

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
<td align="left"><p>EntityNamespace</p></td>
<td align="left"><p>Optional.</p>
<p>The namespace of the external content type where the **Association</span> is defined. If **EntityName</span> is specified, **EntityNamespace** is required.</p>
<p>Attribute type: **String**</p></td>
</tr>
<tr class="even">
<td align="left"><p>EntityName</p></td>
<td align="left"><p>Optional.</p>
<p>The name of the external content type where the **Association</span> is defined. If **EntityNamespace</span> is specified, **EntityName** is required.</p>
<p>Attribute type: **String**</p></td>
</tr>
<tr class="odd">
<td align="left"><p>AssociationName</p></td>
<td align="left"><p>Required.</p>
<p>The name of the **Association**.</p>
<p>Attribute type: **String**</p></td>
</tr>
<tr class="even">
<td align="left"><p>Reverse</p></td>
<td align="left"><p>Optional.</p>
<p>Specifies that the referenced **Association</span> has its source and destination reversed. This would indicate the **Association</span> is working in the opposite direction compared to other associations in the same **AssociationGroup</span>. For example, if the **AssociationGroup</span> references an **Association</span> "GetOrdersForCustomer", returning Order items for the given Customer item, then the **AssociationGroup</span> is in the direction of Customer to Order. The other **AssociationReference**, referencing another association "GetCustomerForOrder", must be marked as reverse, because this association is in the direction of Order to Customer.</p>
<p>Default value: **false**</p>
<p>Attribute type: **Boolean**</p></td>
</tr>
</tbody>
</table>

#### Child elements

None.

#### Parent elements

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th align="left"><p>Element</p></th>
<th align="left"><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p><span sdata="link"><a href="associationgroup-element-in-associationgroups-bdcmetadata-schema.md">AssociationGroup Element in AssociationGroups (BDCMetadata Schema)</a></span></p></td>
<td align="left"><p>The **AssociationGroup</span> that this **AssociationReference** belongs to.</p></td>
</tr>
</tbody>
</table>








