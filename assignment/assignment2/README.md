## Assignment 2: ResNet-50 Implementation for CIFAR-10

이 과제는 PyTorch를 사용하여 ResNet-50 아키텍처 기반의 합성곱 신경망(CNN)을 구현하고, CIFAR-10 데이터셋의 분류 문제를 해결하는 것입니다.

### 폴더 구조
- `code/`: ResNet-50 모델 구현 코드 (`resnet50_skeleton.py`)
- `report/`: 보고서 및 실험 결과 (`CNN_Implementation.pdf`)
- `instruction/`: 과제에 대한 설명

### 주요 내용
- Bottleneck 구조의 Residual Block 직접 구현
- `layer2`, `layer3`, `layer4`, `avgpool`, `fc` 계층 완성
- CrossEntropyLoss와 Adam Optimizer 사용
- CIFAR-10 데이터셋 분류 모델 학습 (500 step)
- Test Accuracy: **81.18%**
