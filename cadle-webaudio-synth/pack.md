# Cadle WebAudio 합성 음향 엔진

3D 슈터 Cadle의 WebAudio 합성 음향 모듈 5개입니다. 녹음 음원 파일 없이 총성·폭발·이동·환경음·지역별 배경악곡을 전부 실행 중에 합성합니다. 원작 NOTICE가 밝히듯 녹음 테이크는 생성 서비스 약관(재배포 금지) 때문에 원작 레포에도 없고, 이 합성 경로가 실제 게임에서 들리는 음향입니다.

**라이선스: MIT(코드).** 저작권 표기와 MIT 전문을 유지하면 사용할 수 있습니다(동봉 LICENSE.txt, NOTICE.txt).

## 내용 (zip, JS 5개)

- `synth.js` — 합성 기본기: noise, tone, fm, click, echo, rnd, sample, drive, metal
- `sfx.js` — 무기·충격·폭발 레시피(라운드로빈·피치 지터·거리 감쇠·덕킹 설계 주석 포함)
- `music.js` — 지역별 생성 악곡
- `ambient.js` — 환경음
- `Audio.js` — 버스·리버브·파노라마를 묶는 엔진
- `LICENSE.txt` — MIT 전문 (Copyright (c) 2026 Ian Cadle)
- `NOTICE.txt` — 원작 NOTICE(에셋·녹음 권리 범위 설명)

## 활용 메모

- 게임 모듈과 결합된 상태 그대로 수록한 참고용 원본입니다. 합성 기본기(synth.js)와 레시피 구조는 그대로 옮겨 쓰기 좋습니다.

- 출처: https://github.com/Humpalumps/Cadle · 한글판 포크: https://github.com/sigco3111/cadle-ko
- 수집일: 2026-11-20 · 파일: cadle-webaudio-synth.zip
