---
title: CLUSCTL\_NODE\_SEND\_DUMMY\_GEM\_MESSAGES control code
description: TBD.
audience: developer
author: REDMOND\\markl
manager: REDMOND\\markl
ms.assetid: F29E4B65-01C4-4675-A429-9CAA0A1EE731
ms.prod: windows-server-dev
ms.technology: failover-clustering
ms.tgt_platform: multiple
keywords:
- CLUSCTL_NODE_SEND_DUMMY_GEM_MESSAGES control code Failover Cluster
topic_type:
- apiref
api_name:
- CLUSCTL_NODE_SEND_DUMMY_GEM_MESSAGES
api_location:
- ClusAPI.h
api_type:
- HeaderDef
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# CLUSCTL\_NODE\_SEND\_DUMMY\_GEM\_MESSAGES control code

TBD. Applications use this [control code](about-control-codes.md) as a [**ClusterNodeControl**](/previous-versions/windows/desktop/api/ClusAPI/nf-clusapi-clusternodecontrol) parameter.


```C++
ClusterNodeControl(
  hNode,               // node handle
  hHostNode,           // optional host node
  CLUSCTL_NODE_SEND_DUMMY_GEM_MESSAGES,  // this control code
  lpInBuffer,          // input buffer
  nInBufferSize,       // input buffer size
  lpOutBuffer,         // output buffer: string
  cbOutBufferSize,     // allocated buffer size (bytes)
  lpcbBytesReturned ); // resulting data size (bytes)
```



## Parameters

The following control code function parameter is specific to this control code. For complete parameter descriptions, see [**ClusterNodeControl**](/previous-versions/windows/desktop/api/ClusAPI/nf-clusapi-clusternodecontrol).

<dl> <dt>

*lpOutBuffer* 
</dt> <dd>

A pointer to an output buffer that receives the data for the operation, or **NULL**.

</dd> </dl>

## Return value

[**ClusterNodeControl**](/previous-versions/windows/desktop/api/ClusAPI/nf-clusapi-clusternodecontrol) returns one of the following values.

<dl> <dt>

**ERROR\_SUCCESS**
</dt> <dd>

0

The operation completed successfully. The *lpcbBytesReturned* parameter points to the actual size of the returned data.

</dd> <dt>

**ERROR\_MORE\_DATA**
</dt> <dd>

234 (0xEA)

More data is available. The output buffer pointed to by *lpOutBuffer* was not large enough to hold the data resulting from the operation. The *lpcbBytesReturned* parameter points to the size required for the output buffer.

</dd> <dt>

**[System error code](https://msdn.microsoft.com/library/windows/desktop/ms681381)**
</dt> <dd>

If any other value is returned, then the operation failed. The value of *lpcbBytesReturned* is unreliable.

</dd> </dl>

## Remarks

ClusAPI.h defines the 32 bits of CLUSCTL\_NODE\_SEND\_DUMMY\_GEM\_MESSAGES (0x040002C9) as follows (for more information, see [Control Code Architecture](control-code-architecture.md)).



| Component      | Bit location | Value                                                    |
|----------------|--------------|----------------------------------------------------------|
| Object code    | 24 31        | **CLUS\_OBJECT\_NODE** (0x4)<br/>                  |
| Global bit     | 23           | **CLUS\_NOT\_GLOBAL** (0x0)<br/>                   |
| Modify bit     | 22           | **CLUS\_NO\_MODIFY** (0x0)<br/>                    |
| User bit       | 21           | **CLCTL\_CLUSTER\_BASE** (0x0)<br/>                |
| Type bit       | 20           | External (0x0)<br/>                                |
| Operation code | 0 23         | **CLCTL\_SEND\_DUMMY\_GEM\_MESSAGES** (0x2C9)<br/> |
| Access code    | 0 1          | **CLUS\_ACCESS\_READ** (0x1)<br/>                  |



 

## Requirements



|                                     |                                                                                      |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Minimum supported client<br/> | None supported<br/>                                                            |
| Minimum supported server<br/> | Windows Server 2012 R2<br/>                                                    |
| Header<br/>                   | <dl> <dt>ClusAPI.h</dt> </dl> |



## See also

<dl> <dt>

[Node Control Codes](node-control-codes.md)
</dt> <dt>

[**ClusterNodeControl**](/previous-versions/windows/desktop/api/ClusAPI/nf-clusapi-clusternodecontrol)
</dt> </dl>

 

 




