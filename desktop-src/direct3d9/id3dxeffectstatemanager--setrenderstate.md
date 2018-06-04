---
Description: A callback function that must be implemented by a user to set render state.
ms.assetid: a5a27e30-c141-44a4-b8d4-38c1d6076b2a
title: ID3DXEffectStateManager::SetRenderState method
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# ID3DXEffectStateManager::SetRenderState method

A callback function that must be implemented by a user to set render state.

## Syntax


```C++
HRESULT SetRenderState(
  [in] D3DRENDERSTATETYPE State,
  [in] DWORD              Value
);
```



## Parameters

<dl> <dt>

*State* \[in\]
</dt> <dd>

Type: **[**D3DRENDERSTATETYPE**](https://msdn.microsoft.com/windows/desktop/2fd56388-f3bd-409f-876c-ae893840b623)**

The render state to set. [**D3DRENDERSTATETYPE**](https://msdn.microsoft.com/windows/desktop/2fd56388-f3bd-409f-876c-ae893840b623)

</dd> <dt>

*Value* \[in\]
</dt> <dd>

Type: **[**DWORD**](https://msdn.microsoft.com/windows/desktop/4553cafc-450e-4493-a4d4-cb6e2f274d46)**

The render state value. See [Effect States (Direct3D 9)](effect-states.md).

</dd> </dl>

## Return value

Type: **[**HRESULT**](https://msdn.microsoft.com/windows/desktop/455d07e9-52c3-4efb-a9dc-2955cbfd38cc)**

The user-implemented method should return S\_OK. If the callback fails when setting the device state, either of the following will occur:

-   The effect will fail during [**ID3DXEffect::BeginPass**](id3dxeffect--beginpass.md).
-   The dynamic effect state call (such as [**IDirect3DDevice9::SetRenderState**](/windows/desktop/api/d3d9helper/nf-d3d9-idirect3ddevice9-setrenderstate)) will fail.

## Requirements



|                    |                                                                                          |
|--------------------|------------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>D3DX9Effect.h</dt> </dl> |
| Library<br/> | <dl> <dt>D3dx9.lib</dt> </dl>     |



## See also

<dl> <dt>

[ID3DXEffectStateManager](id3dxeffectstatemanager.md)
</dt> </dl>

 

 



