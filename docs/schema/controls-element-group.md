---


manager: soliver
ms.date: 3/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Server Ribbon schema
api_type:
- schema
ms.assetid: d3635d99-fb58-4327-864f-6e59b222833d
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
<td align="left"># Controls Element (Group)</td>
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

Contains elements that define controls.

<span codelanguage="other"></span>
<table>
<colgroup>
<col width="100%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><pre><code><Controls
     Id="Text"
     ToolTipImage32by32="Url"
     ToolTipImage32by32Class="CSS Class Selector"
     ToolTipImage32by32Left="Negative Integer"
     ToolTipImage32by32Top="Negative Integer"
     ToolTipTitle="Text"
     ToolTipDescription="Text"
     ToolTipHelpKeyWord="Text"
     ToolTipShortcutKey="Text"
/></code></pre></td>
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
<td align="left"><p>**Id**</p></td>
<td align="left"><p>Required. Identifies the control. The value can be a string representation of a GUID or a unique term such as "Ribbon.Library.Share.NewRibbonCheckBox".</p></td>
</tr>
<tr class="even">
<td align="left"><p>**ToolTipImage32by32**</p></td>
<td align="left"><p>Optional. A server-relative URL to a file that contains a 32-by-32-pixel image to be used in the tooltip, such as "/_layouts/1033/images/formatmap32x32.png".</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**ToolTipImage32by32Class**</p></td>
<td align="left"><p>Optional. The name of a CSS class selector to be applied to the tooltip image.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**ToolTipImage32by32Left**</p></td>
<td align="left"><p>Optional. A negative integer that represents an offset for the left edge of the image. Use this attribute when the **ToolTipImage32by32</span> attribute points to an image file that contains the images for many icons. The value of the **ToolTipImage32by32Left</span> attribute is used to set the CSS **left</span> attribute for the inline style of an HTML **img** tag when the page is created.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**ToolTipImage32by32Top**</p></td>
<td align="left"><p>Optional. A negative integer that represents an offset for the top edge of the image. Use this attribute when the **ToolTipImage32by32</span> attribute points to an image file that contains the images for many icons. The value of the **ToolTipImage32by32Top</span> attribute is used to set the CSS **top</span> attribute for the inline style of an HTML **img** tag when the page is created.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**ToolTipTitle**</p></td>
<td align="left"><p>Optional. The text that appears as the title of the tooltip.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**ToolTipDescription**</p></td>
<td align="left"><p>Optional. The text that appears in the body of the tooltip.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**ToolTipHelpKeyWord**</p></td>
<td align="left"><p>Optional. The keyword that is used by context-sensitive Help.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**ToolTipShortcutKey**</p></td>
<td align="left"><p>Optional. The text to display for the shortcut key in the tooltip. For example, if the shortcut key for the control is ALT + J, then the value for this attribute is "ALT + J". The tooltip will display the text for the shortcut key in parentheses after the tooltip title: "(ALT + J)".</p></td>
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
<td align="left"><p><a href="button-element.md">Button</a></p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="checkbox-element.md">CheckBox</a></p></td>
</tr>
<tr class="odd">
<td align="left"><p><a href="combobox-element.md">ComboBox</a></p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="dropdown-element.md">DropDown</a></p></td>
</tr>
<tr class="odd">
<td align="left"><p><a href="flyoutanchor-element.md">FlyoutAnchor</a></p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="gallerybutton-element-group.md">GalleryButton</a></p></td>
</tr>
<tr class="odd">
<td align="left"><p><a href="label-element.md">Label</a></p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="mrusplitbutton-element.md">MRUSplitButton</a></p></td>
</tr>
<tr class="odd">
<td align="left"><p><a href="spinner-element.md">Spinner</a></p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="splitbutton-element.md">SplitButton</a></p></td>
</tr>
<tr class="odd">
<td align="left"><p><a href="textbox-element.md">TextBox</a></p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="togglebutton-element.md">ToggleButton</a></p></td>
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
<td align="left"><p><a href="group-element-ribbon.md">Group</a></p></td>
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
<td align="left"><p>Minimum: 1</p>
<p>Maximum: 1</p></td>
</tr>
</tbody>
</table>








