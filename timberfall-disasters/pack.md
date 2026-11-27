# Timberfall 재해 시스템 코드 (토네이도·화재·지진·날씨, three.js, MIT)

Timberfall(https://patch.gg/games/blendi/timberfall)의 재해 시스템 TypeScript입니다. 토네이도, 화재 확산,
지진, 비·바람 날씨, 노출(폭풍 노출도)이 물리 구조물과 상호작용하며 건물을 무너뜨립니다.

**라이선스: MIT.** 동봉 LICENSE.txt와 저작권 표기(Copyright (c) 2026 Patch)를 유지하세요.

## 내용 (zip, `src/disasters/`)

- `tornado.ts` 토네이도 흡입·파괴 (287줄), `fire.ts` 화재 점화·확산 (449줄)
- `quake.ts` 지진 (191줄), `weather.ts` 비·바람 (153줄)
- `exposure.ts` 폭풍 노출도 (214줄), `field.ts` 힘 장 (268줄), `index.ts` 통합 (165줄)

## 활용 메모

- 원작의 물리(three-avbd)와 구조물 시스템에 결합된 참고용 원본. 물리 엔진은 카탈로그
  `small-magic-destruction` 팩에 벤더링 사본이 있습니다. three.js 필요, 단독 실행 미검증.
- 출처: https://patch.gg/games/blendi/timberfall · 수집일: 2026-11-27
