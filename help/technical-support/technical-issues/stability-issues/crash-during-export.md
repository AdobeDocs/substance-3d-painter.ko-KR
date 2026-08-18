---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/stability-issues/crash-during-export.html"
breadcrumb-title: ''
description: 안정적인 텍스처 내보내기 워크플로우를 위해 내보내기 작업 중에 Substance 3D Painter 충돌을 수정하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Stability Issues > Crash during export
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 내보내기 중 충돌
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 0%

---


# 내보내기 중 충돌

일부 특정 사례에서는 특히 매우 높은 해상도(예: 4K 또는 8K)로 내보내는 동안 Substance 3D Painter 충돌이 발생할 수 있습니다. 다음은 이 문제의 가장 일반적인 원인 목록입니다.

## TDR(시간 초과 검색 및 복구)

TDR(Timeout Detection and Recovery)은 GPU가 끝나지 않는 계산으로 시스템을 잠그는 것을 방지하기 위한 Microsoft Windows의 안전 메커니즘입니다. 이 메커니즘은 기본적으로 Substance 3D Painter에 대해 너무 제한적입니다.

자세한 내용은 [GPU 드라이버가 긴 계산에 충돌함(TDR 충돌)](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/gpu-drivers-crash-with-long-computations-128745489.html)을 참조하세요.

## 가상 메모리 부족

내보내는 경우 대량의 RAM(컴퓨터 메모리)이 소모될 수 있으며, 이 경우 시스템의 RAM이 부족할 경우 가상 메모리에서 폴백을 시도합니다. 가상 메모리는 일반적으로 하드 디스크 드라이브에 저장된 추가 메모리입니다. 가상 메모리 크기가 너무 작으면 총 메모리가 부족하여 Substance 3D Painter이 충돌합니다.

자세한 내용은 [가상 메모리 부족 충돌](crash-with-low-virtual-memory.md)을 참조하세요.

## 디스크 공간 부족

SVT(Sparse Virtual Textures)가 도입되었기 때문에 Substance 3D Painter은 디스크의 일부 캐시를 스트리밍하여 성능 균형을 맞출 수 있습니다. 디스크에 사용 가능한 공간이 충분하지 않으면 응용 프로그램에서 캐시를 전송 및 쓰지 못했기 때문에 충돌이 발생할 수 있습니다.

캐시 위치는 기본 시스템 임시 파일 폴더에서 이동할 수 있습니다. 자세한 내용은 [스파스 가상 텍스처](../../../features/sparse-virtual-textures.md)를 참조하십시오.

## 오버클럭된 GPU 주파수

오버클럭된 GPU는 처음에 GPU 생성자가 설계하지 않은 주파수를 실행하므로 불안정할 수 있습니다. 잠시 동안 오버클럭킹을 비활성화하는 데 도움이 될 수 있습니다.

자세한 내용은 [오버클럭된 GPU로 작업할 때 충돌](../gpu-issues/crash-when-working-with-overclocked-gpu.md)을 참조하세요.
