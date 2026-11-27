# Don't Look Away 석조 예배당·천사 시야 판정 코드 (Three.js·TypeScript)

Patch의 Don't Look Away(https://patch.gg/games/blendi/dont-look-away) 소스(src/)입니다. TypeScript, three.js.

**라이선스: MIT.** 저작권 고지와 MIT 전문을 유지하면 사용할 수 있습니다(LICENSE.txt). 석재 셰이더·기둥·리브·포장은 Realistic Procedural Dungeons와 Dungeon Forge(Majid Manzarpour)에서 파생되었고 그 MIT 전문이 licenses/에 있습니다.

## 내용 (zip, `src/`)

- stone.ts, stonework.ts 석재 셰이더와 구조물, contact-shadows.ts 접촉 그림자
- flashlight.ts, illumination.ts 손전등과 조명 판정
- angels.ts, visibility.ts 보이는 동안 멈추는 천사, 반사까지 포함한 시야 판정
- temporal.ts, horror.ts, navigation.ts 시간·연출·길찾기
- audio.ts 코드로 합성하는 소리, power-cabinet.ts, world.ts 예배당 구성

## 활용 메모

- 게임과 결합된 원본이라 모듈 단위로 떼어 쓰는 참고용입니다. 단독 실행은 검증하지 않았습니다.
- 모델·텍스처·효과음은 들어 있지 않습니다(별도 팩).
- 출처: https://patch.gg/games/blendi/dont-look-away · 수집일: 2026-11-27
