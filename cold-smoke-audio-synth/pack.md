# Cold Smoke WebAudio 음악·효과음 합성 코드

스키 게임 Cold Smoke의 오디오 모듈 2개입니다. 녹음 음원 파일 없이(원본 저장소에 오디오 파일 0개) 바람·활주·엣지·눈 삐걱임 효과음과, 게임 상황을 따라가는 5레이어 생성형 배경 음악을 실행 중에 합성합니다.

**라이선스: MIT (Copyright (c) 2026 Huisky).** 저작권 표기와 MIT 전문을 유지하면 사용할 수 있습니다(동봉 LICENSE.txt).

## 내용 (zip, JS 4파일 + 문서)

- `18_sound.js` — 물리 기반 효과음 합성(바람·활주·엣지·눈 삐걱임·착지 등; 소스 노이즈는 최초 1회 합성)
- `18b_music.js` — 90bpm 5레이어 생성형 어댑티브 스코어(속도·엣지·시간대·점프에 반응, A 장조 고정 음계)
- `core/00_util.js`, `core/00b_variants.js` — 실행 의존 모듈(동일 원본·동일 MIT)
- `INTEGRATION.md` — 원본 게임과의 결합 지점과 어댑터 가이드
- `LICENSE.txt` — MIT 전문 (Copyright (c) 2026 Huisky)

## 확인한 것 / 확인하지 못한 것

- **확인(2026-11-24, 소스 판독)**: 외부 네트워크·파일 참조 없음(의존은 동봉 core 2종과 Web Audio API뿐); 녹음 음원 미사용; Variants 없이도 가드로 동작.
- **미확인**: 브라우저 단독 실행과 다른 게임 연결은 검증하지 않았습니다. Sound는 원본 게임 상태를 매 프레임 읽는 구조라 어댑터가 필요하고(INTEGRATION.md 참조), Music은 상대적으로 독립적입니다. 완성 에셋이 아니라 통합 작업이 필요한 코드 모듈입니다.

## 활용 메모

- 겨울·설상·스피드감 있는 게임의 환경음·효과음 레시피로 바로 참고할 수 있습니다(노이즈 합성 파라미터가 원 주석에 계량 기록).
- 출처: https://github.com/huiskylabs/cold-smoke (원본, MIT) · 한글 포크: https://github.com/sigco3111/cold-smoke (수록 파일은 원본과 바이트 동일)
- 수집일: 2026-11-24 · 파일: cold-smoke-audio-synth.zip
