# Elemental Sandbox 스킬 VFX 코드 모듈 (Three.js·GLSL)

LinearAbilityExtThreeJS(Elemental Sandbox)의 스킬 VFX 코드 원본입니다. 스킬 7종(Pyre·Electrical Sphere·Portal·Fire Portal·Kraken·Earth·Aether Ring)과 Ability 기반 클래스·매니저, 전용 GLSL 머티리얼 17종, 조준·범위 인디케이터 등 이펙트 모듈, 셰이더 라이브러리·파티클 엔진을 포함합니다.

**라이선스: MIT (코드).** 저작권 표기와 MIT 전문을 유지하면 사용할 수 있습니다(동봉 LICENSE.txt, Copyright (c) 2026 mohamedachrefelouafi).

## 내용 (zip)

- `src/abilities/` — Ability 기반, AbilityManager, 스킬 7종 구현
- `src/materials/` — GLSL 머티리얼 17종 (Pyre, Kraken, Ember, BodyArc, FresnelAura 등)
- `src/effects/` — 조준·범위 인디케이터, 버스트, 스크린플래시 등 연출 모듈
- `src/shaders/` `src/particles/` `src/utils/` — 셰이더 라이브러리·파티클·유틸
- 그 외 `src/core/` `src/world/` 등 — 참고용 원본
- `LICENSE.txt` — MIT 전문

## 제외 항목 (권리상 수록 불가)

- Mixamo 캐릭터 FBX 4종과 `diffuse.png` — Mixamo 에셋은 재배포 금지
- `textures.glb` — 출처 확인 불가
- `docs/screenshots/` — 원작자 스크린샷

## 활용 메모

- 게임 로직과 결합된 상태 그대로 수록한 참고용 원본입니다. 스킬 구조(Ability 기반 클래스 + 머티리얼 조합)와 GLSL 셰이더는 그대로 옮겨 쓰기 좋습니다.
- 레거시 src/archive는 제외했습니다.
- 출처: https://github.com/achrefelouafi/LinearAbilityExtThreeJS
- 수집일: 2026-11-23 · 파일: elemental-sandbox-ability-vfx.zip
