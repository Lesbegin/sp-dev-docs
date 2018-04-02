---


manager: soliver
ms.date: 3/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- dsQueryResponse XML
ms.assetid: e2d1bbbe-c920-41d0-994a-f06a122ba3fd
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
<td align="left"># Row (dsQueryResponse)</td>
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

Represents a row of data from the list. The fields and metadata
properties of the list item that the row contains are represented by
attributes of the **Row** element. Some fields,
depending on their data type, may be represented by additional
attributes that present the field's value in a different format.

<span codelanguage="other"></span>
<table>
<colgroup>
<col width="100%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><pre><code><Row
  Attachments="Integer"
  ContentTypeId="GUID"
  File_x0020_Type="String"
  FileLeafRef="String"
  FileLeafRef.Name="String"
  FileLeafRef.Suffix="String"
  FSObjType="Integer"
  HTML_x0020_File_x0020_Type.File_x0020_Type.mapall="String"
  HTML_x0020_File_x0020_Type.File_x0020_Type.mapcon="String"
  HTML_x0020_File_x0020_Type.File_x0020_Type.mapico="String"
  ID="Integer"
  PermMask="Hex"
  some_field="type appropriate to the field"
  some_booleanField.Value="Integer"
  some_date_time_field.ifnew="Integer"
  some_date_time_field.="unlocalized DateTime"
  some_date_time_field.DateOnly="date"
  some_date_time_field.TimeOnly="time"
  some_date_time_field.ISO8601="ISO8601 compliant DateTime"
  some_date_time_field.MonthDayOnly="month and day"
  some_date_time_field.MonthYearOnly="month and year"
  some_user_field="String"
  some_user_field.id="Integer"
  some_user_field.title="String"
  some_user_field.span="String"
  some_url_field.desc="String"
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
<td align="left"><p>**Attachments**</p></td>
<td align="left"><p>Required. **1</span> if the list item has one or more attachments; otherwise, **0**.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**ContentTypeId**</p></td>
<td align="left"><p>Required. The GUID of the content type of the list item in the format Ox<span class="placeholder">GUID_without_hyphens</span>.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**File_x0020_Type**</p></td>
<td align="left"><p>Required, but ignored if the list is not a document library. The type of files in a document library. Empty string when the list is not a document library.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**FileLeafRef**</p></td>
<td align="left"><p>Required, but ignored if the list is not a document library. The server-relative URL of the document. This is the folder name, followed by "_.", followed by the file name. An example is QuarterlySummaries_.Quarter1.docx. This attribute value is the concatenation of the values of the **FileLeafRef.Name</span> attribute and the **FileLeafRef.Suffix** attribute with a "." separator character.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**FileLeafRef.Name**</p></td>
<td align="left"><p>Required, but ignored if the list is not a document library. The name of the folder that contains the document, followed by an underscore character; for example, QuarterlySummaries_.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**FileLeafRef.Suffix**</p></td>
<td align="left"><p>Required, but ignored if the list is not a document library. The name of the document file; for example, Quarter1.docx.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**FSObjType**</p></td>
<td align="left"><p>Required. **1</span> if the list item is a folder; otherwise, **0**.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**HTML_x0020_File_x0020_Type.File_x0020_Type.mapall**</p></td>
<td align="left"><p>Optional. The value that is returned by a call of the **MapToAll</span> function during the XSLT transformation. For more information, see <span sdata="link"><a href="maptoall-element-view.md">MapToAll Element (View)</a>** and <a href="http://msdn.microsoft.com/en-us/library/dd583143(office.11).aspx">SharePoint Data View Web Part Extension Functions in the ddwrt Namespace</a>.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**HTML_x0020_File_x0020_Type.File_x0020_Type.mapcon**</p></td>
<td align="left"><p>Optional. The value that is returned by a call of the **MapToControl</span> function during the XSLT transformation. For more information, see <span sdata="cer" target="M:Microsoft.SharePoint.Utilities.SPUtility.MapToControl(Microsoft.SharePoint.SPWeb,System.String,System.String)"><span class="nolink">MapToControl(SPWeb, String, String)</span></span>, <span sdata="link"><a href="maptocontrol-element-view.md">MapToControl Element (View)</a>**, and <a href="http://msdn.microsoft.com/en-us/library/dd583143(office.11).aspx">SharePoint Data View Web Part Extension Functions in the ddwrt Namespace</a>.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**HTML_x0020_File_x0020_Type.File_x0020_Type.mapico**</p></td>
<td align="left"><p>Optional. The value that is returned by a call of the **MapToIcon</span> function during the XSLT transformation. For more information, see <span sdata="cer" target="Overload:Microsoft.SharePoint.Utilities.SPUtility.Icon"><strong>Icon()</strong></span>, <span sdata="link"><a href="maptoicon-element-view.md">MapToIcon Element (View)</a>**, and <a href="http://msdn.microsoft.com/en-us/library/dd583143(office.11).aspx">SharePoint Data View Web Part Extension Functions in the ddwrt Namespace</a>.</p></td>
</tr>
<tr class="odd">
<td align="left"><p>**ID**</p></td>
<td align="left"><p>Required. The ID of the list item.</p></td>
</tr>
<tr class="even">
<td align="left"><p>**PermMask**</p></td>
<td align="left"><p>The permissions mask for the list item.</p></td>
</tr>
<tr class="odd">
<td align="left"><p><span class="placeholder">some_field</span></p></td>
<td align="left"><p>Required for every non-hidden field in the list item. For each such field, there is an attribute that has the same name as the internal name of the field.</p></td>
</tr>
<tr class="even">
<td align="left"><p><span class="placeholder">some_field</span>.</p></td>
<td align="left"><p>Optional. The currency, number, and lookup field types in SharePoint Foundation may have a low-level formatting even before any HTML formatting is applied. For example, a negative currency value is enclosed in parentheses. The attribute of each such field is immediately followed by another attribute that has the same name, to which a "." character is appended. This attribute provides the field value as raw unformatted data. For example, a negative currency value is proceeded by a minus sign ("-") and is not in parentheses.</p></td>
</tr>
<tr class="odd">
<td align="left"><p><span class="placeholder">some_booleanField</span>**.Value**</p></td>
<td align="left"><p>Optional. Every **Boolean</span> attribute in the list item is followed by another attribute that has the same name, to which ".Value" is appended. This attribute gives the raw unlocalized form of the field value (1 or 0), whereas the main attribute for the **Boolean** field gives the value relativized to the website's locale.</p></td>
</tr>
<tr class="even">
<td align="left"><p><span class="placeholder">some_date_time_field</span>**.ifnew**</p></td>
<td align="left"><p>Optional. **1</span> if the date time value is recent enough to define the list item as new; otherwise, **0</span>. This attribute appears only if the <span class="placeholder">some_date_time_field** is "Created_x0020_Date".</p></td>
</tr>
<tr class="odd">
<td align="left"><p><span class="placeholder">some_date_time_field</span>.</p></td>
<td align="left"><p>Optional. If there is an attribute for a datetime field whose value is localized, there is also an attribute that has the same name, to which a "." character is appended. This attribute provides the raw value of a datetime field as stored in the content database in ISO8601 format.</p></td>
</tr>
<tr class="even">
<td align="left"><p><span class="placeholder">some_date_time_field</span>**.DateOnly**</p></td>
<td align="left"><p>Optional. The value of a DateTime field with only the date. Used only on blog-related lists.</p></td>
</tr>
<tr class="odd">
<td align="left"><p><span class="placeholder">some_date_time_field</span>**.TimeOnly**</p></td>
<td align="left"><p>Optional. The value of a DateTime field with only the time of day. Used only on blog-related lists.</p></td>
</tr>
<tr class="even">
<td align="left"><p><span class="placeholder">some_date_time_field</span>**.ISO8601**</p></td>
<td align="left"><p>Optional. The value of a DateTime field formatted in compliance with ISO8601. Used only on blog-related lists.</p></td>
</tr>
<tr class="odd">
<td align="left"><p><span class="placeholder">some_date_time_field</span>**.MonthDayOnly**</p></td>
<td align="left"><p>Optional. The value of a DateTime field with only the month and day-of-month. Used only on blog-related lists.</p></td>
</tr>
<tr class="even">
<td align="left"><p><span class="placeholder">some_date_time_field</span>**.MonthYearOnly**</p></td>
<td align="left"><p>Optional. The value of a DateTime field with only the month and year. Used only on blog-related lists.</p></td>
</tr>
<tr class="odd">
<td align="left"><p><span class="placeholder">some_user_field</span>**.id**</p></td>
<td align="left"><p>Optional. If any attribute represents a User type field, there is another attribute that has the same name, to which ".id" is appended. This is the site-relative ID number of the user.</p></td>
</tr>
<tr class="even">
<td align="left"><p><span class="placeholder">some_user_field</span>**.title**</p></td>
<td align="left"><p>Optional. If any attribute represents a User type field, there is another attribute that has the same name, to which ".title" is appended. This is the name of the user, for example "Michiyo Sato". Note that the value of the main attribute, <span class="placeholder">some_user_field</span>, is the HTML **span</span> markup for the user, including, for example, presence information. The following is an example. This markup is used to render the field when the <span sdata="cer" target="F:Microsoft.SharePoint.SPViewFlags.FreeForm"><span class="nolink">FreeForm</span></span> flag of the <span sdata="cer" target="P:Microsoft.SharePoint.WebPartPages.ListViewWebPart.ViewFlags"><span class="nolink">ListViewWebPart.ViewFlags</span></span> property is not set; otherwise the value of the <span class="placeholder">some_user_field</span>**.span** attribute is used.</p>
<div class="code">
<span codelanguage="xmlLang"></span>
XML 
<span class="copyCode" onclick="CopyCode(this)" onkeypress="CopyCode_CheckKey(this, event)" onmouseover="ChangeCopyCodeIcon(this)" onmouseout="ChangeCopyCodeIcon(this)" tabindex="0"><img src=".." title="Copy code" alt="Copy code" />Copy code</span>
<pre><code><span class="ms-imnSpan">
<a href=&#39;javascript:;&#39;
  onclick=&#39;IMNImageOnClick(event);return false;&#39;
  class=&#39;ms-imnlink&#39;>
<img name=&#39;imnmark&#39; 
  class=&#39;ms-imnImg&#39; title=&#39;&#39; border=&#39;0&#39;
  height=&#39;12&#39; width=&#39;12&#39;
  src=&#39;/_layouts/images/blank.gif&#39; 
  alt=&#39;No presence information&#39; 
  sip=&#39;MichiyoS@Contoso.com&#39; 
  id=&#39;imn_1,type=smtp&#39;/>
</a>
<a onclick="GoToLink(this);return false;"
  href="/sites/Contoso/_layouts/userdisp.aspx?ID=1">Michiyo Sato</a>
</span></code></pre>
</div>
<p></p></td>
</tr>
<tr class="odd">
<td align="left"><p><span class="placeholder">some_user_field</span>**.span**</p></td>
<td align="left"><p>Optional. If any attribute represents a User type field, there is another attribute that has the same name, to which ".span" is appended. This is a plainer version of the HTML markup for the user. The following is an example. This markup is used to render the field when the <span sdata="cer" target="F:Microsoft.SharePoint.SPViewFlags.FreeForm"><span class="nolink">FreeForm</span></span> flag of the <span sdata="cer" target="P:Microsoft.SharePoint.WebPartPages.ListViewWebPart.ViewFlags"><span class="nolink">ListViewWebPart.ViewFlags</span></span> property is set; otherwise the value of the <span class="placeholder">some_user_field</span>**.title** attribute is used.</p>
<div class="code">
<span codelanguage="xmlLang"></span>
XML 
<span class="copyCode" onclick="CopyCode(this)" onkeypress="CopyCode_CheckKey(this, event)" onmouseover="ChangeCopyCodeIcon(this)" onmouseout="ChangeCopyCodeIcon(this)" tabindex="0"><img src=".." title="Copy code" alt="Copy code" />Copy code</span>
<pre><code><nobr><span>
<a onclick="GoToLink(this);return false;"
  href="/sites/Contoso/_layouts/userdisp.aspx?ID=1">Michiyo Sato</a>
<img border="0" height="1" width="3"
  src="/_layouts/images/blank.gif"/>
<a href=&#39;javascript:;&#39;
  onclick=&#39;IMNImageOnClick(event);return false;&#39;
  class=&#39;ms-imnlink&#39;>
<img name=&#39;imnmark&#39; class=&#39;ms-imnImg&#39;
  title=&#39;&#39; border=&#39;0&#39; 
  height=&#39;12&#39; width=&#39;12&#39; 
  src=&#39;/_layouts/images/blank.gif&#39; 
  alt=&#39;No presence information&#39; 
  sip=&#39;MichiyoS@Contoso.com&#39; 
  id=&#39;imn_2,type=smtp&#39;/></a>
</span></nobr></code></pre>
</div></td>
</tr>
<tr class="even">
<td align="left"><p><span class="placeholder">some_url_field</span>**.desc**</p></td>
<td align="left"><p>Optional. If any attribute represents a URL field, there is another attribute that has the same name, to which ".desc" is appended. This provides a description of the URL.</p></td>
</tr>
</tbody>
</table>


---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

None


----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<table>
<colgroup>
<col width="100%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><p><a href="rows-dsqueryresponse.md">Rows</a></p></td>
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
<p>Maximum: the value of the **RowLimit</span> attribute of the parent **dsQueryResponse** element.</p></td>
</tr>
</tbody>
</table>


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

For an example, see [Examples of Input and Result Node Trees in XSLT
Transformations](http://msdn.microsoft.com/library/cbe88144-25ac-4cd2-8f2a-50e8c271c6ae(Office.15).aspx).








