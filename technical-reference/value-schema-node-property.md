﻿---
title: Value (Schema Node Property)
TOCTitle: Value (Schema Node Property)
ms:assetid: 77fed485-dcd7-437b-b0e3-807b75b2df9f
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Aa560901(v=BTS.80)
ms:contentKeyID: 51529053
ms.date: 08/30/2017
mtps_version: v=BTS.80
---

# Value (Schema Node Property)

 

Use the **Value** property to specify a value for the selected node that is used differently, depending on whether the value is provided in the source schema or the destination schema. The value is used as follows:

  - In source schemas, the value of the **Value** property is used as the value of the elements or attributes in a generated instance message that corresponds to the selected node. This value is used when generating an instance message for the source schema for the TestMap operation.

  - In destination schemas, the value of the **Value** property specifies a constant value for the elements or attributes in an output instance message that corresponds to the selected node. Any value you provide for this property is used in the XSLT generated by BizTalk Mapper. Set this property if you want the elements or attributes associated with the selected node to be present in output instance messages, and if you want those elements or attributes to have the constant value you provide by using this property rather than a value copied from an input instance message.

## Category

General

## Allowed Values

Any string that conforms to the data type of the node, although BizTalk Mapper does not enforce the conformance.

## Default Value

None.

## Remarks

When you specify a value for the **Value** property of a node in the destination schema, you cannot connect a link to that node.

## See Also

[Schema Node Properties in BizTalk Mapper](schema-node-properties-in-biztalk-mapper.md)
