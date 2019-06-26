---
title: Update currencies | Microsoft Docs
description: Updates a currency object in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen

ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 04/01/2019
ms.author: solsen
---

# Update currencies
Update the properties of a currency object for [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].

## HTTP request
```
PATCH /businesscentral/companies({id})/currencies({id})
```

## Request headers

|Header       |Value                    |
|-------------|-------------------------|
|Authorization|Bearer {token}. Required.|
|Content-Type |application/json         |
|If-Match     |Required. When this request header is included and the eTag provided does not match the current tag on the **currencies**, the **currencies** will not be updated. |

## Request body
In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.

## Response
If successful, this method returns a ```200 OK``` response code and an updated **currencies** object in the response body.

## Example

**Request**

Here is an example of the request.
```json
PATCH https://api.businesscentral.dynamics.com/v1.0/api/v1.0/companies({id})/currencies({id})
Content-type: application/json

{
    "displayName": "United States Dollar"
}
```

**Response**

Here is an example of the response. 

> [!NOTE]  
>   The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "code": "US",
  "displayName": "United States Dollar",
  "symbol": "$",
  "amountDecimalPlaces": "2:2",
  "amountRoundingPrecision": 0.01,
  "lastModifiedDateTime": "2017-03-22T21:12:18.793Z"
}
```


## See also



[Error Codes](../dynamics_error_codes.md)  
[Currencies](../resources/dynamics_currencies.md)  
[Post Currencies](dynamics_create_currencies.md)  
[Get Currencies](dynamics_currencies_get.md)  
[Delete Currencies](dynamics_currencies_delete.md)  