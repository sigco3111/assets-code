# assets-code

재사용 가능한 게임 코드 모듈 (렌더링·이펙트·캐릭터 도구·합성음향 엔진 등). 소스 코드 형태 팩.
전체 목록·라이선스·귀속: [game-asset-catalog](https://github.com/sigco3111/game-asset-catalog/blob/main/catalog.csv)

## 수록 팩

### Starember Field Render Modules
- 파일: `starember-field-render/starember-field-render.zip` (TypeScript 9개: 툰 셰이딩·외곽선, 昼夜 하늘, 물, 풀, 파티클 이펙트, 지형·노이즈, 지오메트리·수학 유틸)
- 제작: weit0529 / 라이선스: MIT / 원본: https://github.com/weit0529/gamedemo_by_Fable5.2
- 비고: 코드 전용. 원본 LICENSE 제외 대상(설정그림·아바타·회사 로고) 미포함

### Starember Field Procedural Character Toolkit
- 파일: `starember-field-char-toolkit/starember-field-char-toolkit.zip` (TypeScript 9개: 절차적 캐릭터 파츠·리그·스프링본·애니메이션·표정 텍스처)
- 제작: weit0529 / 라이선스: MIT / 원본: https://github.com/weit0529/gamedemo_by_Fable5.2
- 비고: 범용 기구만 수록. 특정 캐릭터 조립(roster.ts)·회사 엠블럼(logos.ts)은 권리 문제로 미수록

### Everyday Game 라이더·드리프트 절차적 3D 코드
- 파일: `everyday-game-rider-3d/14-everyday-game-rider-3d.zip` (JavaScript 7개: Three.js 절차적 도시·차량·스쿠터 라이더·신호등·날씨 셰이더, 차량 생성기 makeCar)
- 제작: zhgarylu / 라이선스: 알 수 없음 / 원본: https://github.com/zhgarylu/everyday-game
- 비고: 원작·포크 모두 LICENSE 없음(2026-11-20 확인). 재사용 허락 미확인, 사용 전 원작자 확인 필요. 권리자 요청 시 즉시 내림

### Everyday Game 절차적 3D 코드 11종 (Three.js)
- 파일: `everyday-game-canvas-2d/34-everyday-game-canvas-2d.zip` (JavaScript 11개: 방어탑 9종·전동차·노점·거위·가구 등 Three.js 절차적 3D, 캔버스 2D는 텍스처 생성용)
- 제작: zhgarylu / 라이선스: 알 수 없음 / 원본: https://github.com/zhgarylu/everyday-game
- 비고: 원작·포크 모두 LICENSE 없음(2026-11-20 확인). 재사용 허락 미확인, 사용 전 원작자 확인 필요. 권리자 요청 시 즉시 내림

### Cadle WebAudio 합성 음향 엔진
- 파일: `cadle-webaudio-synth/cadle-webaudio-synth.zip` (JavaScript 5개: 합성 기본기 synth.js, 총기·폭발 전량 합성 레시피 sfx.js, 생성 악곡 music.js, 환경음 ambient.js, 엔진 Audio.js)
- 제작: Ian Cadle (Humpalumps) / 라이선스: MIT / 원본: https://github.com/Humpalumps/Cadle
- 비고: 녹음 음원 없이 모든 음향을 실행 중 합성. 원작 NOTICE의 녹음 테이크(재배포 금지)는 미포함, 코드만 MIT로 수록

### Klarbase 절차적 섬 월드 생성 코드
- 파일: `klarbase-procedural-world/klarbase-procedural-world.zip` (JavaScript 14개: 월드·지형·바이옴·나무·소품·동물 절차적 생성, 약 3,500행)
- 제작: TanmoyP and Klarbase contributors / 라이선스: MIT / 원본: https://github.com/TanmoyP/klarbase
- 비고: 모델·텍스처·오디오 파일 없이 코드로 섬 월드를 생성(원작 README 확인). 게임 결합 상태 참고용

### Lowpoly Tree Generator 절차적 나무 생성 코드
- 파일: `lowpoly-tree-generator/lowpoly-tree-generator.zip` (JavaScript 7모듈: CSG 용접 트렁크·뿌리·가지, 클러스터 캐노피, 아키타입 6종, 덩굴 옵션, GLB 내보내기)
- 제작: Rand Monster contributors / 라이선스: MIT / 원본: https://github.com/pajama-studio/lowpoly-tree-generator
- 비고: three·three-bvh-csg·three-mesh-bvh 의존(모두 MIT). node --test 21개 통과(2026-11-23). 생성 샘플은 assets-3d-lowpoly-2 lowpoly-tree-samples

### Geometry Painter 표면 페인팅·절차적 3D 코드
- 파일: `geometry-painter-threejs/geometry-painter-threejs.zip` (TypeScript 24개: 표면 스트로크 페인팅 모드 시스템, 크리스탈·용암균열·오로라·발광산호 4모드, BVH 피킹·리샘플·컬링 배관, 단일 메커니즘 데모 10종)
- 제작: mohamedachrefelouafi / 라이선스: MIT / 원본: https://github.com/achrefelouafi/GeometryPainterThreeJS
- 비고: 모델·텍스처 없는 코드 전용(WebGPU, WebGL2 폴백). npm run build 통과, WebGL2 렌더 확인(2026-11-23)

### Procedural Animals 절차적 동물 24종 코드 (three.js)
- 파일: `procedural-animals-threejs/procedural-animals-threejs.zip` (JavaScript 239파일 + 타입 선언: SDF 몸 조각·자동 리그/스킨·털/깃털/비늘·IK 보행/액션, 24종 6바디플랜, bake CLI 포함)
- 제작: Majid Manzarpour and procedural-animals contributors / 라이선스: MIT / 원본: https://github.com/majidmanzarpour/threejs-procedural-animals
- 비고: 모델·텍스처·애니메이션 클립 없는 코드 전용(실행 시 생성). node tools/test.mjs 24종 통과(2026-11-23). 베이크 샘플 6종은 assets-3d-lowpoly-2 procedural-animal-samples

### Elemental Sandbox 스킬 VFX 코드 모듈 (Three.js·GLSL)
- 파일: `elemental-sandbox-ability-vfx/elemental-sandbox-ability-vfx.zip` (JavaScript·GLSL src 전체(archive 제외): 스킬 7종(Pyre·ElectricalSphere·Portal·FirePortal·Kraken·Earth·AetherRing)·기반/매니저·GLSL 머티리얼 17종·이펙트/파티클 라이브러리)
- 제작: mohamedachrefelouafi / 라이선스: MIT / 원본: https://github.com/achrefelouafi/LinearAbilityExtThreeJS
- 비고: 참고용 원본 코드. MIT 전문 동봉. Mixamo FBX·diffuse.png(재배포 금지), textures.glb(출처 불명)는 제외

### Ultra Elements 원소 주문 VFX 코드 39종 (Three.js·WebGL2)
- 파일: `ultra-elements-spell-vfx/ultra-elements-spell-vfx.zip` (JavaScript/GLSL: 원소 주문 29모듈·폼 포함 39종, FLIP 유체·연소 솔버·레이마칭 볼륨·중력 렌즈, elements.js 어댑터, spells.json 411설정)
- 제작: Humpalumps (Ultra Elements), 데모 어댑트: Patch / 라이선스: MIT / 원본: https://github.com/Humpalumps/ultra-elements
- 비고: 텍스처·모델·사운드 없이 전량 코드 생성. three 0.186.1 고정, 주문 로딩은 Vite import.meta.glob. MIT 전문 동봉

### AbilityCasting 시네마틱 주문 VFX 코드 9종 (Three.js·GLSL)
- 파일: `abilitycasting-spell-vfx/abilitycasting-spell-vfx.zip` (JavaScript·GLSL src 전체(archive 제외): 주문 9종(Abyssal Maw·Chains of Penance·Dragonfire Circle·Stormheart Gyroscope·Amethyst Verdict·Astral Tome·Wildroot Reliquary·Starbreaker Lance·Astral Fang)·기반/매니저·GPU 파티클·GLSL 머티리얼·래그돌·포스트 체인·조준 인디케이터·VFX 에디터)
- 제작: mohamedachrefelouafi / 라이선스: MIT / 원본: https://github.com/achrefelouafi/AbilityCastingThreeJS
- 비고: 참고용 원본 코드. MIT 전문 동봉. Mixamo FBX·diffuse.png(재배포 금지), Sketchfab 모델 dragon·gyroscope(원라이선스 불명), 출처 미확인 텍스처는 제외. npm run build 통과(2026-11-23). 자작 모델은 assets-3d-lowpoly-2 abilitycasting-models

### 00GameDevs 마법 VFX Starter 5종 (Three.js·WebGL2)
- 파일: `00gamedevs-vfx-starter/00gamedevs-vfx-starter.zip`
- 제작: 00GameDevs (@00vchannel) / 라이선스: MIT / 원본: https://patch.gg/00vchannel/00gamedevs-vfx-starter
- 비고: 마법 VFX 5모듈 원본: 암흑 사슬 폭발·공간 참격·블랙홀·황금 사슬 비·성유물 강림. 외부 텍스처·모델·음원 없음. three 0.187.0/WebGL2 필요. MIT 고지·통합 가이드·SHA256 매니페스트·실행 샘플 동봉. npm build 및 5종 렌더/생명주기 확인. Patch helper·브랜드·게임 아트 제외. 모바일 성능 미검증.

### Long Wind 절차적 환경 생성 코드 (Three.js)
- 파일: `long-wind-env-gen/long-wind-env-gen.zip` (JavaScript 70파일: 지형·풀·죽림·마을·하늘·날씨 절차적 생성, world+levels+fx+core)
- 제작: jbang2004 / 라이선스: MIT / 원본: https://github.com/jbang2004/long-wind (한글판: https://github.com/sigco3111/long-wind)
- 비고: 모델·텍스처 없이 환경 전량을 코드로 생성. 캐릭터·전투·UI 코드와 검술 포즈 데이터는 제외. world/citizens.js(군중 배치)는 제외된 character 모듈 의존으로 미수록. 나머지 모듈 import는 팩 안에서 닫히고 외부 의존은 three.js뿐. MIT 전문 LICENSE.txt 동봉. 참고용 원본 코드

### Long Wind WebAudio 음악·효과음 합성 코드
- 파일: `long-wind-audio-synth/long-wind-audio-synth.zip` (JavaScript 17파일: 합성 엔진·전통 악기 톤·생성 악곡·검술 효과음·환경음·날씨음·군중·음성·IR + 실행 의존 core 5종)
- 제작: jbang2004 / 라이선스: MIT / 원본: https://github.com/jbang2004/long-wind (한글판: https://github.com/sigco3111/long-wind)
- 비고: 녹음 음원 없이 전량 합성(원작 저장소 오디오 파일 0개). 실행에 필요한 core 모듈 5종(bus·globals·wind·noise·glsl, 모두 MIT)을 core/에 동봉. 외부 의존은 three.js(audio.js)뿐. MIT 전문 LICENSE.txt 동봉. 참고용 원본 코드
