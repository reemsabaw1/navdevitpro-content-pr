---
title: "NORMALDATE Function (Date)"
description: NORMALDATE Function (Date)
ms.custom: na
ms.date: 06/05/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: "dynamics-nav-2018"
ms.assetid: f3c48dbf-0f63-4384-881b-a849b004ca58
caps.latest.revision: 13
manager: edupont
---
# NORMALDATE Function (Date)
Gets the regular date \(instead of the closing date\) for the argument Date.  
  
## Syntax  
  
```  
  
NormalDate := NORMALDATE(Date)  
```  
  
#### Parameters  
 *Date*  
 Type: Date  
  
 The input date. You can enter a closing date or a normal date. A run-time error occurs if the value of *Date* is set to the undefined date \(0D\).  
  
## Property Value/Return Value  
 Type: Date  
  
 The resulting date. If the input date is either a normal date or a closing date, then the return value is a normal date.  
  
## Remarks  
 All dates have a corresponding closing date. A closing date is a period of time that follows the given date but comes before the next date. Closing dates are sorted immediately after the corresponding date and before the next date.  
  
 xxxxxxD: regular date  
  
 xxxxxxC: closing date  
  
## Example 1 
 The input date is a regular date. This code example requires that you create the following variables and text constants in the **C/AL Globals** window.  
  
|Variable name|DataType|  
|-------------------|--------------|  
|InputDate|Date|  
|OutputDate|Date|  
  
|Text constant name|ENU value|  
|------------------------|---------------|  
|Text000|The normal date for %1 is %2.|  
  
```  
InputDate := 040414D;  
OutputDate := NORMALDATE(InputDate);  
MESSAGE(Text000, InputDate, OutputDate);  
```  
  
 On a computer that has the regional format set to English \(United States\), the message window displays the following:  
  
 **The normal date for 04/04/14 is 04/04/14.**  
  
## Example 2 
 The input date is a closing date. This code example requires that you create the following variables and text constants in the **C/AL Globals** window.  
  
|Variable name|DataType|  
|-------------------|--------------|  
|InputDate|Date|  
|OutputDate|Date|  
  
|Text constant name|ENU value|  
|------------------------|---------------|  
|Text001|The normal date for %1 is %2.|  
  
```  
InputDate := CLOSINGDATE(040414C);  
OutputDate := NORMALDATE(InputDate);  
MESSAGE(Text001, InputDate, OutputDate);  
```  
  
 On a computer that has the regional format set to English \(United States\), the message window displays the following:  
  
 **The normal date for C04/04/14 is 04/04/14.**  
  
## See Also  
 [Date and Time Functions](Date-and-Time-Functions.md)