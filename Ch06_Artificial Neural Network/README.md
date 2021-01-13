# Ch06_Artificial Neural Network

Date: 2021년 1월 13일
Description: Perceptron, Neural Network, Activation Function, Backpropagation, Problems&Solutions

## [Ch06_Artificial Neural Network]

인공신경망에 대한 전반적인 개념을 이해합니다.

퍼셉트론, XOR문제와 다층 퍼셉트론, 인공신경망, 역전파, 비선형 활성화 함수, 과접합과 기울기 소실 문제와 해결법 등에 대해 배웁니다.

## [Summary]

- 퍼셉트론의 개념과 AND, NAND, OR gate를 단층 퍼셉트론을 이용해 해결해 봅니다.
- 다층 퍼셉트론을 통해 XOR문제를 해결해 봅니다.
- 신경망과 DNN에 대해 이해해 봅니다.
- 역전파를 수식으로 이해해 봅니다.
- 다층 퍼셉트론으로 MNIST를 분류하는 것을 PyTorch로 구현합니다.
- 과적합과 기울기 소실 문제를 이해하고 해결법을 파악합니다.

## [Point]

[용어 정리](https://www.notion.so/d5c1ce8b50644b17b26750e2fb203eb8)

### Activation Function

Sigmoid, Tanh, ReLu, ELU 등등

[angelfox4/DL_floor_study](https://github.com/angelfox4/DL_floor_study/tree/main/Ch03_Neural%20Network)

### Backpropagation

두 가지 방식으로 설명 가능하며 다음 사이트에서 매우 설명이 잘 되어 있음

수식적 방식-PyTorch로 시작하는 딥러닝

그래프 방식-밑바닥부터 시작하는 딥러닝1 또는 css233n 강의

두 가지 방식을 모두 설명해 놓은 것을 정리한 github로 그래프 방식은 코드로 수식적 방식은 손으로 써 놓음.

[angelfox4/DL_floor_study](https://github.com/angelfox4/DL_floor_study/tree/main/ch05_backpropagation)

[출력층의 활성화 함수와 오차 함수의 관계](https://www.notion.so/0c1f88783370414e986bd2b93d8a2af7)

### **Problems**

- Overfitting

복잡성을 낮추기 : 매개변수를 줄이거나 층 수를 줄이기

대량의 데이터 : semi supervised 또는 Augmentation

Regularization : L1(더 강력함) 규제, L2 규제

Dropout : 학습과정에서 신경망의 일부를 사용하지 않는 방법

- Vanishing gradient problem

활성화 함수→css233n에서 은닉층에 시그모이드를 사용하지 말고, 우선적으로 ReLu를 사용한 뒤, ReLu 계열의 함수들을 적용해 보라고 추천

Initalization : 시그모이드 계열 함수를 사용할 경우 Xavier initalization을 사용, ReLu 계열 함수를 사용할 경우 He initalization을 사용이 효율적

Batch Normalization : 인공신경망의 각 층에 들어가는 입력을 평균과 분산으로 정규화

Layer Normalization : 배치정규화는 미니배치 속 feature 단위로 했다면 층 정규화는 미니 배치 속 샘플 단위로 정규화를 시행, 배치크기에 의존적이지 않으며 RNN에도 적용 가능

Residual net : 층과 층 사이를 건너뛰는 에스컬레이터(?) 설치

- Local minima에 빠지는 문제

Momentum : 가속도, weight의 업데이트 값에 이전 업데이트 값의 일정 비율을 더함

NAG : 선험적으로 먼저 업데이트한 후 에러를 교정

Adagrad : 드물게 나타나는 기울기 성분도 고려해서 파라미터 업데이트

Adadelta : adapts learning rates based on a moving window of gradient updates

Rmsprop : Adagrad에서 지수 이동평균을 이용

Adam : momentum+Rmsprop

### [Referrence]

[위키독스](https://wikidocs.net/book/2788)