# Procedural Animals 절차적 동물 24종 코드 (three.js)

three.js용 완전 절차적 동물 24종입니다. SDF로 몸을 조각하고 자동 리그·듀얼 쿼터니언 스킨을 적용하며, 털·깃털·비늘을 입히고 IK 보행·액션으로 움직입니다. 모델 파일, 텍스처, 애니메이션 클립이 전혀 없이 전부 코드로 생성됩니다. `createAnimal('wolf')` 한 줄로 씬에 추가하고 이동·추적·액션을 지시할 수 있습니다.

**라이선스: MIT** (Copyright (c) 2026 Majid Manzarpour and procedural-animals contributors). 재배포 시 저작권 표기와 MIT 전문 유지가 조건입니다.

- 출처: https://github.com/majidmanzarpour/threejs-procedural-animals (HEAD c95ae49) · 쇼케이스: https://majidmanzarpour.github.io/threejs-procedural-animals/
- 수집일: 2026-11-23 · 파일: procedural-animals-threejs.zip (1.2MB)
- 의존: three >=0.160 (피어 의존, 미번들, MIT)
- 구성: src/(코어 빌드·수학·모션·렌더·리그·SDF + 24종 species 모듈, JS 239파일 + 타입 선언), tools/bake.mjs(.animal 베이크 CLI), docs/AUTHORING.md, README, LICENSE, llms.txt, package.json
- 종: bear, boar, cat, cheetah, chicken, cow, crow, deer, dog, eagle, fish, fox, frog, goat, horse, lion, pig, rabbit, rat, shark, sheep, snake, spider, wolf (6바디플랜: paws·hooves·birds·swimmers·snakes·spiders, 품종·암수·어린 개체 지원)
- 품질 단계: hero(~120k 버텍스) ~ crowd(~6k, 드로콜 1개) 5단계; 시드로 개체 재현 가능; Web Worker 빌드·오프라인 베이크 지원
- 검증: 2026-11-23 Node 22에서 `node tools/test.mjs` 24종 전량 통과, bake 6종 라운드트립 검증 통과 (샘플: assets-3d-lowpoly-2 procedural-animal-samples)
- 미리보기: 베이크 개체 6종 실제 렌더(헤드리스 크롬 WebGL, 늑대·말·독수리·상어·뱀·거미)
