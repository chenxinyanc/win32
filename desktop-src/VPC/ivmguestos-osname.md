---
title: IVMGuestOS OSName property
description: The name of the guest operating system running in the virtual machine.
ms.assetid: 6381fc15-a6ab-429b-809d-7f89e7ec666d
keywords:
- OSName property Virtual PC
- OSName property Virtual PC , IVMGuestOS interface
- IVMGuestOS interface Virtual PC , OSName property
topic_type:
- apiref
api_name:
- IVMGuestOS.OSName
- IVMGuestOS.get_OSName
api_location:
- VPCCOMInterfaces.h
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
---

# IVMGuestOS::OSName property

\[Windows Virtual PC is no longer available for use as of Windows 8. Instead, use the [Hyper-V WMI provider (V2)](https://docs.microsoft.com/windows/desktop/HyperV_v2/windows-virtualization-portal).\]

Retrieves the name of the guest operating system running in the virtual machine (VM).

This property is read-only.

## Syntax


```C++
HRESULT get_OSName(
  [out, retval] BSTR *guestOSName
);
```



## Property value

The full name (including suite name) of the guest operating system.

## Error codes



| Name/value                                                                                                                                                                       | Meaning                                                         |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------|
| <dl> <dt>S\_OK</dt> <dt>0</dt> </dl>                                          | The operation was successful.<br/>                        |
| <dl> <dt>E\_POINTER</dt> <dt>0x80004003</dt> </dl>                            | The parameter is **NULL**.<br/>                           |
| <dl> <dt>VM\_E\_VM\_NOT\_RUNNING</dt> <dt>0xA0040206</dt> </dl>               | The VM is not running.<br/>                               |
| <dl> <dt>VM\_E\_ADDITIONS\_FEATURE\_NOT\_AVAIL</dt> <dt>0xA0040505</dt> </dl> | Integration components are not installed in this VM.<br/> |
| <dl> <dt>DISP\_E\_EXCEPTION</dt> <dt>0x80020009</dt> </dl>                    | An unexpected error has occurred.<br/>                    |



## Remarks

The VM must be running (that is, fully booted and not shutting down) and integration components must be installed when this method is invoked.

## Requirements



|                                     |                                                                                               |
|-------------------------------------|-----------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 7 \[desktop apps only\]<br/>                                                    |
| Minimum supported server<br/> | None supported<br/>                                                                     |
| End of client support<br/>    | Windows 7<br/>                                                                          |
| Product<br/>                  | Windows Virtual PC<br/>                                                                 |
| Header<br/>                   | <dl> <dt>VPCCOMInterfaces.h</dt> </dl> |
| IID<br/>                      | IID\_IVMGuestOS is defined as 99fea0db-4880-499a-b6d8-73dff9bc91be<br/>                 |



## See also

<dl> <dt>

[**IVMGuestOS**](ivmguestos.md)
</dt> </dl>

 

 





