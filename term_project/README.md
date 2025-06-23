## Term Project: Missing Person Detection from Drone Imagery

이 프로젝트는 저해상도 드론 영상에서 실종자를 효과적으로 탐지하기 위한 다양한 객체 탐지 및 분류 파이프라인을 실험한 결과입니다.  
YOLOv5, Real-ESRGAN, ResNet18 등을 조합한 네 가지 파이프라인의 성능을 비교하고, SR(Super-Resolution)이 탐지 성능에 미치는 영향을 분석하였습니다.

### 폴더 구조
- `term_project_final.ipynb`: 실험 전체를 실행한 최종 코드 노트북
- `Missing Person Detection...pdf`: 논문 형식의 최종 보고서

### 주요 실험 파이프라인
1. **Only YOLO**  
   - YOLOv5 단독 사용 (Baseline)
2. **SR → YOLO**  
   - 전체 이미지를 SR 후 YOLO 적용 (속도 ↓, 성능 ↓)
3. **YOLO → SR → ResNet (Ver.1)**  
   - YOLO 결과 patch를 SR 후, YOLO로 만든 레이블로 분류 (라벨 노이즈 많음)
4. **YOLO → SR → ResNet (Ver.2)**  
   - GT 라벨로 학습한 ResNet 사용

### 주요 성능 지표 (Ver.2 기준)
- Precision: **48.39%**
- mAP@0.5: **0.7753**
- Inference time: **4210ms**


