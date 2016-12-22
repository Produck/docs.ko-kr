---
title: "/= 연산자(C# 참조) | Microsoft Docs"
ms.custom: ""
ms.date: "12/03/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "devlang-csharp"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "/=_CSharpKeyword"
dev_langs: 
  - "CSharp"
helpviewer_keywords: 
  - "/=(나누기 할당 연산자)[C#]"
  - "나누기 할당 연산자(/=)[C#]"
ms.assetid: 50fc02b0-ee9c-4c3e-b58d-d591282caf1c
caps.latest.revision: 17
caps.handback.revision: 17
author: "BillWagner"
ms.author: "wiwagn"
manager: "wpickett"
---
# /= 연산자(C# 참조)
[!INCLUDE[vs2017banner](../../../csharp/includes/vs2017banner.md)]

나누기 대입 연산자입니다.  
  
## 설명  
 다음과 같이 `/=` 대입 연산자를 사용하는 식은  
  
```  
x /= y  
```  
  
 동일한 함수는  
  
```  
x = x / y  
```  
  
 그러나 `x`가 한 번만 계산된다는 점은 다릅니다.  [\/ 연산자](../../../csharp/language-reference/operators/division-operator.md)는 숫자 형식에 대해 나눗셈을 수행하도록 미리 정의되어 있습니다.  
  
 `/=` 연산자는 직접 오버로드될 수 없지만, 사용자 정의 형식으로 [\/ 연산자](../../../csharp/language-reference/operators/division-operator.md)를 오버로드할 수 있습니다\([operator](../../../csharp/language-reference/keywords/operator.md) 참조\).  모든 복합 대입 연산자에서 이항 연산자를 오버로드하면 동일한 복합 대입도 암시적으로 오버로드됩니다.  
  
## 예제  
 [!CODE [csRefOperators#5](../CodeSnippet/VS_Snippets_VBCSharp/csrefOperators#5)]  
  
## 참고 항목  
 [C\# 참조](../../../csharp/language-reference/index.md)   
 [C\# 프로그래밍 가이드](../../../csharp/programming-guide/index.md)   
 [C\# 연산자](../../../csharp/language-reference/operators/index.md)