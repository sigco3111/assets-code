# Lowpoly Tree Generator 코드

파라미터 기반 Three.js 로우폴리 나무 생성기입니다. 트렁크·버티스 뿌리·1차/2차 가지를 CSG로 용접하고 클러스터 캐노피를 붙여 버텍스 컬러 단일 지오메트리를 만듭니다. 아키타입 6종(ancientGuardian, windCrownedSentinel, weepingLantern, forkedShrine, stormClaw, groveBloom), 덩굴(vines) 옵션, 리그·애니메이션 프리셋, GLB 내보내기 경로를 포함합니다. 프로덕션 코어(Rand Monster Tree Forge의 오픈소스 코어)입니다.

**라이선스: MIT** (Copyright (c) 2026 Rand Monster contributors). 재배포 시 저작권 표기와 MIT 전문 유지가 조건입니다.

- 출처: https://github.com/pajama-studio/lowpoly-tree-generator · 업스트림(패키지 메타데이터 기준): https://github.com/rand-monster/lowpoly-tree-generator (동일 HEAD 4377dd6)
- 수집일: 2026-11-23 · 파일: lowpoly-tree-generator.zip (43KB)
- 의존: three >=0.179 (테스트 0.185.x), three-bvh-csg 0.0.18, three-mesh-bvh 0.9.7 (모두 MIT, THIRD_PARTY_NOTICES.md 동봉)
- 구성: src/ 7개 모듈, examples/, test/ (node --test 21개 통과, 2026-11-23 확인), package.json, README/LICENSE/CREDITS/THIRD_PARTY_NOTICES
- 검증: 2026-11-23 Node 22에서 테스트 전량 통과, 아키타입 6종 GLB 내보내기 성공 (샘플: assets-3d-lowpoly-2 lowpoly-tree-samples)
