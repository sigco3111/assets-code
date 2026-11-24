# Dead Precinct WebAudio 합성 효과음 26종·음악 3곡 코드

PS1 스타일 서바이벌 호러 「DEAD PRECINCT」의 오디오 엔진입니다. 녹음 음원 없이 Web Audio API만으로 전량 실시간 합성합니다.

**라이선스: MIT** (Copyright (c) 2026 Bao5ye). 재배포 시 저작권 표기와 MIT 전문 유지가 조건입니다. 원작 README는 음악·효과음을 모두 자작 합성이라고 명시합니다.

## 내용 (engine/audio.js, 약 75행 발췌)

- **효과음 26종** (`sfx` 객체): shot(무기 3종 변형)·step·moan·snarl·scream·hurt·bite·slash·screech·skitter·roar·thud·slam·creak·glass·pick·click·heal·die(개체 3종 변형)·sting·heart·thunder·drip·bang·alarm·power. 포먼트 보컬(voice: sawtooth+밴드패스 3단+노이즈 호흡), 노이즈 버스트, 서브 사인 드롭, 금속성 스팅 조합.
- **생성형 음악 3곡**: dread(탐색, 60bpm, 불협화 저음 패드+무작위 벨), safe(세이프룸, 66bpm, 코드 아르페지오), boss(140bpm, 킥·베이스 시퀀스). `seq`/`tick` 룩어헤드 스케줄러.
- **공간·연출**: 컨볼버 리버브(절차적 IR 2.8초), 음악 덕킹(duck), 방별 환경음 루프(setAmb 6종), 저체력 심장박동, 무작위 이벤트 스팅.

- 출처: https://github.com/Bao5ye/dead-precinct (원작 commit 3292dc6) · 한글판: https://github.com/sigco3111/dead-precinct-ko
- 수집일: 2026-11-24 · 파일: dead-precinct-audio-synth.zip
- 상태: 게임 결합 원본 발췌(참고용). 통합 방법은 INTEGRATION.md 참조. 브라우저 단독 실행 미검증.
