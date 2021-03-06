---
title: '방법: 펜을 사용하여 선 그리기'
ms.date: 03/30/2017
dev_langs:
- csharp
- vb
helpviewer_keywords:
- lines [Windows Forms], drawing
- pens [Windows Forms], drawing lines
ms.assetid: 0828c331-a438-4bdd-a4d6-3ef1e59e8795
ms.openlocfilehash: 6a728bcaf9946b2b92ce0ee97599f4c4fd0fea69
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/04/2018
---
# <a name="how-to-use-a-pen-to-draw-lines"></a>방법: 펜을 사용하여 선 그리기
필요한 줄을 그리려면는 <xref:System.Drawing.Graphics> 개체 및 <xref:System.Drawing.Pen> 개체입니다. <xref:System.Drawing.Graphics> 개체를 제공는 <xref:System.Drawing.Graphics.DrawLine%2A> 메서드, 및 <xref:System.Drawing.Pen> 개체 선의 색 및 너비와 같은 기능을 저장 합니다.  
  
## <a name="example"></a>예제  
 다음 예제에서 선을 그립니다 (20, 10)에 (300, 100). 첫 번째 문은 사용 하 여는 <xref:System.Drawing.Pen.%23ctor%2A> 클래스 생성자 검정 펜을 만들려고 합니다. 에 전달 되는 하나의 인수는 <xref:System.Drawing.Pen.%23ctor%2A> 생성자는 한 <xref:System.Drawing.Color> 사용 하 여 만든 개체는 <xref:System.Drawing.Color.FromArgb%2A> 메서드. 만드는 데 사용 되는 값은 <xref:System.Drawing.Color> 개체-(255, 0, 0, 0)-색의 알파, 빨간색, 녹색 및 파랑 구성 요소에 해당 합니다. 이러한 값에는 불투명 한 검정색 펜을 정의합니다.  
  
 [!code-csharp[System.Drawing.UsingAPen#11](../../../../samples/snippets/csharp/VS_Snippets_Winforms/System.Drawing.UsingAPen/CS/Class1.cs#11)]
 [!code-vb[System.Drawing.UsingAPen#11](../../../../samples/snippets/visualbasic/VS_Snippets_Winforms/System.Drawing.UsingAPen/VB/Class1.vb#11)]  
  
## <a name="compiling-the-code"></a>코드 컴파일  
 앞의 예제는 Windows forms에서 사용하도록 설계되었으며 <xref:System.Windows.Forms.PaintEventArgs> 이벤트 처리기의 매개 변수인 `e`<xref:System.Windows.Forms.Control.Paint>가 필요합니다.  
  
## <a name="see-also"></a>참고 항목  
 <xref:System.Drawing.Pen>  
 [펜을 사용하여 선과 도형 그리기](../../../../docs/framework/winforms/advanced/using-a-pen-to-draw-lines-and-shapes.md)  
 [GDI+의 펜, 선 및 사각형](../../../../docs/framework/winforms/advanced/pens-lines-and-rectangles-in-gdi.md)
