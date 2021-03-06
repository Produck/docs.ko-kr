---
title: 관리되는 응용 프로그램에서의 호스팅
ms.date: 03/30/2017
ms.assetid: af70132d-e9e1-4f32-b20f-f0014629758a
ms.openlocfilehash: f374c199fb1982ab8854e41c0c8308f46451d9d0
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/04/2018
---
# <a name="hosting-in-a-managed-application"></a>관리되는 응용 프로그램에서의 호스팅
모든 Windows Communication Foundation (WCF) 서비스를 호스팅할 수 있습니다 [!INCLUDE[dnprdnshort](../../../../includes/dnprdnshort-md.md)] 응용 프로그램입니다. 자체 호스팅 서비스는 배포하는 데 최소한의 인프라를 필요로 하기 때문에 가장 유연한 호스팅 옵션입니다. 그러나 가장 약한 호스팅 옵션 때문에 이기도 관리 되는 응용 프로그램에는 고급 호스팅 및 관리 기능 인터넷 정보 서비스 (IIS) 및 Windows 서비스 등의 wcf에서는 다른 호스팅 옵션을 제공 하지 않습니다.  
  
 자체 호스팅 서비스를 만들려면 <xref:System.ServiceModel.ServiceHost>의 인스턴스를 만들고 열어, 여기서 서비스의 메시지 수신 대기를 시작합니다. 자세한 내용은 참조 [하는 방법: 관리 되는 응용 프로그램에서 WCF 서비스 호스팅](../../../../docs/framework/wcf/how-to-host-a-wcf-service-in-a-managed-application.md)합니다.  
  
 계약을 정의 계약을 구현 및 관리 되는 응용 프로그램 내에 서비스를 호스트 하는 방법에는 전체 예제에 대 한 참조는 [초보자를 위한 자습서](../../../../docs/framework/wcf/getting-started-tutorial.md) 및 [자체 호스트](../../../../docs/framework/wcf/samples/self-host.md)합니다.  
  
 다음 단원에서는 이 호스팅 옵션을 사용하는 일반적인 시나리오에 대해 설명합니다.  
  
## <a name="console-applications"></a>콘솔 응용 프로그램  
 자체 호스트할 수 있도록 하는 일반적인 시나리오는 콘솔 응용 프로그램 내에서 실행 되는 WCF 서비스입니다. 콘솔 응용 프로그램 내의 WCF 서비스를 호스팅하는 서비스의 개발 단계에서 일반적으로 유용 합니다. 이 경우 쉽게 디버깅을 수행할 수 있으며, 응용 프로그램 내에서 발생하는 상황을 확인하기 위한 추적 정보를 손쉽게 얻을 수 있으며, 새 위치에 서비스를 복사하여 이동하기 용이합니다.  
  
## <a name="rich-client-applications"></a>리치 클라이언트 응용 프로그램  
 자체 호스팅을 사용 Windows Presentation Foundation (WPF) 또는 Windows Forms (WinForms)에 따라 같은 리치 클라이언트 응용 프로그램에는 다른 일반적인 시나리오입니다. 이 호스팅 옵션을 사용하면 리치 클라이언트 응용 프로그램(예: [!INCLUDE[avalon2](../../../../includes/avalon2-md.md)] 및 WinForms 응용 프로그램)에서 외부와 쉽게 통신할 수 있습니다. 예를 들어, 사용 하는 피어 투 피어 공동 작업 클라이언트가 [!INCLUDE[avalon2](../../../../includes/avalon2-md.md)] 해당 사용자 인터페이스에 대 한도 다른 클라이언트가 연결 하 고 정보를 공유할 수 있도록 WCF 서비스를 호스트 하 고 있습니다.  
  
## <a name="see-also"></a>참고 항목  
 [서비스 호스팅](../../../../docs/framework/wcf/hosting-services.md)  
 [초보자를 위한 자습서](../../../../docs/framework/wcf/getting-started-tutorial.md)
