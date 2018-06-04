---
Description: IsapiMaxEntriesInQueryCache
ms.assetid: aa01f1b6-697b-4134-aa8b-32cd686e9208
title: IsapiMaxEntriesInQueryCache
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# IsapiMaxEntriesInQueryCache

> [!Note]  
> Indexing Service is no longer supported as of Windows XP and is unavailable for use as of Windows 8. Instead, use [Windows Search](https://msdn.microsoft.com/windows/desktop/6da601c6-3742-40ad-99f2-8817f7f642b3) for client side search and [Microsoft Search Server Express]( http://go.microsoft.com/fwlink/p/?linkid=258445) for server side search.

 

The **IsapiMaxEntriesInQueryCache** entry determines the maximum number of cached queries.

### Summary



|          |                |
|----------|----------------|
| Type:    | **REG\_DWORD** |
| Units:   | Queries        |
| Default: | 10             |
| Range:   | 0 - 100        |



 

### Remarks

The value of an identically named entry under the [**Catalog**](catalog--property--and-scope-registry-entries.md) subkey for a specific catalog cannot override the value of this entry.

## Related topics

<dl> <dt>

[Main Registry Entries](main-registry-entries.md)
</dt> <dt>

[MaxSimultaneousRequests](maxsimultaneousrequests.md)
</dt> </dl>

 

 


