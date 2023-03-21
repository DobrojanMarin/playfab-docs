---
author: jasonsandlin
title: "PFInventoryAddInventoryItemsResponse"
description: "PFInventoryAddInventoryItemsResponse data model."
ms.author: jasonsa
ms.topic: reference
ms.service: playfab
ms.date: 03/09/2023
---

# PFInventoryAddInventoryItemsResponse  

PFInventoryAddInventoryItemsResponse data model.  

## Syntax  
  
```cpp
typedef struct PFInventoryAddInventoryItemsResponse {  
    const char* eTag;  
    const char* idempotencyId;  
    const char* const* transactionIds;  
    uint32_t transactionIdsCount;  
} PFInventoryAddInventoryItemsResponse;  
```
  
### Members  
  
**`eTag`** &nbsp; const char*  
*is null-terminated*  
  
(Optional) ETags are used for concurrency checking when updating resources.
  
**`idempotencyId`** &nbsp; const char*  
*is null-terminated*  
  
(Optional) The idempotency id used in the request.
  
**`transactionIds`** &nbsp; const char* const*  
*array of size `transactionIdsCount`*  
  
(Optional) The ids of transactions that occurred as a result of the request.
  
**`transactionIdsCount`** &nbsp; uint32_t  
  
Count of transactionIds
  
  
## Requirements  
  
**Header:** PFInventoryTypes.h
  
## See also  
[PFInventoryTypes members](../pfinventorytypes_members.md)  

  
  