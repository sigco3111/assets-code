# Kervan asset-forge 절차적 3D 모델 생성 파이프라인

Kervan의 GLB 모델 11종을 코드로 생성하는 headless Blender 파이프라인(assets/src)입니다. 공통 키트 `_kv.py`와 모델별 빌더(도시 랜드마크 7, 시장, 카라반사라이, 낙타, 라이더), GLB 슬림화 `slim_glb.py`, 빌드·텍스처 PowerShell 드라이버로 구성됩니다. 색·치수·파츠를 바꿔 변형 모델을 만들 때 그대로 쓸 수 있습니다.

**라이선스: MIT** (Copyright (c) 2026 Furkiozknn). 재배포 시 저작권 표기와 MIT 전문 유지가 조건입니다.

- 출처: https://github.com/Furkiozknn/kervan (assets/src) · 생성물 팩: assets-3d-lowpoly-2 kervan-anatolia-models
- 수집일: 2026-11-24 · 파일: kervan-asset-forge.zip (Python 12 + PowerShell 2 + MIT 전문 + 사용 안내)
- 의존: Blender 4.x headless, 외부 파이썬 패키지 없음
