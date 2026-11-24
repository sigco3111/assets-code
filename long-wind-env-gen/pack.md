# Long Wind 절차적 환경 생성 코드 (Three.js)

수묵 무협 게임 Long Wind에서 지형·풀·죽림·마을·하늘·날씨를 로드 시점에 전부 절차적으로 생성하는 코드 모듈입니다. 에셋 파일 없이 산·초원·대나무숲·기와마을·하늘·비·폭풍을 만드는 완전 경로로, 다른 게임의 환경 생성에 가져다 쓰기 가장 좋은 부분입니다.

**라이선스: MIT (Copyright (c) 2026 jbang2004).** 저작권 표기와 MIT 전문을 유지하면 사용할 수 있습니다(동봉 LICENSE.txt).

## 내용 (zip, JS 71파일)

- `world/` — 지형(terrain·bake·worker·pool), 풀(grass·glsl), 죽림·수목·화초(trees·flora·flowers·foliage·bamboo), 마을(town·town-arch·geo·mat), 하늘(sky), 바위 배치(rocks·lod·plan), 소품(props·pavilion·stone·carve), 지형 그림자·군집(layout·chunks·shadows·plumes·mountains)
- `levels/` — 초원·죽림·마을 레벨 구성(steppe·bamboo·town·runtime)
- `fx/` — 날씨·파티클(rain·storm·particles·vfx·ambient·soft·trail·common)
- `core/` — 노이즈·바람·대기·포스트 파이프라인(noise·wind·atmosphere·glsl·post*)
- `LICENSE.txt` — MIT 전문 (Copyright (c) 2026 jbang2004)

## 활용 메모

- 원본 게임 결합 상태의 참고용 코드로, 모듈 간 의존이 있습니다. 생성기 단위로 떼어 쓰는 용도에 적합합니다.
- 캐릭터·전투·UI 코드와 참고영상 기반 검술 포즈 데이터(src/character/mocap/jian-demo.js)는 팩에서 제외했습니다.
- 출처: https://github.com/jbang2004/long-wind · 한글판: https://github.com/sigco3111/long-wind
- 수집일: 2026-11-24 · 파일: long-wind-env-gen.zip
