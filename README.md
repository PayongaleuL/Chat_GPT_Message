# 🧪 Adobe 실험실: 어도비 관련 문제 및 버그 탐구 프로젝트

## 📌 프로젝트 개요

본 저장소는 Adobe의 다양한 소프트웨어(After Effects, Premiere Pro, Photoshop 등)를 사용하면서 겪는 **이상 현상, 버그, 비일관성 있는 기능, 호환성 문제** 등을 수집하고, 이에 대해 **직접 실험한 결과와 해결 시도**를 기록하기 위한 공간입니다.

일반 사용자들은 물론이고 현업에서 어도비 소프트웨어를 쓰는 디자이너, 편집자, 개발자들에게도 유용한 정보를 제공하고자 합니다. 단순한 '에러 보고'를 넘어서 **현상을 재현 가능한 방법으로 정리**하고, **실제 사용 환경과 조건을 기반으로 한 실험 결과**를 통해 문제의 원인과 대응 방안을 찾는 데 목적이 있습니다.

---

## 🎯 프로젝트 목적

- 어도비 프로그램 사용 중 발생하는 버그, 렌더링 오류, UI 오작동 등의 **현상을 체계적으로 정리**
- 문제 상황을 **재현 가능한 형태로 문서화**하여 다른 사용자들도 참고할 수 있도록 제공
- 실험을 통해 얻은 **회피 방법, 임시 해결책, 조건별 결과 차이** 등을 상세히 기록
- Adobe Community 및 Bug Report 제출 시 **참조 가능한 문서 제공**
- 사용자 경험 개선을 위한 **기능 피드백 및 제안 정리**

---

## 🗂️ 실험 항목 구조

각 문제는 **폴더 단위로 분류**되며, 각 폴더 안에는 다음과 같은 구성 요소가 포함됩니다:

- `README.md` — 실험 주제 설명, 배경, 발생 조건, 실험 목적
- `test_project` — 문제가 발생한 실제 어도비 프로젝트 파일 (예: `.aep`, `.prproj`)
- `screenshots` — 문제를 시각적으로 보여주는 스크린샷
- `recordings` — 실시간 재현 영상 (가능한 경우)
- `results.md` — 실험 방법, 환경, 단계별 결과, 해결 가능성 분석
- `workarounds.md` — 회피 방법, 대체 기능, 임시 조치 등
- `references.md` — Adobe Forum, Reddit, Stack Overflow 등에서 참고한 글

---

## 🧪 예시 실험 주제

| 주제 | 설명 |
|------|------|
| 🔄 [After Effects에서 Expression이 랜덤하게 무시되는 버그](/after-effects/expression-random-bug) | 특정 조건에서 `time`이나 `random()` 기반 Expression이 렌더링 시 무시되는 현상 분석 |
| 🖼️ [Premiere Pro에서 PSD 파일의 레이어가 깨지는 문제](/premiere/psd-layer-issue) | 특정 해상도와 색공간 설정 시 PSD 레이어가 정상적으로 출력되지 않음 |
| 🎚️ [Adjustment Layer가 일부 플러그인에서 동작하지 않는 현상](/premiere/adjustment-layer-plugins) | Lumetri, Neat Video 등 일부 효과가 Adjustment Layer 위에서만 무력화되는 사례 |
| 🖥️ [Mac vs Windows 환경에서 동일 프로젝트의 렌더 결과 차이](/cross-platform/render-difference) | 크로스 플랫폼 사용자의 프로젝트 호환 문제 실험 |

---

## 🧾 실험 환경 명세

실험은 다음과 같은 환경에서 이루어졌습니다 (버전에 따라 차이 발생 가능):

- OS:
  - Windows 11 (22H2)
  - macOS Sonoma (14.x)
- Adobe Creative Cloud:
  - After Effects 2024 (버전 24.1~)
  - Premiere Pro 2024 (버전 24.0~)
  - Photoshop 2024 (버전 25.0~)
- 하드웨어:
  - Intel i7 / AMD Ryzen 7 이상
  - RAM 32GB 이상
  - GPU: NVIDIA RTX 3060 이상 또는 Apple M1 이상

---

## 🗣️ 참여 및 제보 방법

같은 문제를 겪고 있거나, 실험을 같이 하고 싶은 분들을 환영합니다!

1. Issue를 통해 버그나 실험 아이디어 제보
2. Pull Request로 새로운 실험 추가 (위 구조 참고)
3. 댓글이나 Discussions에서 경험 공유

---

## 🤝 후원 및 감사

이 저장소는 특정 기업과는 무관하게, **사용자의 자발적인 문제 해결 시도**에 의해 운영됩니다. 실험에 소요되는 시간과 리소스는 전적으로 개인의 열정으로 유지되고 있으며, 작은 응원이나 피드백도 큰 힘이 됩니다.

---

## 📜 라이선스

본 저장소의 실험 결과 및 문서들은 MIT License 하에 자유롭게 사용하실 수 있으며, 반드시 출처를 남겨주시기 바랍니다.

> “버그는 끝이 없고, 실험은 멈추지 않는다.”
