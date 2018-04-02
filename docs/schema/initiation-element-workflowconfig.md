---


manager: laurawi
ms.date: 3/9/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- SharePoint workflows
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5aab14eb-fa08-4917-b0d3-5f25626f5509
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
<td align="left"># Initiation Element (WorkflowConfig)</td>
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

Contains workflow initiation information, such as the workflow
initiation form, and the data fields on the initiation form.

<span codelanguage="other"></span>
<table>
<colgroup>
<col width="100%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><pre><code><Initiation URL="Text"
</Initiation></code></pre></td>
</tr>
</tbody>
</table>


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><p>Attribute</p></td>
<td align="left"><p>Description</p></td>
</tr>
<tr class="even">
<td align="left"><p>**URL**</p></td>
<td align="left"><p>Required **Text**. Specifies the path to the workflow initiation form for the workflow.</p>
<p>The path specified must be relative to the location of the workflow configuration file.</p></td>
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
<td align="left"><p><span sdata="link"><a href="parameters-element-workflowconfig.md">Parameters Element (WorkflowConfig)</a></span></p>
<p><span sdata="link"><a href="fields-element-workflowconfig.md">Fields Element (WorkflowConfig)</a></span></p></td>
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
<td align="left"><p><span sdata="link"><a href="workflowconfig-element.md">WorkflowConfig Element</a></span></p></td>
</tr>
</tbody>
</table>


----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

The initiation form specified should contain a data field for each <span
sdata="link">[Field Element
(Field)](field-element-field.md)</span> element
defined in the [Fields Element
(WorkflowConfig)](fields-element-workflowconfig.md)</span>
section of the workflow configuration file. If a data field is not
present, the default value is used when the workflow starts.

Once the workflow has been associated with a specific SharePoint list,
the contents of the URL attribute are stored in the <span sdata="cer"
target="P:Microsoft.SharePoint.Workflow.SPWorkflowTemplate.InstantiationUrl"><span
class="nolink">InstantiationUrl</span></span> property of the <span
sdata="cer"
target="T:Microsoft.SharePoint.Workflow.SPWorkflowTemplate"><span
class="nolink">SPWorkflowTemplate</span></span> and <span sdata="cer"
target="T:Microsoft.SharePoint.Workflow.SPWorkflowAssociation"><span
class="nolink">SPWorkflowAssociation</span></span> objects for the
workflow.

Applications created to work as a declarative rules-based, code-free
workflow editor can use the <span sdata="cer"
target="M:websvcWebPartPages.WebPartPagesWebService.AssociateWorkflowMarkup(System.String,System.String)">**AssociateWorkflowMarkup(String,
String)**</span> method of the <span sdata="cer"
target="N:websvcWebPartPages">**websvcWebPartPages**</span> Web Service
to create a workflow template and associate it to a SharePoint list
specifying a workflow markup file, a workflow configuration file, and
optionally, a workflow rules markup file.

For more information about creating an application that can act as a
declarative rules-based, code-free workflow editor, see [Creating
Declarative, No-Code Workflow
Editors](http://msdn.microsoft.com/library/60dfda8d-e724-4d7d-9578-aa239c362dcf(Office.15).aspx).


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

The following example Initiation element contains a URL attribute that
specifies the location of the workflow initiation form to use for this
workflow.

The element also contains a Fields element, which in turn contains a
Field element that defines the single data field on the initiation form.
Note that the Parameters element contains a corresponding Parameter
element, with a matching Name attribute value, that specifies the data
type of the Field element.

This example has been edited for clarity.

<span codelanguage="xmlLang"></span>
XML 
<span class="copyCode" onclick="CopyCode(this)"
onkeypress="CopyCode_CheckKey(this, event)"
onmouseover="ChangeCopyCodeIcon(this)"
onmouseout="ChangeCopyCodeIcon(this)" tabindex="0">![Copy
code] "Copy code")Copy code</span>
    <Initiation 
        URL="Workflows/Notify Me/Notify Me.aspx">
      <Fields>
        <Field 
          Name="Reason_for_Review" 
          …
          DisplayName="Reason_for_Review" 
          …
        >
          <Default>Standard review of new documents</Default>
        </Field>
      </Fields>
      <Parameters>
        <Parameter Name="Reason_for_Review" Type="System.String" />
      </Parameters>
    </Initiation>


-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

#### Concepts

[Workflow configuration schema
reference](workflow-configuration-schema-reference.md)</span>

#### Other resources

[Workflow Development for Windows SharePoint
Services](http://msdn.microsoft.com/library/ad7a5bf2-fab0-4b30-ae0b-46b15f16b491(Office.15).aspx)

[Creating Declarative, No-Code Workflow
Editors](http://msdn.microsoft.com/library/60dfda8d-e724-4d7d-9578-aa239c362dcf(Office.15).aspx)

[Office SharePoint Designer 2007
Overview](http://msdn.microsoft.com/library/5ef4e933-564e-4dea-b2f4-c1b621774969(Office.15).aspx)








