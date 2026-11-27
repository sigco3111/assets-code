# Timberfall 합성 사운드 엔진 (WebAudio, MIT)

Timberfall(https://patch.gg/games/blendi/timberfall)의 소리 코드입니다. 그라인더, 발소리, 도구 휘두르기,
경보, UI 소리와 믹스 전체를 WebAudio로 합성합니다.

**라이선스: MIT.** 동봉 LICENSE.txt와 저작권 표기(Copyright (c) 2026 Patch, 일부 Steven Bobyn)를 유지하세요.

## 내용 (zip)

- `src/audio/sounds.ts` 소리 합성·레이어·믹스 전체 (1,350줄)

## 활용 메모

- 원작은 Sonniss GDC 녹음 98개를 추가 층으로 입히지만 재배포 금지 라이선스라 제외했습니다.
  코드는 그 파일들이 없어도 동작합니다(404는 건너뜀, LAYERS 구조 참고).
- three-voxel-destruction에서 Brickfall을 거쳐 온 사운드 믹스 포함(Steven Bobyn + Patch, MIT).
- 출처: https://patch.gg/games/blendi/timberfall · 수집일: 2026-11-27
