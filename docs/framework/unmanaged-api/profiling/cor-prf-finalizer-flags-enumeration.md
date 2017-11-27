---
title: "COR_PRF_FINALIZER_FLAGS 枚举"
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: reference
api_name: COR_PRF_FINALIZER_FLAGS
api_location: mscorwks.dll
api_type: COM
f1_keywords: COR_PRF_FINALIZER_FLAGS
helpviewer_keywords: COR_PRF_FINALIZER_FLAGS enumeration [.NET Framework profiling]
ms.assetid: 297d7721-3911-4f36-9e34-d9da0c33e22a
topic_type: apiref
caps.latest.revision: "10"
author: mairaw
ms.author: mairaw
manager: wpickett
ms.openlocfilehash: 63707ca18be29555919264f9aa3a0f143efdd374
ms.sourcegitcommit: bd1ef61f4bb794b25383d3d72e71041a5ced172e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2017
---
# <a name="corprffinalizerflags-enumeration"></a><span data-ttu-id="bb7f5-102">COR_PRF_FINALIZER_FLAGS 枚举</span><span class="sxs-lookup"><span data-stu-id="bb7f5-102">COR_PRF_FINALIZER_FLAGS Enumeration</span></span>
<span data-ttu-id="bb7f5-103">描述对象的终结器。</span><span class="sxs-lookup"><span data-stu-id="bb7f5-103">Describes the finalizer for an object.</span></span>  
  
## <a name="syntax"></a><span data-ttu-id="bb7f5-104">语法</span><span class="sxs-lookup"><span data-stu-id="bb7f5-104">Syntax</span></span>  
  
```  
typedef enum {  
    COR_PRF_FINALIZER_CRITICAL = 0x1  
} COR_PRF_FINALIZER_FLAGS;  
```  
  
## <a name="members"></a><span data-ttu-id="bb7f5-105">成员</span><span class="sxs-lookup"><span data-stu-id="bb7f5-105">Members</span></span>  
  
|<span data-ttu-id="bb7f5-106">成员</span><span class="sxs-lookup"><span data-stu-id="bb7f5-106">Member</span></span>|<span data-ttu-id="bb7f5-107">描述</span><span class="sxs-lookup"><span data-stu-id="bb7f5-107">Description</span></span>|  
|------------|-----------------|  
|`COR_PRF_FINALIZER_CRITICAL`|<span data-ttu-id="bb7f5-108">终结器至关重要。</span><span class="sxs-lookup"><span data-stu-id="bb7f5-108">The finalizer is critical.</span></span>|  
  
## <a name="remarks"></a><span data-ttu-id="bb7f5-109">备注</span><span class="sxs-lookup"><span data-stu-id="bb7f5-109">Remarks</span></span>  
 <span data-ttu-id="bb7f5-110">`COR_PRF_FINALIZER_FLAGS`枚举由[icorprofilercallback2:: Finalizeableobjectqueued](../../../../docs/framework/unmanaged-api/profiling/icorprofilercallback2-finalizeableobjectqueued-method.md)方法，用于描述一个对象的终结器。</span><span class="sxs-lookup"><span data-stu-id="bb7f5-110">The `COR_PRF_FINALIZER_FLAGS` enumeration is used by the [ICorProfilerCallback2::FinalizeableObjectQueued](../../../../docs/framework/unmanaged-api/profiling/icorprofilercallback2-finalizeableobjectqueued-method.md) method to describe the finalizer for an object.</span></span>  
  
## <a name="requirements"></a><span data-ttu-id="bb7f5-111">要求</span><span class="sxs-lookup"><span data-stu-id="bb7f5-111">Requirements</span></span>  
 <span data-ttu-id="bb7f5-112">**平台：**请参阅[系统要求](../../../../docs/framework/get-started/system-requirements.md)。</span><span class="sxs-lookup"><span data-stu-id="bb7f5-112">**Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).</span></span>  
  
 <span data-ttu-id="bb7f5-113">**头文件：** CorProf.idl、CorProf.h</span><span class="sxs-lookup"><span data-stu-id="bb7f5-113">**Header:** CorProf.idl, CorProf.h</span></span>  
  
 <span data-ttu-id="bb7f5-114">**库：** CorGuids.lib</span><span class="sxs-lookup"><span data-stu-id="bb7f5-114">**Library:** CorGuids.lib</span></span>  
  
 <span data-ttu-id="bb7f5-115">**.NET framework 版本：**[!INCLUDE[net_current_v20plus](../../../../includes/net-current-v20plus-md.md)]</span><span class="sxs-lookup"><span data-stu-id="bb7f5-115">**.NET Framework Versions:** [!INCLUDE[net_current_v20plus](../../../../includes/net-current-v20plus-md.md)]</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="bb7f5-116">另请参阅</span><span class="sxs-lookup"><span data-stu-id="bb7f5-116">See Also</span></span>  
 [<span data-ttu-id="bb7f5-117">分析枚举</span><span class="sxs-lookup"><span data-stu-id="bb7f5-117">Profiling Enumerations</span></span>](../../../../docs/framework/unmanaged-api/profiling/profiling-enumerations.md)