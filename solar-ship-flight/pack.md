# Solar 우주선 비행·자동조종·조종석 코드

Solar(https://patch.gg/games/blendi/solar)의 우주선 비행 코드입니다. 관성 그대로 미끄러지는 뉴턴 비행, 목표 세계 고정·자동조종·속도 맞추기, 조종석 책상(다이얼·착륙 글라스)을 다룹니다.

**라이선스: MIT (코드).** 동봉 LICENSE.txt와 저작권 표기(Copyright (c) 2026 Patch)를 유지하세요.

## 내용 (zip, `src/`)
- ship.js 선체 거동·추력·착륙 다리·충돌
- pilot.js 세계 고정(lock)·자동조종·속도 맞추기·접근 정보
- desk.js 조종석 책상: 다이얼, 접근·거리 표시, 착륙 글라스(지면 투시)
- input.js 키보드·마우스·게임패드 통합 입력(아날로그 트리거·스틱)

## 활용 메모
- 게임과 결합된 참고용 원본. three(npm) 필요, 단독 실행 미검증.
- 출처: https://patch.gg/games/blendi/solar · 수집일: 2026-11-27
