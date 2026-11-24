# Cold Smoke 절차적 인체 생성 코드 (Human)

스키 게임 Cold Smoke의 `human/` 모듈입니다. 모델 파일·텍스처 없이 **코드만으로 사람 몸을 생성**합니다: 성별·키·체중·체지방·골격 입력 → 59본 스켈레톤(VRM/Unity Humanoid 상위집합) → 34근육 볼륨 몸통 → 서피스넷 메쉬 → LBS/DQS 스키닝 → 모션 클립. 모듈 헤더에 "게임 전역을 읽지 않으며 어떤 페이지에도 넣을 수 있다"고 명시된 독립 모듈이며, 모든 것이 하나의 전역 `Human` 아래에 있습니다.

**라이선스: MIT (Copyright (c) 2026 Huisky).** 저작권 표기와 MIT 전문을 유지하면 사용할 수 있습니다(동봉 LICENSE.txt). 09a_refdata.js에 포함된 MakeHuman 베이스 메쉬는 CC0 1.0(공식 확인, NOTICE.md 참조).

## 내용 (zip, human/src JS 11파일 + 빌드 스크립트)

- `00_math.js` 벡터·쿼터니언·swing-twist
- `01_params.js` 체형 파라미터 → ANSUR II 회귀 신체 치수
- `02_skeleton.js` 59본 스켈레톤·관절 가동범위·해부학 포즈
- `03_body.js` 로프트 단면 몸통 + 근육 볼륨
- `04_mesh.js` 바인드 포즈 서피스넷 메쉬·법선·체적
- `05_measure.js` 둘레 측정·ANSUR 피팅
- `06_skin.js` LBS·DQS·투영 스키닝
- `07_poses.js` 스트레스 포즈·지면 정렬
- `08_motion.js` 모션 클립(걷기·턱·모굴 등 12종)
- `09_refbody.js` + `09a_refdata.js` MakeHuman CC0 참조 몸(연구용, 없어도 동작)
- `build-module.js` → `human/dist/human.js` 단일 파일 생성(원본 대비 모캡 내장 단계 생략)

## 확인한 것 / 확인하지 못한 것

- **확인(2026-11-24, Node 22 단독 실행)**: 기본 체형으로 몸 생성 → 메쉬 12,986정점/25,976삼각형, 체적 69.3L(75kg 기준 타당); 모션 클립 12종 샘플링 성공; MakeHuman 참조 몸(13,380정점) 해석·스켈레톤 적용 성공. 외부 네트워크·파일 참조 없음.
- **미확인**: 브라우저에서의 렌더링·실제 게임 연결(스키닝 GPU 업로드, 애니메이션 루프 통합)은 다른 게임에 붙여 보지 않았습니다. 완성 에셋이 아니라 통합 작업이 필요한 코드 모듈입니다.

## 활용 메모

- 출처: https://github.com/huiskylabs/cold-smoke (원본, MIT) · 한글 포크: https://github.com/sigco3111/cold-smoke (수록 파일은 원본과 바이트 동일)
- 모듈 설명·연구 근거: 원본 저장소 human/README.md
- 수집일: 2026-11-24 · 파일: cold-smoke-human-body.zip
