---
title: false 연산자(C# 참조)
ms.date: 07/20/2015
ms.prod: .net
ms.technology:
- devlang-csharp
ms.topic: article
helpviewer_keywords:
- false operator keyword [C#]
ms.assetid: 81a888fd-011e-4589-b242-6c261fea505e
caps.latest.revision: 21
author: BillWagner
ms.author: wiwagn
ms.openlocfilehash: 6f9761fb49e2c7f6e4a7615e64cec9fed88318c1
ms.sourcegitcommit: 4f3fef493080a43e70e951223894768d36ce430a
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/21/2017
---
# <a name="false-operator-c-reference"></a>false 연산자(C# 참조)
[bool](../../../csharp/language-reference/keywords/bool.md) 값 `true`를 반환하여 피연산자가 `false`임을 나타내고, false가 아니면 `false`를 반환합니다.  
  
 C# 2.0 이전에는 `true` 및 `false` 연산자를 사용하여 `SqlBool` 등의 형식과 호환되는 사용자 정의 nullable 값 형식을 만들었습니다. 그러나 이제 언어에서 nullable 값 형식에 대한 기본 제공 지원을 제공하며, 가능한 한 `true` 및 `false` 연산자를 오버로드하는 대신 이러한 형식을 사용해야 합니다. 자세한 내용은 [Nullable 형식](../../../csharp/programming-guide/nullable-types/index.md)을 참조하세요.  
  
 nullable 부울을 사용하는 경우 하나 또는 두 값이 모두 null일 수 있기 때문에 `a != b` 식이 `!(a == b)`와 다를 수 있습니다. 식에서 null 값을 올바르게 처리하려면 `true` 및 `false` 연산자를 별도로 둘 다 오버로드해야 합니다. 다음 예제에서는 `true` 및 `false` 연산자를 오버로드하고 사용하는 방법을 보여 줍니다.  
  
 [!code-csharp[csrefKeywordsOperator#16](../../../csharp/language-reference/keywords/codesnippet/CSharp/false-operator_1.cs)]  
  
 [if](../../../csharp/language-reference/keywords/if-else.md), [do](../../../csharp/language-reference/keywords/do.md), [while](../../../csharp/language-reference/keywords/while.md) 및 [for](../../../csharp/language-reference/keywords/for.md) 문의 제어 식과 [조건식](../../../csharp/language-reference/operators/conditional-operator.md)에서 `true` 및 `false` 연산자를 오버로드하는 형식을 사용할 수 있습니다.  
  
 형식이 `false` 연산자를 정의하는 경우 [true](../../../csharp/language-reference/keywords/true.md) 연산자도 정의해야 합니다.  
  
 형식에서 직접 조건부 논리 연산자([&&](../../../csharp/language-reference/operators/conditional-and-operator.md) 및 [&#124;&#124;](../../../csharp/language-reference/operators/conditional-or-operator.md))를 오버로드할 수는 없지만 일반 논리 연산자와 `true` 및 `false` 연산자를 오버로드하면 동일한 효과를 얻을 수 있습니다.  
  
## <a name="c-language-specification"></a>C# 언어 사양  
 [!INCLUDE[CSharplangspec](~/includes/csharplangspec-md.md)]  
  
## <a name="see-also"></a>참고 항목  
 [C# 참조](../../../csharp/language-reference/index.md)  
 [C# 프로그래밍 가이드](../../../csharp/programming-guide/index.md)  
 [C# 키워드](../../../csharp/language-reference/keywords/index.md)  
 [C# 연산자](../../../csharp/language-reference/operators/index.md)  
 [true](../../../csharp/language-reference/keywords/true.md)
