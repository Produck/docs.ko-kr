---
title: 라우팅 계약
ms.date: 03/30/2017
ms.assetid: 9ceea7ae-ea19-4cf9-ba4f-d071e236546d
ms.openlocfilehash: 64ebb673b17159967bb4acd4e3a5e0a3f89142f5
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/04/2018
---
# <a name="routing-contracts"></a>라우팅 계약
라우팅 계약은 라우팅 서비스에서 처리할 수 있는 메시지 패턴을 정의합니다.  각 계약은 형식이 없으며 메시지 스키마나 동작을 몰라도 서비스에서 메시지를 받을 수 있도록 합니다. 따라서 라우트할 기본 메시지의 세부 사항에 대한 추가 구성 없이 라우팅 서비스에서 일반적인 방식으로 메시지를 라우트할 수 있습니다.  
  
## <a name="routing-contracts"></a>라우팅 계약  
 라우팅 서비스에서 제네릭 WCF 메시지 개체를 허용하기 때문에 계약을 선택할 때 가장 중요한 고려 사항은 클라이언트 및 서비스와 통신할 때 사용할 채널의 셰이프입니다. 메시지를 처리할 때 라우팅 서비스에서 대칭 메시지 펌프를 사용하므로 인바운드 계약의 셰이프와 아웃바운드 계약의 셰이프가 일치해야 합니다. 그러나 서비스 모델 디스패처 디스패처가 이중 채널 요청-회신 채널로 변환 하거나 필요 하지 않습니다 (즉 사용 되지 않는 경우 세션 지원을 채널에서 제거 하는 등 모양을 수정할 수 있는 경우도 있습니다. 때 **SessionMode.Allowed**개체로 변환 하는 **IInputSessionChannel** 에 **IInputChannel**).  
  
 이러한 메시지 펌프를 지원하기 위해 라우팅 서비스는 <xref:System.ServiceModel.Routing> 네임스페이스에 자신이 사용하는 서비스 끝점을 정의할 때 사용되어야 하는 계약을 제공합니다. 이러한 계약은 형식이 없기 때문에 모든 메시지 형식이나 동작을 받을 수 있도록 하고 특정 메시지 스키마를 몰라도 라우팅 서비스에서 메시지를 처리할 수 있도록 합니다. 라우팅 서비스에서 사용 하는 계약에 대 한 자세한 내용은 참조 [라우팅 계약](../../../../docs/framework/wcf/feature-details/routing-contracts.md)합니다.  
  
 라우팅 서비스에서 제공하는 계약은 <xref:System.ServiceModel.Routing> 네임스페이스에 있습니다. 다음 표에서는 이러한 계약에 대해 설명합니다.  
  
|계약|모양|채널 셰이프|  
|--------------|-----------|-------------------|  
|<xref:System.ServiceModel.Routing.ISimplexDatagramRouter>|SessionMode = SessionMode.Allowed<br /><br /> AsyncPattern = true<br /><br /> IsOneWay = true|IInputChannel -> IOutputChannel|  
|<xref:System.ServiceModel.Routing.ISimplexSessionRouter>|SessionMode = SessionMode.Required<br /><br /> AsyncPattern = true<br /><br /> IsOneWay = true|IInputSessionChannel -> IOutputSessionChannel|  
|<xref:System.ServiceModel.Routing.IRequestReplyRouter>|SessionMode = SessionMode.Allowed<br /><br /> AsyncPattern = true|IReplyChannel -> IRequestChannel|  
|<xref:System.ServiceModel.Routing.IDuplexSessionRouter>|SessionMode=SessionMode.Required<br /><br /> CallbackContract=typeof(ISimplexSession)<br /><br /> AsyncPattern = true<br /><br /> IsOneWay = true<br /><br /> TransactionFlow(TransactionFlowOption.Allowed)|IDuplexSessionChannel -> IDuplexSessionChannel|  
  
## <a name="see-also"></a>참고 항목  
 [라우팅 서비스](http://msdn.microsoft.com/library/5ac8718c-bcef-456f-bfd5-1e60a30d6eaa)  
 [라우팅 소개](../../../../docs/framework/wcf/feature-details/routing-introduction.md)
