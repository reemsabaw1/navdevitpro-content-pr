---
title: "DataItemLinkReference Property"
description: Describes the DataItemLinkReference property and provides additional remarks.
ms.custom: na
ms.date: 06/05/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: "dynamics-nav-2018"
ms.assetid: fc18f455-197e-423f-897d-1818eda47bd9
caps.latest.revision: 6
manager: edupont
---
# DataItemLinkReference Property
Sets the parent data item to which a child \(indented\) data item is linked. After you specify the **DataItemLinkReference** value, use the [DataItemLink Property \(Reports\)](DataItemLink-Property--Reports-.md) to specify a field from each data item on which to base the link.  
  
## Applies To  
  
-   Data items  
  
-   Reports  
  
## Remarks  
 The default value is the name of the last preceding data item in the report with lower indentation. You can set **DataItemLinkReference** and **DataItemLink** properties for a data item that is not a child of another data item, however, this will not have any effect.