---
title: -warnaserror (Visual Basic)
ms.date: 03/13/2018
helpviewer_keywords:
- warnaserror compiler option [Visual Basic]
- /warnaserror compiler option [Visual Basic]
- -warnaserror compiler option [Visual Basic]
ms.assetid: 49819f1d-a1bd-4201-affe-5afe6d9712e1
author: rpetrusha
ms.author: ronpet
ms.openlocfilehash: 6c04bff4070b0f1c288c8853e5045fbf670d8e9e
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/04/2018
---
# <a name="-warnaserror-visual-basic"></a>-warnaserror (Visual Basic)
컴파일러에서 맨 처음 발견 되는 경고를 오류로 처리 하도록 합니다.  
  
## <a name="syntax"></a>구문  
  
```  
-warnaserror[+ | -][:numberList]  
```  
  
## <a name="arguments"></a>인수  
  
|용어|정의|  
|---|---|  
|+ &#124; -|선택 사항입니다. 기본적으로 `-warnaserror-` 됩니다. 경고 되지 않더라도 컴파일러에서 출력 파일을 생성 합니다. `-warnaserror` 동일한 옵션으로 `-warnaserror+`, 경고를 오류로 처리 합니다.|  
|`numberList`|선택 사항입니다. 경고 ID의 쉼표로 구분 된 목록에 있는 번호는 `-warnaserror` 옵션은 적용 됩니다. 경고 ID를 지정 하는 경우는 `-warnaserror` 옵션은 모든 경고에 적용 됩니다.|  
  
## <a name="remarks"></a>설명  
 `-warnaserror` 모든 경고를 오류로 처리 하는 옵션입니다. 일반적으로 보고 되는 경고는 대신 오류로 보고 되는 모든 메시지입니다. 컴파일러 경고로 동일한 경고를 보고합니다.  
  
 기본적으로 `-warnaserror-` 이 적용 되는 정보 경고를 발생 합니다. `-warnaserror` 동일한 옵션으로 `-warnaserror+`, 경고를 오류로 처리 합니다.  
  
 특정 경고만 경고가 오류로 처리 하려는 경우를 오류로 처리할 경고 번호를 쉼표로 구분 된 목록이 지정할 수 있습니다.  
  
> [!NOTE]
>  `-warnaserror` 옵션에 경고가 표시 되는 방식을 제어 하지 않습니다. 사용 하 여는 [-nowarn](../../../visual-basic/reference/command-line-compiler/nowarn.md) 경고를 사용 하지 않도록 설정 하는 옵션입니다.  
  
|-Warnaserror 모든 경고를 Visual Studio IDE에서 오류로 처리 하도록 설정 하려면|  
|---|  
|1.  **솔루션 탐색기**에서 프로젝트를 선택합니다. **프로젝트** 메뉴에서 **속성**을 클릭합니다. <br />2.  **컴파일** 탭을 클릭합니다.<br />3.  있는지 확인은 **모든 경고를 해제** 확인란이 선택 되어 있습니다.<br />4.  확인 된 **모든 경고를 오류로 처리** 확인란 합니다.|  
  
|-Warnaserror 특정 경고 Visual Studio IDE에서 오류를 처리 하도록 설정 하려면|  
|---|  
|1.  **솔루션 탐색기**에서 프로젝트를 선택합니다. **프로젝트** 메뉴에서 **속성**을 클릭합니다.<br />2.  **컴파일** 탭을 클릭합니다.<br />3.  있는지 확인은 **모든 경고를 해제** 확인란이 선택 되어 있습니다.<br />4.  있는지 확인은 **모든 경고를 오류로 처리** 확인란이 선택 되어 있습니다.<br />5.  선택 **오류** 에서 **알림** 열 옆에 경고를 오류로 처리할지를 실행 합니다.|  
  
## <a name="example"></a>예제  
 다음 코드에서는 `In.vb` 경고가의 첫 번째 오류를 표시 하려면 컴파일러를 안내 합니다.  
  
```console
vbc -warnaserror in.vb  
```  
  
## <a name="example"></a>예제  
 다음 코드에서는 `T2.vb` 만 사용 하지 않는 지역 변수 (42024)에 대 한 경고를 오류로 취급 하 고 있습니다.  
  
```console
vbc -warnaserror:42024 t2.vb  
```  
  
## <a name="see-also"></a>참고 항목  
 [Visual Basic 명령줄 컴파일러](../../../visual-basic/reference/command-line-compiler/index.md)  
 [샘플 컴파일 명령줄](../../../visual-basic/reference/command-line-compiler/sample-compilation-command-lines.md)  
 [Visual Basic에서 경고 구성](/visualstudio/ide/configuring-warnings-in-visual-basic)
