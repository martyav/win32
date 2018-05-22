---
Description: 'The AddTail method appends another list to the end of this list.'
ms.assetid: '996523cd-d9ba-406a-afdf-494d328dc9dd'
title: 'CBaseList.AddTail method'
---

# CBaseList.AddTail method

The `AddTail` method appends another list to the end of this list.

## Syntax


```C++
BOOL AddTail(
  �CBaseList *pList
);
```



## Parameters

<dl> <dt>

*pList* 
</dt> <dd>

Pointer to the list to append.

</dd> </dl>

## Return value

Returns **TRUE** if successful, or **FALSE** otherwise.

## Remarks

If the method fails, some items may have been added to the list.

## Requirements



|                    |                                                                                                                                                                                            |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>Wxlist.h (include Streams.h)</dt> </dl>                                                                                    |
| Library<br/> | <dl> <dt>Strmbase.lib (retail builds); </dt> <dt>Strmbasd.lib (debug builds)</dt> </dl> |



## See also

<dl> <dt>

[**CBaseList Class**](cbaselist.md)
</dt> </dl>

�

�



