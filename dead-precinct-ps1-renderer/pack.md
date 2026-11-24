# Dead Precinct PS1 WebGL 렌더러 코드

PS1 스타일 서바이벌 호러 「DEAD PRECINCT」의 자체 WebGL1 렌더러입니다. 외부 라이브러리 없이 320×240으로 그리고 CRT 질감을 얹습니다.

**라이선스: MIT** (Copyright (c) 2026 Bao5ye). 재배포 시 저작권 표기와 MIT 전문 유지가 조건입니다.

## 내용 (engine/ps1-renderer.js)

- **셰이더**: 버텍스 스냅(160×120 그리드 지터), 어파인 텍스처 매핑(원근 보정 생략), 버텍스별 2점 조명+거리 감쇠, 지수 안개, 15비트 ordered 디더링(2×2 베이어).
- **절차적 표면 머티리얼 7종** (머티리얼 id 3~8): 벽돌·타일·목재 판자·콘크리트·금속 리브·천, 해시/밸류 노이즈 기반, 가장자리 AO와 바닥 그라데이션 포함.
- **지오메티 파이프라인**: vtx/quad/box 적재(단일 Float32Array 버퍼), 4×4 행렬·투영·뷰 유틸.
- **draw3**: 씬 드로 + 프리렌더 배경 합성. 배경을 `md=1` 모드로 깊이 테스트 없이 그린 뒤 컬러 마스크로 깊이만 먼저 쓰고 실시간 메시를 덧그리는 3패스 구조(고정 카메라 서바이벌 호러 방식).
- **CRT 마감**: 그레인, 라디얼 비네트(2D 오버레이 캔버스), CSS 스캔라인.

- 출처: https://github.com/Bao5ye/dead-precinct (원작 commit 3292dc6) · 한글판: https://github.com/sigco3111/dead-precinct-ko
- 수집일: 2026-11-24 · 파일: dead-precinct-ps1-renderer.zip
- 상태: 게임 결합 원본 발췌(참고용). 배경 텍스처 로더는 외부 PNG 경로 예시로 고쳐 둠(assets-2d-pixel `dead-precinct-backgrounds` 팩과 같은 이름). 캐릭터 로프트 메시 코드는 이 팩에 없음.
