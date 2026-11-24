# Cold Smoke SDF 메쉬 생성 코드 (Surface Nets)

스키 게임 Cold Smoke의 `06_sdfmesh.js` 단일 파일입니다. 부호거리함수(SDF)로 나무·동물·스키어 같은 입체 형상을 수학식으로 모델링하고, 내로우밴드 서피스넷으로 삼각형 메쉬를 만듭니다. 외부 의존 0, 게임 전역 참조 0의 순수 수학 모듈입니다.

**라이선스: MIT (Copyright (c) 2026 Huisky).** 저작권 표기와 MIT 전문을 유지하면 사용할 수 있습니다(동봉 LICENSE.txt).

## 내용 (zip, JS 1파일 + 문서)

- `06_sdfmesh.js` — `sd`(SDF 라이브러리: 구·타원체·테이퍼 캡슐·둥근 상자·smin/smax), `meshSDF`(서피스넷 메셔), `meshBuilder`(파라메트릭 스윕 메쉬 빌더)
- `README-module.md` — API·반환 형식(정점당 float 10: 위치3+법선3+속성4)·사용 예
- `LICENSE.txt` — MIT 전문 (Copyright (c) 2026 Huisky)

## 확인한 것 / 확인하지 못한 것

- **확인(2026-11-24, Node 22 단독 실행)**: 구 3개+캡슐을 smin으로 블렌딩한 테스트 SDF → 메쉬 16,722정점/33,144삼각형, 455ms 생성(미리보기 이미지가 그 출력).
- **미확인**: WebGL/WebGPU 파이프라인으로의 업로드·렌더링은 다른 게임에 붙여 보지 않았습니다. 정점 레이아웃(10 floats)은 원본 게임의 커스텀 포맷이므로 자기 파이프라인에 맞게 읽어야 합니다.

## 활용 메모

- 출처: https://github.com/huiskylabs/cold-smoke (원본, MIT) · 한글 포크: https://github.com/sigco3111/cold-smoke (수록 파일은 원본과 바이트 동일)
- 수집일: 2026-11-24 · 파일: cold-smoke-sdf-mesher.zip
