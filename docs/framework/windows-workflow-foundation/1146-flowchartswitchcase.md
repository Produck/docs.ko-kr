---
title: 1146 - FlowchartSwitchCase
ms.date: 03/30/2017
ms.assetid: 274e9209-1720-4512-a615-e742f00895f4
ms.openlocfilehash: 9f4e3af664ed30634e4b56f16cd6caf2366c3674
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/04/2018
---
# <a name="1146---flowchartswitchcase"></a>1146 - FlowchartSwitchCase
## <a name="properties"></a>속성  
  
|||  
|-|-|  
|ID|1146|  
|키워드|WFActivities|  
|수준|정보|  
|채널|Microsoft-Windows-응용 프로그램 서버-응용 프로그램/디버그|  
  
## <a name="description"></a>설명  
 Flowchart 스위치에서 Case가 선택되었음을 나타냅니다.  
  
## <a name="message"></a>메시지  
 Flowchart '%1'/FlowSwitch - Case '%2'을(를) 선택했습니다.  
  
## <a name="details"></a>설명  
  
|데이터 항목 이름|데이터 항목 형식|설명|  
|--------------------|--------------------|-----------------|  
|FlowChart|xs:string|FlowChart의 표시 이름입니다.|  
|Case|xs:string|switch case가 선택되었습니다.|  
|AppDomain|xs:string|AppDomain.CurrentDomain.FriendlyName에서 반환되는 문자열입니다.|
