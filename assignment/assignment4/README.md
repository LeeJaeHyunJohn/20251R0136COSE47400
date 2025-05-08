## Assignment 4: Transformer Implementation from Scratch

이 과제는 Transformer 아키텍처를 PyTorch로 처음부터 직접 구현하고, IMDb 영화 리뷰 데이터를 이용하여 텍스트 분류를 수행하는 것입니다.  
또한 사전학습된 BERT 모델을 동일한 데이터셋에 fine-tuning하여 두 모델의 성능을 비교 분석하였습니다.

### 폴더 구조
- `code/`: Transformer 모델 구현 코드 (`transformer_skeleton.py`)
- `report/`: 과제 보고서 및 실험 결과
- `instruction/`: 과제에 대한 설명 

### 주요 내용
- Positional Encoding, Multi-Head Attention, Transformer Encoder Layer 직접 구현
- IMDb 감성 분류 데이터셋 사용 (Train 15,000 / Valid 5,000 / Test 5,000)
- Self-implemented Transformer 결과:
  - Test Accuracy: **64.56%**
- Fine-tuned BERT 결과:
  - Test Accuracy: **82.48%**
- Pretraining이 NLP 성능에 미치는 영향 분석
