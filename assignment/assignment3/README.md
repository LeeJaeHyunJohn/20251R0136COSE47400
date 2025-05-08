## Assignment 3: RNN vs GRU for Sequence Classification

이 과제는 PyTorch를 이용하여 기본 순환 신경망(Vanilla RNN)과 게이트 순환 유닛(GRU)을 직접 구현하고, 시퀀스 분류 문제에서 두 모델의 성능을 비교하는 것입니다.

### 폴더 구조
- `code/`: RNN 및 GRU 구현 코드 (`RNN_skeleton.py`, `GRU_skeleton.py`)
- `report/`: 과제 보고서 및 결과 분석
- `instruction/`: 과제에 대한 설명 

### 주요 내용
- Vanilla RNN과 GRU의 forward/backward pass를 직접 구현
- GRU: reset gate, update gate, candidate activation 포함
- 동일한 데이터셋, 하이퍼파라미터 설정 하에 학습 수행
- CrossEntropyLoss 및 Adam Optimizer 사용
- Test Accuracy:
  - **Vanilla RNN: 41.02%**
  - **GRU: 74.25%**
