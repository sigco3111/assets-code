# 00GameDevs 마법 VFX Starter 5종 (Three.js)

MIT 라이선스의 마법 이펙트 JavaScript 모듈 5개를 원본 그대로 수록했습니다.

- Darkchain Sigil Rupture: 암흑 구체·사슬·보라색 번개 폭발
- Rift-Shattering Slashes: 공간 균열 참격·유리 파편
- Luminous Vortex Black Hole: 소용돌이·배경 왜곡 블랙홀
- Golden Chain Rain: 황금 사슬 비·마법진
- Sacred Relic Descent: 백금 피라미드 강림·빛과 연기 5파동

## 사용

Three.js 0.187.0, WebGL2가 필요합니다. 외부 텍스처·모델·음원은 필요하지 않습니다. `npm ci`, `npm run dev`로 샘플을 실행합니다. `?effect=black-hole` 등 모듈 ID로 샘플을 선택합니다. 샘플은 특정 시점의 정지 장면이며 실제 게임에서는 프레임마다 update를 호출합니다.

```js
import createVFX from './effects/darkchain-detonation.js';
const effect = createVFX();
scene.add(effect.group);
effect.update(deltaSeconds);
effect.reset();
effect.stop(); // 종료될 때까지 update 계속 호출
// 영구 제거 시 effect.dispose()
```

동일한 Three.js 인스턴스를 공유하고 XZ 지면, +Y 위쪽을 사용하세요. SRGBColorSpace·NoToneMapping 기준이며 게임의 렌더러 전역 설정을 임의로 바꾸지 마세요. 배경 왜곡은 불투명 오브젝트 위주로 작동합니다. Sacred Relic은 시각 효과만 제공하며 치유·충돌·지형 변경은 구현하지 않습니다. 모바일 실기기 성능 보장은 없습니다.

## 출처와 권리

- 제작: 00GameDevs (@00vchannel)
- 원본: https://patch.gg/00vchannel/00gamedevs-vfx-starter
- 버전: 0.1.2
- 라이선스: MIT. 모듈 내부의 저작권·허가 고지와 동봉 LICENSE를 유지하세요.
- Three.js MIT 고지는 THIRD-PARTY-NOTICES.md에 보존했습니다.
- 원본 배포 매니페스트와 5개 모듈 SHA-256 일치 확인.
- 원본 웹사이트 UI·브랜드·아바타·게임 아트와 Patch 전용 helper는 제외했습니다. 미리보기는 수집 시 모듈을 직접 렌더한 이미지입니다.
- AI 생성 여부·도구: 원본에서 명시적으로 확인하지 못함.
- 검증: npm ci/build 통과, 5종 WebGL2 렌더 및 reset/stop/finished/dispose 확인(2026-11-23). 물리 휴대전화 성능은 미검증.
