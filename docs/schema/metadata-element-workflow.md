---


manager: soliver
ms.date: 3/9/2015
ms.audience: Developer
ms.topic: reference
keywords:
- workflow definition schema, metadata element (workflow)
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c454e18c-ea94-4dd1-8081-a25a8acbacef
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
<td align="left"># MetaData Element (Workflow)</td>
</tr>
<tr class="odd">
<td align="left"><a href="#exampleToggle">Example</a>  <a href="#seeAlsoToggle">See also</a>  <span id="headfeedbackarea" class="feedbackhead"><a href="javascript:SubmitFeedback(&#39;docthis@Microsoft.com&#39;,&#39;&#39;,&#39;&#39;,&#39;&#39;,&#39;1.0.18082.1225&#39;,&#39;%0\dThank%20you%20for%20your%20feedback.%20The%20developer%20writing%20teams%20use%20your%20feedback%20to%20improve%20documentation.%20While%20we%20are%20reviewing%20your%20feedback,%20we%20may%20send%20you%20e-mail%20to%20ask%20for%20clarification%20or%20feedback%20on%20a%20solution.%20We%20do%20not%20use%20your%20e-mail%20address%20for%20any%20other%20purpose%20and%20we%20delete%20it%20after%20we%20finish%20our%20review.%0\AFor%20further%20information%20about%20the%20privacy%20policies%20of%20Microsoft,%20please%20see%20http://privacy.microsoft.com/en-us/default.aspx.%0\A%0\d&#39;,&#39;Customer%20feedback&#39;);">Send feedback</a></span></td>
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

Contains any additional, custom metadata elements that are valid XML for
the workflow.

<span codelanguage="other"></span>
<table>
<colgroup>
<col width="100%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><pre><code><MetaData>
</Metadata></code></pre></td>
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
<td align="left"><p>**None**</p></td>
<td align="left"><p></p></td>
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
<td align="left"><p>None.</p></td>
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
<td align="left"><p><span sdata="link"><a href="workflow-element-elements.md">Workflow Element (Elements)</a></span></p></td>
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


----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

SharePoint Foundation uses the following elements to define additional
workflow information in the **MetaData**
element:

-   **InitiationType**

-   **Modification\_GUID\_Name **

-   **StatusPageUrl**

-   **ExtendedStatusColumnValues**


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Following is an example of a **Metadata**
element containing information on how the workflow can be initiated, the
name of a workflow modification contained in the workflow, and custom
status column values.

## Definition
XML 
<span class="copyCode" onclick="CopyCode(this)"
onkeypress="CopyCode_CheckKey(this, event)"
onmouseover="ChangeCopyCodeIcon(this)"
onmouseout="ChangeCopyCodeIcon(this)" tabindex="0">![Copy
code] "Copy code")Copy code</span>
      <MetaData>
        <InitiationType>Manual;#OnNewItem;#OnItemUpdate;#OnMajorCheckIn</InitiationType>
        <Modification_af71f77b-e6c8-483a-acbf-30b4a84bd209_Name>myWorkflowModification</Modification_af71f77b-e6c8-483a-acbf-30b4a84bd209_Name>
        <Modification_Format><my:myFields xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:my="http://schemas.adventureworks.com/workflows/myXSD">{0}</my:myFields></Modification_Format>
        <StatusPageUrl>_layouts/myWrkStat.aspx</StatusPageUrl>
        <ExtendedStatusColumnValues>
          <StatusColumnValue>Canceled</StatusColumnValue>
          <StatusColumnValue>Approved</StatusColumnValue>
          <StatusColumnValue>Rejected</StatusColumnValue>
        </ExtendedStatusColumnValues>  
      </MetaData>


-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

#### Concepts

[Workflow
Definitions](workflow-definitions.md)</span>

#### Other resources

[Workflows in Windows SharePoint
Services](http://msdn.microsoft.com/library/be0888d4-20b2-4d39-bf28-2d8a71829d8e(Office.15).aspx)

[Workflow Deployment Using
Features](http://msdn.microsoft.com/library/ad294f09-483d-4e87-bd19-fa37795ed558(Office.15).aspx)








