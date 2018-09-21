﻿---
title: JET_OPENTEMPORARYTABLE properties (Microsoft.Isam.Esent.Interop.Vista)
TOCTitle: JET_OPENTEMPORARYTABLE properties
ms:assetid: Properties.T:Microsoft.Isam.Esent.Interop.Vista.JET_OPENTEMPORARYTABLE
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/microsoft.isam.esent.interop.vista.jet_opentemporarytable_properties(v=EXCHG.10)
ms:contentKeyID: 55104127
ms.date: 07/30/2014
mtps_version: v=EXCHG.10
---

# JET\_OPENTEMPORARYTABLE properties

Include protected members  
Include inherited members  

The [JET\_OPENTEMPORARYTABLE](dn351217\(v=exchg.10\).md) type exposes the following members.

## Properties

<table>
<thead>
<tr class="header">
<th> </th>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><img src="images/Dn292128.pubproperty(EXCHG.10).gif" title="Public property" alt="Public property" /></td>
<td><a href="dn335290(v=exchg.10).md">cbKeyMost</a></td>
<td>Gets or sets the maximum size for a key representing a given row. The maximum key size may be set to control how keys are truncated. Key truncation is important because it can affect when rows are considered to be distinct. If this parameter is set to 0 or 255 then the maximum key size and its semantics will remain identical to the maximum key size supported by Windows Server 2003. This parameter may also be set to a larger value as a function of the database page size for the instance <a href="hh596135(v=exchg.10).md">DatabasePageSize</a>. See <a href="dn335292(v=exchg.10).md">KeyMost</a> for more information.</td>
</tr>
<tr class="even">
<td><img src="images/Dn292128.pubproperty(EXCHG.10).gif" title="Public property" alt="Public property" /></td>
<td><a href="dn351219(v=exchg.10).md">cbVarSegMac</a></td>
<td>Gets or sets maximum amount of data that will be used from any variable lengthcolumn to construct a key for a given row. This parameter may be used to control the amount of key space consumed by any given key column. This limit is in bytes. If this parameter is zero or is the same as the <a href="dn335290(v=exchg.10).md">cbKeyMost</a> property then no limit is in effect.</td>
</tr>
<tr class="odd">
<td><img src="images/Dn292128.pubproperty(EXCHG.10).gif" title="Public property" alt="Public property" /></td>
<td><a href="dn335287(v=exchg.10).md">ccolumn</a></td>
<td>Gets or sets the number of columns in <a href="dn351228(v=exchg.10).md">prgcolumndef</a>.</td>
</tr>
<tr class="even">
<td><img src="images/Dn292128.pubproperty(EXCHG.10).gif" title="Public property" alt="Public property" /></td>
<td><a href="dn351232(v=exchg.10).md">grbit</a></td>
<td>Gets or sets options for the temp table.</td>
</tr>
<tr class="odd">
<td><img src="images/Dn292128.pubproperty(EXCHG.10).gif" title="Public property" alt="Public property" /></td>
<td><a href="dn335288(v=exchg.10).md">pidxunicode</a></td>
<td>Gets or sets the locale ID and normalization flags to use to compare any Unicode key column data in the temporary table. When this parameter is null, then the default LCID will be used to compare any Unicode key columns in the temporary table. The default LCID is the U.S. English locale. When this parameter is null, then the default normalization flags will be used to compare any Unicode key column data in the temp table. The default normalization flags are: NORM_IGNORECASE, NORM_IGNOREKANATYPE, and NORM_IGNOREWIDTH.</td>
</tr>
<tr class="even">
<td><img src="images/Dn292128.pubproperty(EXCHG.10).gif" title="Public property" alt="Public property" /></td>
<td><a href="dn351228(v=exchg.10).md">prgcolumndef</a></td>
<td>Gets or sets the column definitions for the columns created in the temporary table.</td>
</tr>
<tr class="odd">
<td><img src="images/Dn292128.pubproperty(EXCHG.10).gif" title="Public property" alt="Public property" /></td>
<td><a href="dn351233(v=exchg.10).md">prgcolumnid</a></td>
<td>Gets or sets the output buffer that receives the array of column IDs generated during the creation of the temporary table. The column IDs in this array will exactly correspond to the input array of column definitions. As a result, the size of this buffer must correspond to the size of <a href="dn351228(v=exchg.10).md">prgcolumndef</a>.</td>
</tr>
<tr class="even">
<td><img src="images/Dn292128.pubproperty(EXCHG.10).gif" title="Public property" alt="Public property" /></td>
<td><a href="dn335293(v=exchg.10).md">tableid</a></td>
<td>Gets the table handle for the temporary table created as a result of a successful call to JetOpenTemporaryTable.</td>
</tr>
</tbody>
</table>


Top

## See also

#### Reference

[JET\_OPENTEMPORARYTABLE class](dn351217\(v=exchg.10\).md)

[Microsoft.Isam.Esent.Interop.Vista namespace](hh558039\(v=exchg.10\).md)
