# Lighthouse Cup OKLab 90색 디더링 픽셀 후처리 코드

고정 90색 팔레트를 OKLab 공간에서 가장 가까운 색으로 맞추는 Three.js r128 후처리 패스입니다. 4x4 Bayer 순서 디더링, 깊이 텍스처 기반 윤곽선, 저해상도 렌더 타깃(픽셀 크기 조절), 절차적 하늘 셰이더(별·시간·요 회전)를 포함합니다.

**라이선스: MIT** (Copyright (c) 2026 Aizzul Luqman). 재배포 시 저작권 표기와 MIT 전문 유지가 조건입니다.

- 내용: engine/dither.js (약 343행, 원작 영문판 발췌)
- 출처: https://github.com/itsLucas02/lighthouse-cup · 한글판: https://github.com/sigco3111/lighthouse-cup-ko
- 수집일: 2026-11-26 · 상태: 단일 index.html에서 잘라낸 발췌(참고용). 이 팩 단독으로 브라우저 실행은 검증하지 않았습니다. 통합 방법은 INTEGRATION.md 참조.
- 원작 README의 제작자 표기: gemini-4-carbon (별도 확인하지 않음).
