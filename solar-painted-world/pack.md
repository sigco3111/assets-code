# Solar 절차적 행성 월드 코드

Solar(https://patch.gg/games/blendi/solar)의 '그린' 소행성 월드 전체를 만드는 코드입니다. 대기 산란 하늘, 지형, 풀, 나무, 꽃, 호수, 달, 별, 태양계와 행성 위 걷기까지 모두 코드로 그립니다(외부 텍스처·모델 없음).

**라이선스: MIT (코드).** 동봉 LICENSE.txt와 저작권 표기(Copyright (c) 2026 Patch)를 유지하세요.

## 내용 (zip, `src/`)
- page.js 대기 합성 최종 렌더 설계 · sky.js 하늘 · air.js 대기·날씨·조명
- land.js 지형 · grass.js 풀 · trees.js 나무 · flowers.js 꽃 · water.js 호수 · moon.js 달(크레이터)
- world.js·system.js 세계·태양계(자전·공전) · noise.js · shape.js · paint.js 붓질 질감 · motes.js 공중 먼지
- cover.js 나무 그림자 커버맵(태양 방향 스캔라인 그림자) · walker.js 구형 행성 표면 걷기(방위 유지)

## 활용 메모
- 게임과 결합된 참고용 원본. 모듈끼리 import하며 three(npm)가 필요합니다. 단독 실행 미검증.
- 출처: https://patch.gg/games/blendi/solar · 수집일: 2026-11-27
