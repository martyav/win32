---
Description: 'Windows GDI+ exposes a flat API that consists of about 600 functions, which are implemented in Gdiplus.dll and declared in Gdiplusflat.h.'
ms.assetid: 'def64d31-9a4b-4365-a618-b87735ce38f1'
title: Brush Functions
---

# Brush Functions

Windows GDI+ exposes a flat API that consists of about 600 functions, which are implemented in Gdiplus.dll and declared in Gdiplusflat.h. The functions in the GDI+ flat API are wrapped by a collection of about 40 C++ classes. It is recommended that you do not directly call the functions in the flat API. Whenever you make calls to GDI+, you should do so by calling the methods and functions provided by the C++ wrappers. Microsoft Product Support Services will not provide support for code that calls the flat API directly. For more information on using these wrapper methods, see [GDI+ Flat API](-gdiplus-flatapi-flat.md).

The following flat API functions are wrapped by the [**Brush**](-gdiplus-class-brush-class.md) C++ class.

## Brush Functions and Corresponding Wrapper Methods



| Flat function                                                                        | Wrapper method                                          | Description                                                                                                                                          |
|--------------------------------------------------------------------------------------|---------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------|
| GpStatus WINGDIPAPI GdipCloneBrush(GpBrush \*brush, GpBrush \*\*cloneBrush)          | [**Brush::Clone**](-gdiplus-class-brush-clone-.md)     | The [**Brush::Clone**](-gdiplus-class-brush-clone-.md) method creates a new [**Brush**](-gdiplus-class-brush-class.md) object based on this brush. |
| GpStatus WINGDIPAPI GdipDeleteBrush(GpBrush \*brush)                                 | virtual ~Brush()                                        | Cleans up resources used by a [**Brush**](-gdiplus-class-brush-class.md) object.                                                                    |
| GpStatus WINGDIPAPI GdipGetBrushType(GpBrush \*brush, GpBrushType \*type)<br/> | [**Brush::GetType**](-gdiplus-class-brush-gettype-.md) | The [**Brush::GetType**](-gdiplus-class-brush-gettype-.md) method gets the type of this brush.                                                      |



�

�

�



