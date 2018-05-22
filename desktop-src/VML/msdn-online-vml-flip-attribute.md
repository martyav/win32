---
title: VML Flip Attribute
description: VML Flip Attribute
ms.assetid: '0d3d4c54-e769-4f6b-a9f5-6e48125a7215'
---

# VML Flip Attribute

This topic describes VML, a feature that is deprecated as of Windows Internet Explorer 9. Webpages and applications that rely on VML should be [migrated to SVG](http://go.microsoft.com/fwlink/p/?LinkID=236964) or other widely supported standards.

> [!Note]  
> As of December 2011, this topic has been archived. As a result, it is no longer actively maintained. For more information, see [Archived Content](https://msdn.microsoft.com/library/hh772377). For information, recommendations, and guidance regarding the current version of Windows Internet Explorer, see [Internet Explorer Developer Center](http://go.microsoft.com/fwlink/p/?linkid=204313).

 

Switches the orientation of a shape. Read/write. **String**.

**Applies To**

[Shape](shape-element--vml.md)

**Tag Syntax**

&lt;v: *element* style="flip: *expression* "&gt;

**Script Syntax**

*element* .style.flip="*expression*"

*expression*=*element*.style.flip

**Remarks**

Values include:



| Value | Description                                           |
|-------|-------------------------------------------------------|
| x     | Flip along the y-axis, reversing the *x*-coordinates. |
| y     | Flip along the *x*-axis, reversing the y-coordinates. |
| xy    | Flip along both the y- and *x*-axis.                  |
| yx    | Flip along both the *x*- and *y*-axis.                |



 

*VML Standard Attribute*

**See Also**

[VgFlipOrientation](msdn-online-vector-markup-language-object-model-reference.md#vgfliporientation)

**Example**

The shape is flipped along the *y* -axis by reversing the *x* -coordinates.


```HTML
   <v:rect id=myrect fillcolor="red"
   style="position:relative;top:1;left:1;width:20;height:20;flip:x">
   </v:rect>
```



[Flip Attribute Example](http://samples.msdn.microsoft.com/workshop/samples/vml/shape/examples/x_flip.md). (Requires Microsoft Internet Explorer 5 or greater.)

 

 



