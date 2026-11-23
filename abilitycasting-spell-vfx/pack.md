# AbilityCasting 시네마틱 주문 VFX 코드 9종 (Three.js·GLSL)

AbilityCastingThreeJS(Elemental Sandbox)의 시네마틱 주문 VFX 코드 원본입니다. 주문 9종(Abyssal Maw·Chains of Penance·Dragonfire Circle·Stormheart Gyroscope·Amethyst Verdict·Astral Tome·Wildroot Reliquary·Starbreaker Lance·Astral Fang)과 Ability 기반 클래스·매니저, GPU 파티클 엔진, 전용 GLSL 머티리얼, 래그돌·전투 더미, 깊이 프리패스·화면 왜곡·ACES 포스트 체인, 지면 조준 인디케이터, 실시간 VFX 에디터(lil-gui)를 포함합니다.

**라이선스: MIT (코드).** 저작권 표기와 MIT 전문을 유지하면 사용할 수 있습니다(동봉 LICENSE.txt, Copyright (c) 2026 mohamedachrefelouafi).

## 내용 (zip)

- `src/abilities/` — 주문 9종과 Ability 기반, AbilityManager
- `src/materials/` `src/shaders/` — GLSL 머티리얼·셰이더 라이브러리
- `src/effects/` — 조준 인디케이터, 데칼, 번개, 버스트, 카메라 연출
- `src/particles/` — GPU 파티클 시스템
- `src/combat/` — 전투 더미와 래그돌 솔버
- `src/postprocessing/` — 깊이 프리패스, 왜곡 버퍼, ACES·그레이드 컴포저
- `src/world/` `src/core/` `src/config/` `src/assets/` 등 — 참고용 원본
- `LICENSE.txt` — MIT 전문

## 제외 항목 (권리상 수록 불가)

- Mixamo 캐릭터 FBX 4종(Idle·cast1~3·dummy)과 `diffuse.png` — Mixamo 에셋은 재배포 금지
- `dragon.glb`, `magical_gyroscope.glb` — Sketchfab 서드파티 모델, 원라이선스 확인 불가
- cathedral·배너·스테인드글라스·룬 텍스처 — 출처 확인 불가
- `docs/screenshots/` — 원작자 스크린샷(팩 미리보기로만 사용)

## 활용 메모

- 게임 로직과 결합된 상태 그대로 수록한 참고용 원본입니다. Ability 기반 클래스 구조와 GLSL 셰이더는 그대로 옮겨 쓰기 좋습니다.
- 레거시 src/archive는 제외했습니다.
- 주문이 쓰는 자작 모델은 같은 원본의 모델 팩(assets-3d-lowpoly-2 abilitycasting-models)에 있습니다.
- npm 의존(three, lil-gui 등)은 미번들이라 `npm install`이 필요합니다. `npm run build`(vite) 통과 확인(2026-11-23).
- 출처: https://github.com/achrefelouafi/AbilityCastingThreeJS
- 수집일: 2026-11-23 · 파일: abilitycasting-spell-vfx.zip
