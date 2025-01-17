---
title: "GETLASTERRORCODE Function"
description: Describes the GETLASTERRORCODE function and provides syntax, return value, and an example.
ms.custom: na
ms.date: 06/05/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: "dynamics-nav-2018"
ms.assetid: 7df300fa-21f6-4e5e-8a24-a27674e530c6
caps.latest.revision: 8
manager: edupont
---
# GETLASTERRORCODE Function
Gets the classification of the last error that occurred.  
  
## Syntax  
  
```  
  
String := GETLASTERRORCODE  
```  
  
## Property Value/Return Value  
 Type: Text  
  
 A string that contains the error code of the last error. The error code is a classification of the error.  
  
 If no error has occurred, then the function returns an empty string.  
  
## Remarks  
 You use the GETLASTERRORCODE function to identify the type of the last error that occurred. You use the [GETLASTERRORTEXT Function](GETLASTERRORTEXT-Function.md) to get the details of the last error.  
  
 The result of the GETLASTERRORCODE function is not translated into the local language. The result of the GETLASTERRORTEXT function is translated into the local language.  
  
## Example  
 This example opens a file and then causes an error to occur by trying to open the file again. If the code for the error that occurred is not the expected error code, then an error message is displayed.  
  
 This example requires that you create the following text constant and variables.  
  
|Text constant|ENU value|  
|-------------------|---------------|  
|Text001|The error code is not valid. Expected: %1. Actual: %2. Error message: %3|  
  
|Variable name|DataType|Length|  
|-------------------|--------------|------------|  
|ErrorCode|Text|1024|  
|ExpectedErrorCode|Text|1024|  
|FileObj1|File|Not applicable|  
|FileObj2|File|Not applicable|  
  
```  
ExpectedErrorCode := 'StreamIO';  
FileObj1.CREATETEMPFILE;  
ASSERTERROR FileObj2.CREATE(FileObj1.NAME);  
ErrorCode := GETLASTERRORCODE;  
IF ErrorCode <> ExpectedErrorCode THEN  
  ERROR(Text001, ExpectedErrorCode, ErrorCode, GETLASTERRORTEXT);  
  
```  
  
## See Also  
 <!-- [Error Handling](Error-Handling.md) -->