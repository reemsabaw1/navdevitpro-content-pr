---
title: "COUNT Function (MediaSet)"
description: "Describes the COUNT function (MediaSet), which counts the number of media objects that are included in the MediaSet of a record."
ms.custom: na
ms.date: 06/05/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.author: jswymer
ms.prod: "dynamics-nav-2018"
---
# COUNT Function (MediaSet)
Counts the number of media objects that are included in the MediaSet of a record.

## Syntax  

```  

Number := Record.MediaSetField.COUNT  
```  

#### Parameters  
 *Record*  
 Type: Record  

 Specifies the record.  

 *MediaSetField*  
 Type: MediaSet  

 Specifies the MediaSet data type field for the record.  

## Property Value/Return Value  
 Type: Integer  

 Specifies the number of media objects that are associated with the MediaSet field of the record.  

## Example  
 This example counts the number of media objects that are available for item No. 1000 in table **27 Item** of the  [!INCLUDE[demolonglight_md](includes/demolonglight_md.md)]. In this example, the field in the **Item** table that is used for the MediaSet data type is **Picture**.  

This code requires you to create the following variables.

|Variable name|DataType|Subtype|  
|-------------------|--------------|-------------|  
|itemRec|Record|Item|  
|count|Integer||  

 This code requires you to create the following text constant.  

|  Text constant  |  ConstValue  |  
|-----------------|--------------|  
|Text000|The number of media files: %1|  

```  
itemRec.GET('1000');  
    count := (itemRec.Picture.COUNT);  
    MESSAGE(Text000,count);  
```  

## See Also  
[Working With Media on Records](Working-With-Media-on-Records.md)  
[MediaSet Data Type](MediaSet-Data-Type.md)  
