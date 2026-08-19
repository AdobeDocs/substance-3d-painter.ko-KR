---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/technical-support/technical-issues/gpu-issues/gpu-drivers-crash-with-long-computations-tdr-crash.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 긴 계산 중에 GPU 드라이버 충돌을 해결하여 TDR 시간 초과 오류를 방지하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > GPU drivers crash with long computations (TDR crash)
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 긴 계산과 함께 GPU 드라이버 충돌(TDR 충돌)
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '859'
ht-degree: 0%

---


# 긴 계산과 함께 GPU 드라이버 충돌(TDR 충돌)

Substance 3D Painter의 ![TDR 경고](../../../assets/tdr-window-v2.png "Substance 3D Painter의 TDR 경고"){zoomable="yes"}

Windows에서 Substance 3D Painter이 현재 TDR 값이 특정 제한(10초) 미만임을 감지하면 이 창이 나타납니다.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

## GPU 드라이버가 충돌하는 이유는 무엇입니까?

</td>
<td style="border: 0;" valign="top">

### TDR 값을 편집하는 방법

</td>
<td style="border: 0;" valign="top">

### TDR 값을 기본값으로 되돌리기

</td>
</tr>
</table>

## GPU 드라이버가 충돌하는 이유는 무엇입니까?

렌더링 또는 GPU 계산이 **시스템을 잠그는 것**&#x200B;을 방지하기 위해, Windows 운영 체제 **렌더링이 몇 초 이상 걸릴 때마다 GPU 드라이버를 종료합니다**. 드라이버를 제거하면 해당 드라이버를 사용하는 응용 프로그램이 자동으로 충돌합니다. 렌더링 작업이나 계산이 얼마나 걸릴 수 있는지 알 수 없습니다(GPU, 드라이버, OS, 메시 크기, 텍스처 크기 등에 따라 다름). 따라서 컴퓨터가 처리해야 하는 정도를 제한하고 응용 프로그램 수준에서 충돌을 피할 수 없습니다.

Windows에는 GPU 드라이버를 종료하기 전에 OS가 기다려야 하는 시간을 지정하는 **레지스트리** **키**&#x200B;가 있습니다. 응용 프로그램에서는 이 설정을 직접 수정할 권한이 없으므로 이 절차는 수동으로 수행해야 합니다(아래 참조).

자세한 내용은 공식 문서 <https://docs.microsoft.com/en-us/windows-hardware/drivers/display/tdr-registry-keys>을(를) 참조하십시오.

### 변경해야 하는 키 목록

TDR을 조정하려면 TDR 지연을 늘리기만 하면 됩니다. **TdrDelay** 및 **TdrDdiDelay**&#x200B;을 모두 더 높은 값(예: 60초)으로 변경하십시오.

![Windows 레지스트리 편집기의 TDR 키](../../../assets/registry-example.png "Windows 레지스트리 편집기의 TDR 키"){zoomable="yes"}

>[!NOTE]
>
> 이러한 키는 Windows 업데이트 또는 GPU 드라이버 업데이트로 기본값으로 재설정할 수 있습니다.

## TDR 값을 편집하는 방법

다음 절차에 따라 TDR 값을 변경합니다.

***두 개의 다른 키를 만들거나 편집해야 합니다.***

>[!WARNING]
>
> 레지스트리를 편집하면 시스템을 시작하지 못할 수 있고 전체 운영 체제를 다시 설치해야 할 수도 있는 심각하고 예기치 않은 결과가 발생할 수 있습니다. 그러나 이 페이지에서 언급한 레지스트리 키는 이러한 종류의 문제를 만들지 않아야 합니다.
> 
> Adobe은 시스템 레지스트리를 수정하여 시스템에 발생한 손상에 대해 책임을 지지 않습니다.

### 1 - 실행 창 열기

**시작** 및 **실행**&#x200B;을 클릭합니다(또는 **Windows** 및 **R** 키를 누름). **실행** 창이 열립니다.

![Windows 실행 대화 상자](../../../assets/run-window.png "Windows 실행 대화 상자"){zoomable="yes"}

### 2 - 레지스트리 편집기 시작

텍스트 필드에 **regedit**&#x200B;을(를) 입력하고 **확인**&#x200B;을 누릅니다.

Windows 실행 대화 상자의 ![&#39;regedit&#39;](../../../assets/run-regedit-2.png " Windows 실행 대화 상자의 &#39;regedit&#39;"){zoomable="yes"}

### 3 - GraphicsDrivers 레지스트리 키로 이동합니다.

레지스트리 창이 열립니다.\
왼쪽 창에서 다음 위치로 이동하여 트리에서 **GraphicsDrivers** 키로 이동합니다.

```
Computer\HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\GraphicsDrivers
```


다음 단계를 진행하기 전에 레지스트리 **아래 키**&#x200B;에서 **GraphicsDrivers의**&#x200B;을(를) 유지하고&#x200B;**클릭하지 않도록** 하세요.

+++Windows 레지스트리 트리의 &#39;GraphicsDrivers&#39;
Windows 레지스트리 트리의 ![&#39;GraphicsDrivers&#39;](../../../assets/reg-left-pane.png " Windows 레지스트리 트리의 &#39;GraphicsDriver&#39;"){zoomable="yes"}



+++

### 4 - TdrDelay 값 추가 또는 편집

>[!NOTE]
>
> <b>TdrDelay</b> 값 <b>이(가) 아직 존재하지 않는 경우</b> 오른쪽 창에서 마우스 오른쪽 단추를 클릭하고 <b>새로 만들기 > DWORD(32비트) 값</b> 을 선택합니다. 이름을 &quot;<b>TdrDelay</b>&quot;로 지정합니다. 대/소문자가 중요한 경우 반드시 그 뒤에 따라가도록 하고(그리고 후행 공백과 같은 다른 문자가 없는지 확인).
> 
> ![](../../../assets/create-value.png)

**오른쪽 창**&#x200B;에서 값 **TdrDelay**&#x200B;을(를) 두 번 클릭합니다. **기본** 설정을 **소수점**(으)로 변경합니다. 값을 기본값인 **2**&#x200B;이(가) 아닌 값으로 설정합니다(권장: **60**).

이 값은 연산 중 GPU가 응답하지 않음을 고려하기 전에 운영 체제가 대기하는 시간을 초 단위로 나타냅니다.

Windows 레지스트리 편집기의 ![&#39;TdrDelay&#39; DWORD 값](../../../assets/tdrdelay-edit.png " Windows 레지스트리 편집기의 &#39;TdrDelay&#39; DWORD 값"){zoomable="yes"}

### 5 - TdrDdiDelay 값 추가 또는 편집

>[!NOTE]
>
> <b>TdrDdiDelay</b> 값 <b>이(가) 존재하지 않는 경우</b> , 오른쪽 창에서 마우스 오른쪽 단추를 클릭하고 <b>새로 만들기 > DWORD(32비트) 값</b> 을 선택합니다. 이름을 &quot; <b>TdrDdiDelay</b> &quot;로 지정합니다. 대/소문자가 중요한 경우 반드시 따라야 합니다(공백 등 다른 문자가 없는지 확인).
> 
> ![](../../../assets/create-value.png)

**오른쪽 창**&#x200B;에서 **TdrDdiDelay** 값을 두 번 클릭합니다. **기본** 설정을 **소수점**(으)로 변경합니다. 값을 기본값인 **5** 이외의 값으로 설정합니다(**60** 권장).

이 값은 소프트웨어가 GPU 드라이버를 종료하는 데 너무 많은 시간이 걸린다는 점을 고려하기 전에 운영 체제가 대기하는 시간을 초 단위로 나타냅니다.

**16진수**&#x200B;가 기본값입니다. **10진수**(으)로 전환하여 올바른 값을 표시하십시오. **3C**(16진수)은 **60**(10진수)과(와) 같습니다.

### 6 - 완료 및 다시 시작

오른쪽 창은 이제 다음과 같이 표시됩니다.

Windows 레지스트리 편집기의 ![TDR 키 - 최종](../../../assets/registry-example.png "Windows 레지스트리 편집기의 TDR 키 - 최종"){zoomable="yes"}

레지스트리 편집기를 **닫기**. **시작** 및 **다시 시작** 을 사용하여 **컴퓨터를 다시 시작**&#x200B;합니다.

TdrValue는 컴퓨터가 시작될 때만 나타나므로 강제로 새로 고치려면 다시 부팅해야 합니다.

긴 계산을 수행할 때 응용 프로그램이 여전히 충돌하면 지연 시간(초)을 60에서 120으로 늘려 보십시오.

## TDR 값을 기본값으로 되돌리기

TDR을 기본값으로 되돌리는 방법에는 두 가지가 있습니다.

* 위에 설명된 단계에 따라 **TdrDelay**&#x200B;을(를) **2s**(으)로, **TdrDdiDelay**&#x200B;을(를) **5s**(으)로 설정하십시오.
* 또는 레지스트리 항목에서 **TdrDelay** 및 **TdrDdiDelay** 키를 **제거**&#x200B;합니다.
