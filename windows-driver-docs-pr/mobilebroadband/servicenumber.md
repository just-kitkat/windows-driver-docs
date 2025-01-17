---
title: ServiceNumber
description: ServiceNumber
ms.date: 04/20/2017
---

# ServiceNumber

[!include[MBAE deprecation warning](../includes/mbae-deprecation-warning.md)]

The ServiceNumber element specifies the unique self-generated GUID that represents the mobile operator. This GUID must be present and is checked when account provisioning metadata is applied to a PC to ensure a match with the GUID value declared in the Carrier ID identified in that file. The account provisioning metadata is generated by the mobile broadband app or an operator website. Account provisioning metadata is described in [Account provisioning](account-provisioning.md).

## Usage


``` syntax
<ServiceNumber>
  text
</ServiceNumber>
```

## Attributes


There are no attributes.

## Text value


A string of [GUIDType](guidtype-serviceinfo.md).

## Child elements


There are no child elements.

## Parent elements


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Element</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><a href="serviceinfo.md" data-raw-source="[ServiceInfo](serviceinfo.md)">ServiceInfo</a></p></td>
<td><p>The <a href="serviceinfo.md" data-raw-source="[ServiceInfo](serviceinfo.md)">ServiceInfo</a> element is the parent element of the <a href="serviceinfo-xml-schema.md" data-raw-source="[ServiceInfo XML schema](serviceinfo-xml-schema.md)">ServiceInfo XML schema</a>.</p></td>
</tr>
</tbody>
</table>

 

## XSD


``` syntax
<xs:element name="ServiceNumber" type ="tns:ServiceNumberType" />

<xs:simpleType name="ServiceNumberType">
  <xs:union memberTypes="tns:GUIDType xs:string" />
</xs:simpleType>
```

## Remarks


The ServiceNumber element is required.

 

 





