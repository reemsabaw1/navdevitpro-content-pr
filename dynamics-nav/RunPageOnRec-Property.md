---
title: "RunPageOnRec Property"
description: Describes the RunPageOnRec property and provides property values and additional remarks.
ms.custom: na
ms.date: 06/05/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: "dynamics-nav-2018"
ms.assetid: b453e896-1467-4123-ab2e-1bbce78ed7bd
caps.latest.revision: 8
---

# RunPageOnRec Property
Sets the same record on the page you launch from this control as is already displayed on the current page.  
  
## Applies To  
  
- Page actions  
  
## Property Value  
**Yes** if the current record on the page that you will launch from this control is displayed; otherwise, **No**. The default is **No**.  
  
## Remarks  
For example, suppose the current page is the sales order and you are providing a way to see the sales statistics for the current customer. You would select **RunObject** in the **PushAction** property and then use the [RunObject Property](RunObject-Property.md) to run the sales statistics page. And then in the **RunPageOnRec** property you could select **Yes** to display the same record on both pages.  
  
## See Also  
[RunPageView Property](RunPageView-Property.md)   
[RunPageLink Property](RunPageLink-Property.md)