## [Ch02_PyTorch Basic]

벡터, 행렬, 텐서의 개념에 대해서 이해하고, Numpy와 파이토치로 벡터, 행렬, 텐서를 다루는 방법에 대해서 이해합니다.

## [Summary]

- **벡터, 행렬 그리고 텐서(Vector, Matrix and Tensor)**

딥 러닝을 위한 가장 기본적인 수학적 지식인 벡터, 행렬, 텐서에 대해서 알아봅니다.

- **넘파이 훑어보기(Numpy Review)**

파이토치는 파이썬 패키지 넘파이(Numpy)와 유사합니다. 따라서 넘파이에 대해서 간단히 살펴보겠습니다.

- **파이토치 텐서 선언하기(PyTorch Tensor Allocation)**

넘파이로 실습을 해봤습니다. 이제 파이토치 텐서 선언 방법에 대해서 알아봅니다.

- **행렬 곱셈(Maxtrix Multiplication)**

행렬 연산에 대해서 이해합니다.

- **텐서 조작하기(Tensor Manipulation)**

텐서를 조작하는 여러 방법들을 알아봅니다.

## [Point]
| Term | Description |
|:-- |:--|
|뷰(View) | 원소의 수를 유지하면서 텐서의 크기 변경. |
|스퀴즈(Squeeze) | 1인 차원을 제거한다. |
|언스퀴즈(Unsqueeze) | 특정 위치에 1인 차원을 추가한다. |
|연결하기(concatenate) | 두 텐서를 연결하는 법 |
|스택킹(Stacking) | 연결과 비슷하지만 쌓는 법(더 편리함) |
|ones_like와 zeros_like | 0으로 채워진 텐서와 1로 채워진 텐서 |

(view(), squeeze(), unsqueeze()는 텐서의 원소 수를 그대로 유지하면서 모양과 차원을 조절합니다.)
