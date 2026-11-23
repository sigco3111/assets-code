# Ultra Elements 원소 주문 VFX 코드 39종 (Three.js·WebGL2)

Ultra Elements(Humpalumps)의 원소 주문 39종과 그것을 게임용으로 감싼 Patch의 elements.js 어댑터입니다. 번개·불·물·얼음·대지·바람·공허·빛·산성·비전 10속성 + 혼합 3종. 텍스처·모델·사운드 없이 모든 것을 코드로 그립니다(GPU 입자, 물·산성 FLIP 유체, 불·연기 연소 솔버, 레이마칭 볼륨, 번개, 중력 렌즈, 바닥 반응 필드).

**라이선스: MIT (코드).** 저작권 표기와 MIT 전문을 유지하면 사용할 수 있습니다(동봉 LICENSE.txt — Patch 어댑트 부분, LICENSE-ultra-elements.txt — Humpalumps 원본).

## 내용 (zip)

- `elements.js` — 프레임 전체를 그리는 래퍼: `createElements({renderer, camera, sky})`, `cast(name, point, {from, target, held})`, `pick(x,y)`, `setParam`, `setSky`, `warmAll`, `autoQuality` 등 (Patch, MIT)
- `lib-ultra-elements/` — 주문 29개 모듈(폼 포함 39종)과 엔진(입자·유체·볼륨·후처리·훈련장), 저작자 문서 README/SPELLBOOK/CONTRIBUTING 포함 (Humpalumps, MIT)
- `spells.json` — 39종 전체의 설정 411개(기본값·범위)와 프리셋 3종씩
- `tuning.js` — 크기·강도 등 공통 조절을 각 주문 설정으로 매핑
- `LICENSE.txt`, `LICENSE-ultra-elements.txt`, `THIRD_PARTY_NOTICES-ultra-elements.md`

## 활용 메모

- three.js 0.186.1에 맞춰져 있고, 주문 로딩은 Vite의 `import.meta.glob`을 씁니다(다른 번들러는 로더 교체 필요).
- 새 주문은 모듈 하나 복사로 추가 가능(`lib-ultra-elements/src/spells/_template.js`, SPELLBOOK.md에 아이디어 80여 개).
- 주문은 y=0 평지, 중심에서 18m 이내를 기준으로 설계돼 있습니다.
- 한국어 데모(설정 패널 포함): https://sigco3111.github.io/elements-ko/ · 원본 데모: https://patch.gg/patch/elements
- 수집일: 2026-11-23 · 파일: ultra-elements-spell-vfx.zip
