---
title: Bluetooth and WSAQUERYSET for Device Inquiry
description: Used to facilitate the discovery of devices and services in the Bluetooth namespace, NS\_BTH.
ms.assetid: '0c0d26f7-b6c3-42a9-8c01-118278c381cc'
keywords: ["Bluetooth and WSAQUERYSET for Device Inquiry Bluetooth", "WSAQUERYSET Bluetooth , for device inquiry"]
---

# Bluetooth and WSAQUERYSET for Device Inquiry

In Bluetooth, the [**WSAQUERYSET**](https://msdn.microsoft.com/library/windows/desktop/ms741679) structure, is used to facilitate the discovery of devices and services in the Bluetooth namespace, NS\_BTH.

The [**WSALookupServiceBegin**](https://msdn.microsoft.com/library/windows/desktop/ms741633) and [**WSALookupServiceNext**](https://msdn.microsoft.com/library/windows/desktop/ms741641) functions use the [**WSAQUERYSET**](https://msdn.microsoft.com/library/windows/desktop/ms741679) structure to obtain information about the device inquiry process. The following table lists and describes member values in the **WSAQUERYSET** structure.

| Member                      | Input to WSALookupServiceBegin with LUP\_CONTAINERS specified                                                                                                                                              | Returned value from WSALookupServiceNext                                                                                                                                                                                                                                                                                                                                                                                        |
|-----------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **dwSize**                  | Must be set to **sizeof**([**WSAQUERYSET**](https://msdn.microsoft.com/library/windows/desktop/ms741679)).                                                                                                                                       | **sizeof**([**WSAQUERYSET**](https://msdn.microsoft.com/library/windows/desktop/ms741679)) returned by system.                                                                                                                                                                                                                                                                                                                                                        |
| **dwOutputFlags**           | Not used.                                                                                                                                                                                                  | May have one or more of these flags set: **BTHNS\_RESULT\_DEVICE\_CONNECTED** Specifies the device is connected.<br/> **BTHNS\_RESULT\_DEVICE\_REMEMBERED** Specifies the device is a remembered device. Not all remembered devices are authenticated.<br/> **BTHNS\_RESULT\_DEVICE\_AUTHENTICATED** Specifies the device is authenticated, paired, or bonded. All authenticated devices are remembered.<br/> |
| **lpszServiceInstanceName** | Not used.                                                                                                                                                                                                  | Display name of the device, originally returned from a Bluetooth Remote Name Request operation, and possibly updated by the local user. Returned if **LUP\_RETURN\_NAME** is specified.                                                                                                                                                                                                                                         |
| **lpServiceClassId**        | Not used.                                                                                                                                                                                                  | The 32-bit Bluetooth class of device (COD) field mapped to the **Data1** member of the GUID. Returned if **LUP\_RETURN\_TYPE** is specified.                                                                                                                                                                                                                                                                                    |
| **lpVersion**               | Not used.                                                                                                                                                                                                  | Not used.                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **lpszComment**             | Not used.                                                                                                                                                                                                  | Not used.                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **dwNameSpace**             | Must be NS\_BTH.                                                                                                                                                                                           | Returns **NS\_BTH**.                                                                                                                                                                                                                                                                                                                                                                                                            |
| **lpNSProviderId**          | Not used.                                                                                                                                                                                                  | Not used.                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **lpszContext**             | Not used.                                                                                                                                                                                                  | Not used.                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **dwNumberOfProtocols**     | Not used.                                                                                                                                                                                                  | Not used.                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **lpafpProtocols**          | Not used.                                                                                                                                                                                                  | Not used.                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **lpszQueryString**         | Not used.                                                                                                                                                                                                  | Not used.                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **dwNumberOfCsAddrs**       | Not used.                                                                                                                                                                                                  | Indicates the number of elements in the array of [**CSADDR\_INFO**](https://msdn.microsoft.com/library/windows/desktop/ms737640) structures.                                                                                                                                                                                                                                                                                                                          |
| **lpcsaBuffer**             | Not used.                                                                                                                                                                                                  | Pointer to a [**CSADDR\_INFO**](https://msdn.microsoft.com/library/windows/desktop/ms737640) structure with its **LocalAddr.lpSockaddr** member pointing to a [**SOCKADDR\_BTH**](sockaddr-bth.md) structure with the address of the remote device. Returned if **LUP\_RETURN\_ADDR** is specified.                                                                                                                                                                  |
| **lpBlob**                  | Optional. May point to a [**BLOB**](https://msdn.microsoft.com/library/windows/desktop/ms737551) structure that points to a [**BTH\_QUERY\_DEVICE**](bth-query-device.md) structure that may limit the length of non-cached device inquiry operations. | Pointer to a [**BLOB**](https://msdn.microsoft.com/library/windows/desktop/ms737551) structure that points to a [**BTH\_DEVICE\_INFO**](bth-device-info.md) structure. **lpBlob** is returned if **LUP\_RETURN\_BLOB** is specified. Specify **LUP\_RETURN\_NAME** to retrieve the name field of **BTH\_DEVICE\_INFO**.                                                                                                                                                     |



�

## Related topics

<dl> <dt>

[Bluetooth and WSAQUERYSET for Set Service](bluetooth-and-wsaqueryset-for-set-service.md)
</dt> <dt>

[Bluetooth and WSAQUERYSET for Service Inquiry](bluetooth-and-wsaqueryset-for-service-inquiry.md)
</dt> <dt>

[Bluetooth and BLOB](bluetooth-and-blob.md)
</dt> <dt>

[Bluetooth and WSALookupServiceBegin](bluetooth-and-wsasetservice.md)
</dt> <dt>

[Bluetooth and WSALookupServiceNext](bluetooth-and-wsasetservice.md)
</dt> <dt>

[**BLOB**](https://msdn.microsoft.com/library/windows/desktop/ms737551)
</dt> <dt>

[**BTH\_DEVICE\_INFO**](bth-device-info.md)
</dt> <dt>

[**BTH\_QUERY\_DEVICE**](bth-query-device.md)
</dt> <dt>

[**CSADDR\_INFO**](https://msdn.microsoft.com/library/windows/desktop/ms737640)
</dt> <dt>

[**SOCKADDR\_BTH**](sockaddr-bth.md)
</dt> <dt>

[**WSAQUERYSET**](https://msdn.microsoft.com/library/windows/desktop/ms741679)
</dt> <dt>

[Windows Sockets](https://msdn.microsoft.com/library/windows/desktop/ms740673)
</dt> </dl>

�

�




