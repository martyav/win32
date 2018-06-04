---
Description: The GetEnumObject method enumerates the bidi requests in a list.
ms.assetid: 1aa7b934-c56b-4bfb-800e-950e1dbd5ba3
title: IBidiRequestContainer::GetEnumObject method
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# IBidiRequestContainer::GetEnumObject method

The **GetEnumObject** method enumerates the bidi requests in a list.

## Syntax


```C++
HRESULT GetEnumObject(
  [out] IEnumUnknown **ppenum
);
```



## Parameters

<dl> <dt>

*ppenum* \[out\]
</dt> <dd>

Pointer to the variable that receives a pointer to the [**IEnumUnknown**](https://www.bing.com/search?q=**IEnumUnknown**) interface that enumerates the bidi requests in the container.

</dd> </dl>

## Return value

The method returns one of the following values. For more information about COM error codes, see [Error Handling](https://www.bing.com/search?q=Error Handling).



| Value                                                                                            | Description                                                                        |
|--------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------|
| <dl> <dt>**S\_OK**</dt> </dl>             | The operation was successfully carried out.<br/>                             |
| <dl> <dt>**E\_HANDLE**</dt> </dl>         | The interface handle was invalid.<br/>                                       |
| <dl> <dt>**None of the above**</dt> </dl> | The **HRESULT** contains an error code corresponding to the last error.<br/> |



 

## Remarks

An application can call [**IEnumUnknown::Next**](https://www.bing.com/search?q=**IEnumUnknown::Next**) to retrieve one or more [**IBidiRequest**](ibidirequest.md) interfaces.

## Requirements



|                                     |                                                                                        |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows XP<br/>                                                                  |
| Minimum supported server<br/> | Windows Server 2003<br/>                                                         |
| Target platform<br/>          | <dl> <dt>Desktop</dt> </dl>     |
| Header<br/>                   | <dl> <dt>Bidispl.h</dt> </dl>   |
| DLL<br/>                      | <dl> <dt>Bidispl.dll</dt> </dl> |



## See also

<dl> <dt>

[Bidirectional Communication Interfaces](bidirectional-communication-interfaces.md)
</dt> <dt>

[Bidirectional Communication Schema](https://www.bing.com/search?q=Bidirectional Communication Schema)
</dt> <dt>

[**IBidiRequestContainer**](ibidirequestcontainer.md)
</dt> <dt>

[**IEnumUnknown**](https://www.bing.com/search?q=**IEnumUnknown**)
</dt> </dl>

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bprint\print%5D:%20IBidiRequestContainer::GetEnumObject%20method%20%20RELEASE:%20%285/12/2018%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/en-us/default.aspx. "Send comments about this topic to Microsoft")




