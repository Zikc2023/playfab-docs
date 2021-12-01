---
author: tomcoMSFT
title: "PFLobbyMembershipLock"
description: "Values representing the state of the lobby's membership lock."
ms.author: tomco
ms.topic: reference
ms.prod: playfab
ms.date: 10/27/2021
---

# PFLobbyMembershipLock  

Values representing the state of the lobby's membership lock.    

## Syntax  
  
```cpp
enum class PFLobbyMembershipLock  : uint32_t  
{  
    Unlocked = 0,  
    Locked = 1,  
}  
```  
  
## Constants  
  
| Constant | Description |
| --- | --- |
| Unlocked | Lobby membership is unlocked. New members will not be prevented from joining. |  
| Locked | Lobby membership is locked. New members will be prevented from joining. |  
  
  
## Requirements  
  
**Header:** PFLobby.h
  
## See also  
[PFLobby members](../pflobby_members.md)  

  
  