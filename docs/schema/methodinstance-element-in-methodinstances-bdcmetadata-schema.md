---


manager: soliver
ms.date: 3/9/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- VS.SharePointTools.BDC.MethodInstance
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 577ff9d0-706b-be7d-af5b-883e137cada8
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
<td align="left"># MethodInstance Element in MethodInstances (BDCMetadata Schema)</td>
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

Specifies a **MethodInstance**.

**Namespace**:
http://schemas.microsoft.com/windows/2007/BusinessDataCatalog

**Schema**: BDCMetadata

The following two cases in a BDC model result in an
[InvalidOperationException](http://msdn.microsoft.com/library/frlrfSystemInvalidOperationExceptionClassTopic.aspx)
at run time:

-   Two **SpecificFinder** method instances
    that return the same set of fields.

-   Two **SpecificFinder** method instances
    that have the same number of fields and that share the same number
    of fields with another method instance, such as a <span
    class="keyword">Finder</span>.

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
<td align="left"><pre><code><MethodInstance Type = "String" Default = "Boolean" ReturnParameterName = "String" ReturnTypeDescriptorName = "String" ReturnTypeDescriptorLevel = "Integer" Name = "String" DefaultDisplayName = "String" IsCached = "Boolean"> </MethodInstance></code></pre></td>
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
<td align="left"><p>Type</p></td>
<td align="left"><p>Required.</p>
<p>Specifies the type of the **MethodInstance**.</p>
<p>The following table lists the possible values for this attribute.</p>
<div class="tableSection">
<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th align="left"><p>Value</p></th>
<th align="left"><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>Finder</p></td>
<td align="left"><p>A type of **MethodInstance</span> that can be called to return a collection of zero or more **EntityInstances</span> of a particular **Entity</span>. **Finder</span> input is defined by the **FilterDescriptors</span> that are contained in the **Method</span> that contains the **Finder**.</p></td>
</tr>
<tr class="even">
<td align="left"><p>SpecificFinder</p></td>
<td align="left"><p>A type of **MethodInstance</span> that can be called to return a specific **EntityInstance</span> of a specific **Entity</span> given its **EntityInstanceId</span>. **SpecificFinder</span> input is defined and ordered by the **Identifiers</span> that are associated with the **Entity**.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>GenericInvoker</p></td>
<td align="left"><p>A type of **MethodInstance</span> that can be called to perform a specific task in an external system. **GenericInvoker</span> input and output is specific to the **Method**.</p></td>
</tr>
<tr class="even">
<td align="left"><p>IdEnumerator</p></td>
<td align="left"><p>A type of **MethodInstance</span> that can be called to return the **Field</span> values that represent the identity of **EntityInstances</span> of a specific **Entity</span>. The **IdEnumerator</span> input is defined by the **FilterDescriptors</span> that are contained in the method that contains the **IdEnumerator** to get the list of IDs, which are the unique keys for each entity that should be searchable. This method instance enables external data search in Microsoft SharePoint Server 2010.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>ChangedIdEnumerator</p></td>
<td align="left"><p>A type of **MethodInstance</span> that can be called to retrieve **EntityInstanceIds</span> of **EntityInstances** that were modified in an external system after a specified time.</p></td>
</tr>
<tr class="even">
<td align="left"><p>DeletedIdEnumerator</p></td>
<td align="left"><p>A type of **MethodInstance</span> that can be called to retrieve **EntityInstanceIds</span> of **EntityInstances** that were deleted from an external system after the specified time.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>Scalar</p></td>
<td align="left"><p>A **MethodInstance</span> that returns a single value that you can invoke in the external system. For example, you can use a scalar method instance to get the total sales made to date from the external system. **Entities** have zero or more scalar method instances.</p></td>
</tr>
<tr class="even">
<td align="left"><p>AccessChecker</p></td>
<td align="left"><p>A type of **MethodInstance</span> that can be called to retrieve the permissions that the calling security principal has for each of a collection of **EntityInstances</span> that are identified by the specified **EntityInstanceIds**.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>Creator</p></td>
<td align="left"><p>A type of **MethodInstance</span> that can be called to create an **EntityInstance</span>. The set of fields that are required to create the **EntityInstance** is referred to as the Creator View.</p></td>
</tr>
<tr class="even">
<td align="left"><p>Deleter</p></td>
<td align="left"><p>A type of **MethodInstance</span> that can be called to delete an **EntityInstance</span> with a specified **EntityInstanceId**.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>Updater</p></td>
<td align="left"><p>A type of **MethodInstance</span> that can be called to update an **EntityInstance</span> identified by a specified **EntityInstanceId</span>. The set of fields that is required to update the **EntityInstance** is known as the Updater View. The set of fields whose values should be passed before they are changed is known as the PreUpdater View.</p></td>
</tr>
<tr class="even">
<td align="left"><p>StreamAccessor</p></td>
<td align="left"><p>A type of **MethodInstance</span> that can be called to retrieve a field of an **EntityInstance** in the form of a data stream of bytes.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>BinarySecurityDescriptorAccessor</p></td>
<td align="left"><p>A type of **MethodInstance</span> that can be called to retrieve a sequence of bytes from an external system. The system-specific byte sequence describes a set of security principals and the associated permissions that each security principal has for the **EntityInstance</span> identified by a specified **EntityInstanceId**.</p></td>
</tr>
<tr class="even">
<td align="left"><p>BulkSpecificFinder</p></td>
<td align="left"><p>A type of **MethodInstance</span> that can be called to return a set of specific **EntityInstances</span> of an **Entity</span>, given a set of corresponding **EntityInstanceIds**.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>BulkIdEnumerator</p></td>
<td align="left"><p>A type of **MethodInstance</span> that can be called to retrieve minimal information about the external items corresponding to the given identities. This method instance can be used to optimize synchronization of cached data. This method should return only the identities and version information of the external items that correspond to given **Identities**, which the calling application can compare with the local version to identify if anything has changed, and if so, request the changed external items to update the cached data.</p></td>
</tr>
</tbody>
</table>
</div></td>
</tr>
<tr class="even">
<td align="left"><p>Default</p></td>
<td align="left"><p>Optional.</p>
<p>Specifies whether the **MethodInstance</span> is the default among all **MethodInstances</span> that share its type within the containing external content type (**Entity**).</p>
<p>Default value: **false**</p>
<p>Attribute type: **Boolean**</p></td>
</tr>
<tr class="odd">
<td align="left"><p>ReturnParameterName</p></td>
<td align="left"><p>Optional.</p>
<p>The name of the **Parameter</span> that contains the **ReturnTypeDescriptor</span> of the **MethodInstance</span>. The **Direction</span> attribute of the **Parameter</span> must be a **ParameterDirection</span> attribute with a value of **Out</span>, **InOut</span>, or **Return**.</p>
<p>This attribute must be specified for all types of **MethodInstances</span> except **GenericInvoker</span>, **Creator</span>, **Deleter</span>, and **Updater**.</p>
<p>Attribute type: **String**</p></td>
</tr>
<tr class="even">
<td align="left"><p>ReturnTypeDescriptorLevel</p></td>
<td align="left"><p>Optional.</p>
<p>This has been deprecated. Use the **ReturnTypeDescriptorPath** instead.</p>
<p>Attribute type: **Integer**</p></td>
</tr>
<tr class="odd">
<td align="left"><p>ReturnTypeDescriptorPath</p></td>
<td align="left"><p>Optional.</p>
<p>The dotted path of the **TypeDescriptor** of the Association.</p>
<p>Attribute type: **String**</p></td>
</tr>
<tr class="even">
<td align="left"><p>Name</p></td>
<td align="left"><p>Required.</p>
<p>Specifies the name of the **MethodInstance**.</p>
<p>Attribute type: **String**</p></td>
</tr>
<tr class="odd">
<td align="left"><p>DefaultDisplayName</p></td>
<td align="left"><p>Optional.</p>
<p>Specifies the default display name for the **MethodInstance**.</p>
<p>Attribute type: **String**</p></td>
</tr>
<tr class="even">
<td align="left"><p>IsCached</p></td>
<td align="left"><p>Optional.</p>
<p>Specifies whether the **MethodInstance** is used frequently.</p>
<p>Default value: **true**</p>
<p>Attribute type: **Boolean**</p></td>
</tr>
</tbody>
</table>

#### Child elements

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
<td align="left"><p><span sdata="link"><a href="localizeddisplaynames-element-in-metadataobject-bdcmetadata-schema.md">LocalizedDisplayNames Element in MetadataObject (BDCMetadata Schema)</a></span></p></td>
<td align="left"><p>The localized display names of the **MethodInstance**.</p></td>
</tr>
<tr class="even">
<td align="left"><p><span sdata="link"><a href="properties-element-in-metadataobject-bdcmetadata-schema.md">Properties Element in MetadataObject (BDCMetadata Schema)</a></span></p></td>
<td align="left"><p>The properties of the **MethodInstance**.</p></td>
</tr>
<tr class="odd">
<td align="left"><p><span sdata="link"><a href="accesscontrollist-element-bdcmetadata-schema.md">AccessControlList Element (BDCMetadata Schema)</a></span></p></td>
<td align="left"><p>The access control lists (ACLs) of the **MethodInstance**.</p></td>
</tr>
</tbody>
</table>

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
<td align="left"><p><span sdata="link"><a href="methodinstances-element-in-method-bdcmetadata-schema.md">MethodInstances Element in Method (BDCMetadata Schema)</a></span></p></td>
<td align="left"><p>The **MethodInstances</span> element that contains this **MethodInstance**.</p></td>
</tr>
</tbody>
</table>








