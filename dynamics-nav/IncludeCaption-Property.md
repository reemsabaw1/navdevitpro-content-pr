---
title: "IncludeCaption Property"
description: "This topic describes the IncludeCaption property, which sets whether to include the caption of a field in the dataset of a report."
ms.custom: na
ms.date: 06/05/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: "dynamics-nav-2018"
ms.assetid: 5c155846-4dd6-49d0-a6f5-9af11f725d54
caps.latest.revision: 8
manager: edupont
---
# IncludeCaption Property
Sets whether to include the caption of a field in the dataset of a report.  

## Applies To  
 Columns on client report definition \(RDLC\) report datasets.  

## Property Value  
 **Yes** if the caption is included in the dataset; otherwise **No**. The default value is **No**.  

## Remarks  
 In Visual Studio Report Designer, if you want to use the Caption or CaptionML values of a field as a label on a report layout, then you must include the caption in the dataset. You design the dataset by using Report Dataset Designer. When you add table fields to the dataset with Report Dataset Designer, you can set the **IncludeCaption property** to **Yes** to specify that the caption for the field is also added to the dataset. If you do not include the caption in the dataset, then in a multilanguage application, you cannot use the multilanguage captions as labels in the report.  

 You can set the **IncludeCaption property** either in the **Properties** window of a data item or in the **IncludeCaption** column of Report Dataset Designer for a data item or a column. If you set the **IncludeCaption** column of a data item, then the **IncludeCaption property** is set to **Yes** for every child column of the data item.  

## See Also  
 [Caption Property](Caption-Property.md)   
 [How to: Create Labels for a Report](How-to--Create-Labels-for-a-Report.md)
