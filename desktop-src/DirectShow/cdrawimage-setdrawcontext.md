---
Description: 'The SetDrawContext method sets the device contexts used for drawing.'
ms.assetid: 'dd752970-99b3-42bb-95a5-8103cab276da'
title: 'CDrawImage.SetDrawContext method'
---

# CDrawImage.SetDrawContext method

The `SetDrawContext` method sets the device contexts used for drawing.

## Syntax


```C++
void SetDrawContext();
```



## Parameters

This method has no parameters.

## Return value

This method does not return a value.

## Remarks

This method retrieves the window and memory device contexts from the owning [**CBaseWindow**](cbasewindow.md) object. Call this method after the window is initialized, but before you begin drawing.

## Requirements



|                    |                                                                                                                                                                                            |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>Winutil.h (include Streams.h)</dt> </dl>                                                                                   |
| Library<br/> | <dl> <dt>Strmbase.lib (retail builds); </dt> <dt>Strmbasd.lib (debug builds)</dt> </dl> |



## See also

<dl> <dt>

[**CDrawImage Class**](cdrawimage.md)
</dt> </dl>

�

�



