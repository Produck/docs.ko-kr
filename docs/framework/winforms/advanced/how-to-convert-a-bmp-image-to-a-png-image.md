---
title: "방법: BMP 이미지를 PNG 이미지로 변환 | Microsoft Docs"
ms.custom: ""
ms.date: "03/30/2017"
ms.prod: ".net-framework"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "dotnet-winforms"
ms.tgt_pltfrm: ""
ms.topic: "article"
dev_langs: 
  - "jsharp"
helpviewer_keywords: 
  - "BMP 이미지, PNG로 변환"
  - "이미지 형식, 상호 변환"
ms.assetid: 9d4a692d-73ac-4ce3-9e05-9ec321e8fbd6
caps.latest.revision: 10
author: "dotnet-bot"
ms.author: "dotnetcontent"
manager: "wpickett"
caps.handback.revision: 10
---
# 방법: BMP 이미지를 PNG 이미지로 변환
이미지 파일 형식 간에 변환하려는 경우가 많습니다.  <xref:System.Drawing.Image> 클래스의 <xref:System.Drawing.Image.Save%2A> 메서드를 호출하고 원하는 이미지 파일 형식에 대해 <xref:System.Drawing.Imaging.ImageFormat>을 지정하여 이 변환을 쉽게 수행할 수 있습니다.  
  
## 예제  
 다음 예제에서는 형식에서 BMP 이미지를 로드하고 PNG 형식으로 이미지를 저장합니다.  
  
 [!code-csharp[UsingImageEncodersDecoders#4](../../../../samples/snippets/csharp/VS_Snippets_Winforms/UsingImageEncodersDecoders/CS/Form1.cs#4)]
 [!code-vb[UsingImageEncodersDecoders#4](../../../../samples/snippets/visualbasic/VS_Snippets_Winforms/UsingImageEncodersDecoders/VB/Form1.vb#4)]  
  
## 코드 컴파일  
 이 예제에는 다음 사항이 필요합니다.  
  
-   Windows Forms 응용 프로그램  
  
-   `System.Drawing.Imaging` 네임스페이스에 대한 참조  
  
## 참고 항목  
 [방법: 설치된 인코더 나열](../../../../docs/framework/winforms/advanced/how-to-list-installed-encoders.md)   
 [관리 GDI\+에서 이미지 인코더 및 디코더 사용](../../../../docs/framework/winforms/advanced/using-image-encoders-and-decoders-in-managed-gdi.md)   
 [비트맵의 유형](../../../../docs/framework/winforms/advanced/types-of-bitmaps.md)