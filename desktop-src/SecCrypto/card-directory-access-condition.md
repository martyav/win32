---
Description: Specifies access control permissions for a directory on a smart card.
ms.assetid: 361d9fa0-286e-4d2c-8452-3b5f48e77779
title: CARD\_DIRECTORY\_ACCESS\_CONDITION enumeration
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: enumeration
ms.date: 05/31/2018
---

# CARD\_DIRECTORY\_ACCESS\_CONDITION enumeration

The **CARD\_DIRECTORY\_ACCESS\_CONDITION** enumeration specifies access control permissions for a directory on a [*smart card*](https://www.bing.com/search?q=*smart card*).

## Syntax


```C++
typedef enum  { 
  InvalidAc               = 0,
  UserCreateDeleteDirAc   = 1,
  AdminCreateDeleteDirAc  = 2
} CARD_DIRECTORY_ACCESS_CONDITION;
```



## Constants

<dl> <dt>

<span id="InvalidAc"></span><span id="invalidac"></span><span id="INVALIDAC"></span>**InvalidAc**
</dt> <dd>

This value is not valid.

</dd> <dt>

<span id="UserCreateDeleteDirAc"></span><span id="usercreatedeletedirac"></span><span id="USERCREATEDELETEDIRAC"></span>**UserCreateDeleteDirAc**
</dt> <dd>

Specific users can read, write, and delete the directory.

</dd> <dt>

<span id="AdminCreateDeleteDirAc"></span><span id="admincreatedeletedirac"></span><span id="ADMINCREATEDELETEDIRAC"></span>**AdminCreateDeleteDirAc**
</dt> <dd>

Administrators can read, write, and delete the directory.

</dd> </dl>

## Requirements



|                                     |                                                                                      |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows XP, Windows XP \[desktop apps only\]<br/>                              |
| Minimum supported server<br/> | Windows Server 2003, Windows Server 2003 \[desktop apps only\]<br/>            |
| Header<br/>                   | <dl> <dt>Cardmod.h</dt> </dl> |



## See also

<dl> <dt>

[Microsoft Base Smart Card Cryptographic Service Provider](https://msdn.microsoft.com/windows/desktop/8d71e365-c581-4ec8-977b-0725a8c7d9ad)
</dt> <dt>

[**CardCreateDirectory**](https://msdn.microsoft.com/windows/desktop/e5f067e1-fdd7-4a83-993e-ffbca22c1a38)
</dt> <dt>

[**CardDeleteDirectory**](https://msdn.microsoft.com/windows/desktop/c5a4e77d-fa0e-4808-8f62-e099aa3b3ecf)
</dt> </dl>

 

 



