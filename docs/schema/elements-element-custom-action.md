---


manager: soliver
ms.date: 3/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a0b64f14-48d9-4149-b7cd-eb86c95856ca
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
<td align="left"># Elements Element (Custom Action)</td>
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

Top-level element in a Feature manifest file that contains Feature
element declarations.

<span codelanguage="other"></span>
<table>
<colgroup>
<col width="100%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><pre><code><Elements
  Id = "Text">
</Elements></code></pre></td>
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
<td align="left"><p>**xmlns**</p></td>
<td align="left"><p>Required. Identifies the XML namespace. The value must be <span class="code">http://schemas.microsoft.com/sharepoint/</span>.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**Id**</p></td>
<td align="left"><p>Optional **Text**. Specifies a unique identifier for the Feature manifest file.</p></td>
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
<td align="left"><p><a href="customaction-element.md">CustomAction</a></p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="customactiongroup-element-custom-action.md">CustomActionGroup</a></p></td>
</tr>
<tr class="odd">
<td align="left"><p><a href="hidecustomaction-element.md">HideCustomAction</a></p></td>
</tr>
</tbody>
</table>


----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

None


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

The following example defines a custom action that adds a button to the
Server ribbon.

## Definition
XML 
<span class="copyCode" onclick="CopyCode(this)"
onkeypress="CopyCode_CheckKey(this, event)"
onmouseover="ChangeCopyCodeIcon(this)"
onmouseout="ChangeCopyCodeIcon(this)" tabindex="0">![Copy
code] "Copy code")Copy code</span>
    <Elements xmlns="http://schemas.microsoft.com/sharepoint/">
      <CustomAction 
        Id="Ribbon.Library.Actions.AddAButton"
        Location="CommandUI.Ribbon"
        RegistrationId="101"
        RegistrationType="List"
        Title="Add a Ribbon Button">
        <CommandUIExtension>
          <CommandUIDefinitions>
            <CommandUIDefinition
              Location="Ribbon.Library.Share.Controls._children">
              <Button Id="Ribbon.Library.Share.NewRibbonButton"
                Command="NewRibbonButtonCommand"
                Image16by16="Insert an image URL here."
                Image32by32="Insert an image URL here."
                LabelText="Hello World"
                TemplateAlias="o2" />
            </CommandUIDefinition>
          </CommandUIDefinitions>
          <CommandUIHandlers>
            <CommandUIHandler 
              Command="NewRibbonButtonCommand"
              CommandAction="javascript:alert('Hello, world');" />
          </CommandUIHandlers>
        </CommandUIExtension>
      </CustomAction>
    </Elements>








