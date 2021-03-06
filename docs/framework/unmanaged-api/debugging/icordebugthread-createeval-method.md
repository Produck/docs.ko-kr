---
title: ICorDebugThread::CreateEval 메서드
ms.date: 03/30/2017
api_name:
- ICorDebugThread.CreateEval
api_location:
- mscordbi.dll
api_type:
- COM
f1_keywords:
- ICorDebugThread::CreateEval
helpviewer_keywords:
- CreateEval method [.NET Framework debugging]
- ICorDebugThread::CreateEval method [.NET Framework debugging]
ms.assetid: 36605067-33d3-4579-9c72-fb0e551ab0f1
topic_type:
- apiref
author: rpetrusha
ms.author: ronpet
ms.openlocfilehash: 5e2d99d85a6e6b09558e5941d08a7f522aaf66cb
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/04/2018
---
# <a name="icordebugthreadcreateeval-method"></a>ICorDebugThread::CreateEval 메서드
수집 하 고이 ICorDebugThread 기능을 노출 하는 ICorDebugEval 개체를 만듭니다.  
  
## <a name="syntax"></a>구문  
  
```  
HRESULT CreateEval (  
    [out] ICorDebugEval   **ppEval  
);  
```  
  
#### <a name="parameters"></a>매개 변수  
 `ppEval`  
 [out] 주소에 대 한 포인터는 `ICorDebugEval` 수집 하 고이 스레드에 기능을 노출 하는 개체입니다.  
  
## <a name="remarks"></a>설명  
 평가 개체는 계산을 수행 하기 전에 스레드의 새 체인을 푸시합니다. 현재 수행 중인 스레드에서 확인이 완료 될 때까지 계산을 중단 합니다.  
  
## <a name="requirements"></a>요구 사항  
 **플랫폼:** 참조 [시스템 요구 사항](../../../../docs/framework/get-started/system-requirements.md)합니다.  
  
 **헤더:** CorDebug.idl, CorDebug.h  
  
 **라이브러리:** CorGuids.lib  
  
 **.NET framework 버전:** [!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]
