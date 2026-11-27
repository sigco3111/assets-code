# Small Magic 파괴 물리 코드

Small Magic(https://patch.gg/games/blendi/small-magic)의 "부서지는 건물" 코드입니다. 건물이 돌·들보·기와 조각으로 지어져 맞은 만큼 부서지고, 놓아주면 다시 쉬는 구조입니다.

**라이선스: MIT.** Patch 코드와 벤더링된 three-avbd(Steven Bobyn, MIT, 서드파티 고지 THIRD_PARTY_NOTICES.md 포함) 모두 MIT입니다. LICENSE와 고지를 유지하세요.

## 내용 (zip)

- `src/physics/` builder.ts, structure.ts, materials.ts: 조각으로 구조물 짓기와 용접 임계값
- `src/ruin.js` 파괴 처리, `src/structures.js` 마을 건물(성채·오두막·풍차·수도원) 구성
- `vendor/three-avbd/` AVBD 물리 엔진(원본 https://github.com/sbobyn/three-avbd, 커널 1개 변경은 VENDOR.md 참고)

## 활용 메모

- vite alias로 `three-avbd`와 `three-avbd/advanced`를 vendor 경로에 연결해야 합니다(원작 vite.config.mjs 참고).
- 참고용 원본, 단독 실행 미검증.
- 출처: https://patch.gg/games/blendi/small-magic · 수집일: 2026-11-27
