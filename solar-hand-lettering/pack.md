# Solar 펜 스트로크 레터링·인쇄 코드

Solar(https://patch.gg/games/blendi/solar)의 문자 렌더링 코드입니다. 폰트 파일 없이 모든 글자를 펜 획 몇 개로 직접 그리고, 선박 안의 차트·카드·다이얼 면 인쇄물을 만듭니다.

**라이선스: MIT (코드).** 동봉 LICENSE.txt와 저작권 표기(Copyright (c) 2026 Patch)를 유지하세요.

## 내용 (zip, `src/`)
- hand.js 획 단위 손글씨 엔진(write/width, 게임 내 모든 문자 표기)
- prints.js 선박 인쇄물: 항해 차트, 카드, 이름, 다이얼 문자판
- words.js 키 안내 표기(검은 타일+키 이름, 상황별 조작 힌트)

## 활용 메모
- 게임과 결합된 참고용 원본. three(npm) 필요, 단독 실행 미검증. 영문 대문자 위주 획 데이터.
- 출처: https://patch.gg/games/blendi/solar · 수집일: 2026-11-27
