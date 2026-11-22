# Geometry Painter 표면 페인팅·절차적 3D 코드

Three.js WebGPU(WebGL2 폴백) 기반 표면 페인팅 시스템입니다. 구 표면에 스트로크를 그으면 모드별 절차적 3D가 자랍니다. 모드 4종(크리스탈 군집, 용암 균열, 오로라 실크, 발광 산호 리프)이 같은 스트로크 입력을 공유하는 플러그인형 모드 시스템이 핵심이며, 공통 페인팅 배관(BVH 피킹, 앵커 공간, 스트로크 리샘플, 컬링, 성장 애니메이션)이 분리되어 있습니다. TSL 셰이더(흑체 열 램프, 주름 고정 밝기 등), 스튜디오 환경 라이팅, 블룸 후처리를 포함합니다.

**라이선스: MIT** (Copyright (c) 2026 mohamedachrefelouafi). 재배포 시 저작권 표기와 MIT 전문 유지가 조건입니다.

- 출처: https://github.com/achrefelouafi/GeometryPainterThreeJS (HEAD 79c7556)
- 수집일: 2026-11-23 · 파일: geometry-painter-threejs.zip (118KB)
- 의존: three ^0.185, lil-gui ^0.21, three-mesh-bvh ^0.9 (모두 MIT, THIRD_PARTY_NOTICES.md 동봉)
- 구성: src/ 10개 모듈(앱·표면페인터·BVH·UI + 모드 4종·모드 인터페이스), demos/ 단일 메커니즘 데모 10종(피킹·앵커공간·리샘플·컬·성장·리본·흑체·주름광·펄스·스튜디오), index.html, package.json, tsconfig, vite 설정, README/ARTICLE(기법 해설; 참조 gif는 원본 저장소에 없음)
- 코드 전용: 모델·텍스처·오디오 파일 없이 모든 지오메트리·재질을 코드로 생성
- 검증: 2026-11-23 Node 22에서 npm run build(tsc --noEmit 포함) 통과, WebGL2 백엔드 헤드리스 크롬 렌더 캡처 확인(미리보기 이미지)
- 미리보기: 크리스탈 모드 실제 렌더(검정 래커 구 + 자수정 크리스탈)
