---
title: '방법: Windows Forms MonthCalendar 컨트롤에서 날짜 범위 선택'
ms.date: 03/30/2017
dev_langs:
- csharp
- vb
- cpp
helpviewer_keywords:
- dates [Windows Forms], selecting range in calendar controls
- examples [Windows Forms], calendar controls
- calendars [Windows Forms], selecting date range
- MonthCalendar control [Windows Forms], selecting date range
ms.assetid: 95d9ab95-b0f8-4c19-9f63-b5cd4593a5d0
ms.openlocfilehash: 8b6d64fcffb02c4496cff3f2821861117b0062fd
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/04/2018
---
# <a name="how-to-select-a-range-of-dates-in-the-windows-forms-monthcalendar-control"></a>방법: Windows Forms MonthCalendar 컨트롤에서 날짜 범위 선택
Windows Forms의 중요 한 기능은 <xref:System.Windows.Forms.MonthCalendar> 컨트롤은 사용자가 날짜 범위를 선택할 수 있습니다. 이 기능은의 날짜 선택 기능 개선 된는 <xref:System.Windows.Forms.DateTimePicker> 만 단일 날짜/시간 값을 선택할 수 있는 컨트롤입니다. 날짜 범위를 설정 하거나 속성을 사용 하 여 사용자가 설정한 선택 범위를 가져올 수는 <xref:System.Windows.Forms.MonthCalendar> 제어 합니다. 다음 코드 예제에서는 선택 범위를 설정 하는 방법을 보여 줍니다.  
  
### <a name="to-select-a-range-of-dates"></a>날짜 범위를 선택 하려면  
  
1.  만들 <xref:System.DateTime> 범위에서 첫 번째 및 마지막 날짜를 나타내는 개체입니다.  
  
    ```vb  
    Dim projectStart As Date = New DateTime(2001, 2, 13)  
    Dim projectEnd As Date = New DateTime(2001, 2, 28)  
    ```  
  
    ```csharp  
    DateTime projectStart = new DateTime(2001, 2, 13);  
    DateTime projectEnd = new DateTime(2001, 2, 28);  
    ```  
  
    ```cpp  
    DateTime projectStart = DateTime(2001, 2, 13);  
    DateTime projectEnd = DateTime(2001, 2, 28);  
    ```  
  
2.  <xref:System.Windows.Forms.MonthCalendar.SelectionRange%2A> 속성을 설정합니다.  
  
    ```vb  
    MonthCalendar1.SelectionRange = New SelectionRange(projectStart, projectEnd)  
    ```  
  
    ```csharp  
    monthCalendar1.SelectionRange = new SelectionRange(projectStart, projectEnd);  
    ```  
  
    ```cpp  
    monthCalendar1->SelectionRange = gcnew  
       SelectionRange(projectStart, projectEnd);  
    ```  
  
     – 또는 –  
  
     <xref:System.Windows.Forms.MonthCalendar.SelectionStart%2A> 및 <xref:System.Windows.Forms.MonthCalendar.SelectionEnd%2A> 속성을 설정합니다.  
  
    ```vb  
    MonthCalendar1.SelectionStart = projectStart  
    MonthCalendar1.SelectionEnd = projectEnd  
    ```  
  
    ```csharp  
    monthCalendar1.SelectionStart = projectStart;  
    monthCalendar1.SelectionEnd = projectEnd;  
    ```  
  
    ```cpp  
    monthCalendar1->SelectionStart = projectStart;  
    monthCalendar1->SelectionEnd = projectEnd;  
    ```  
  
## <a name="see-also"></a>참고 항목  
 [MonthCalendar 컨트롤](../../../../docs/framework/winforms/controls/monthcalendar-control-windows-forms.md)  
 [방법: Windows Forms MonthCalendar 컨트롤의 모양 변경](../../../../docs/framework/winforms/controls/how-to-change-monthcalendar-control-appearance.md)  
 [방법: Windows Forms MonthCalendar 컨트롤을 사용하여 특정 날짜를 굵게 표시](../../../../docs/framework/winforms/controls/display-specific-days-in-bold-with-wf-monthcalendar-control.md)  
 [방법: Windows Forms MonthCalendar 컨트롤에서 여러 달 표시](../../../../docs/framework/winforms/controls/display-more-than-one-month-wf-monthcalendar-control.md)
