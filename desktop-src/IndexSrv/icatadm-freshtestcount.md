---
title: ICatAdm FreshTestCount property
description: Contains the number of entries in the fresh test list.
ms.assetid: 8b3be607-1a2f-4151-b72c-b586f4d93990
keywords:
- FreshTestCount property Indexing Service
- FreshTestCount property Indexing Service , ICatAdm interface
- ICatAdm interface Indexing Service , FreshTestCount property
topic_type:
- apiref
api_name:
- ICatAdm.FreshTestCount
- ICatAdm.get_FreshTestCount
api_location:
- Ciodm.dll
api_type:
- COM
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# ICatAdm::FreshTestCount property

\[Indexing Service is no longer supported as of Windows XP and is unavailable for use as of Windows 8. Instead, use [Windows Search](https://msdn.microsoft.com/library/windows/desktop/aa965362) for client side search and [Microsoft Search Server Express]( http://go.microsoft.com/fwlink/p/?linkid=258445) for server side search.\]

Contains the number of entries in the fresh test list.

This property is read-only.

## Syntax


```C++
HRESULT get_FreshTestCount(
  [out, retval] LONG *pVal
);
```



## Property value

The number of entries in the fresh test list.

## Remarks

Retrieving this property requires Indexing Service to be running. If it is not running, an error object is created with the **Number** property set to CI\_E\_NOT\_RUNNING.

## Requirements



|                                     |                                                                                      |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 2000 Professional \[desktop apps only\]<br/>                           |
| Minimum supported server<br/> | Windows 2000 Server \[desktop apps only\]<br/>                                 |
| End of client support<br/>    | Windows 7<br/>                                                                 |
| End of server support<br/>    | Windows Server 2008 R2<br/>                                                    |
| DLL<br/>                      | <dl> <dt>Ciodm.dll</dt> </dl> |



## See also

<dl> <dt>

[**ICatAdm**](icatadm.md)
</dt> </dl>

 

 




