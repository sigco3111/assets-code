# Small Magic 주문 VFX·초원 월드 코드 (Three.js)

Patch의 Small Magic(https://patch.gg/games/blendi/small-magic) 소스에서 주문 이펙트와 초원 월드 코드를 모은 팩입니다. 모든 그래픽이 코드로 그려지며 외부 텍스처·모델이 없습니다.

**라이선스: MIT (코드).** 저작권 표기(Copyright (c) 2026 Patch)와 MIT 전문을 유지하면 사용할 수 있습니다(동봉 LICENSE.txt).

## 내용 (zip, `src/`)

- spells.js 시전 로직(불·냉기·바람·성장·폭발·특이점·토네이도·시간)
- fire.js flames.js billows.js fx.js 번지는 불, 불꽃, 폭발 연기, 파티클
- blast.js hole.js twister.js 폭발·블랙홀·토네이도
- time.js 시간 정지·되감기(세계 상태 기록과 복원)
- wall.js stroke.js sigil.js staff.js 돌벽, 번개, 룬 서클, 지팡이
- grass.js air.js noise.js shape.js paint.js page.js 풀, 공기, 노이즈, 도형, 페인트 마감, 마무리 패스
- meadow/world.js 초원 월드

## 활용 메모

- 게임과 결합된 원본이라 player.js, structures.js, physics/(destruction 팩) 등을 import 합니다. 모듈 단위로 떼어 쓰는 참고용입니다.
- 의존: three (npm). 원작은 three 0.186.1.
- 제외: Mixamo 마법사·동작, Sonniss GDC 녹음(재배포 금지), AI로 그린 UI 이미지.
- 출처: https://patch.gg/games/blendi/small-magic · 수집일: 2026-11-27
