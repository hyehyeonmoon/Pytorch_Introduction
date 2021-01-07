# Ch03_Linear Regression

Date: 2021년 1월 6일

## [Ch03_LInear Regression]

가설과 이에 대한 비용함수를 구해 경사하강법으로 최적의 해를 찾는 법을 배웁니다. 단순선형회귀, 다중선형회귀를 PyTorch로 구현하고, nn.Module, class, mini batch도 적용합니다.

## [Summary]

- **데이터에 대한 이해(Data Definition)**

학습할 데이터에 대해서 알아봅니다.

- **가설(Hypothesis) 수립**

가설을 수립하는 방법에 대해서 알아봅니다.

- **손실 계산하기(Compute loss)**

학습 데이터를 이용해서 연속적으로 모델을 개선시키는데 이 때 손실(loss)를 이용합니다.

- **경사 하강법(Gradient Descent)**

학습을 위한 핵심 알고리즘인 경사 하강법(Gradient Descent)에 대해서 이해합니다.

- **단순 선형회귀(Simple Linear regression), 다중 선형회귀(Multivariate Linear regression)**

선형회귀의 구조와 모수에 대해 이해하고, 파이토치로 구현해 봅니다.

- **미니배치(Mini Batch)**

epoch, batch, iteration 용어를 이해하고 코드로 적용해 봅니다.

## [Point]

선형회귀(행렬 표현)

![Ch03_Linear%20Regression%20da41bf679e0a47f3be8eeb1589cece2f/Untitled.png](Ch03_Linear%20Regression%20da41bf679e0a47f3be8eeb1589cece2f/Untitled.png)

![Ch03_Linear%20Regression%20da41bf679e0a47f3be8eeb1589cece2f/Untitled%201.png](Ch03_Linear%20Regression%20da41bf679e0a47f3be8eeb1589cece2f/Untitled%201.png)

MSE(Mean squared Error)

![Ch03_Linear%20Regression%20da41bf679e0a47f3be8eeb1589cece2f/Untitled%202.png](Ch03_Linear%20Regression%20da41bf679e0a47f3be8eeb1589cece2f/Untitled%202.png)

Mini Batch

![Ch03_Linear%20Regression%20da41bf679e0a47f3be8eeb1589cece2f/Untitled%203.png](Ch03_Linear%20Regression%20da41bf679e0a47f3be8eeb1589cece2f/Untitled%203.png)

배치 크기(batch size) : 미니 배치의 크기

에포크(Epoch) : 전체 훈련 데이터가 학습에 한 번 사용된 주기

이터레이션(Iteration) : 한 번의 에포크 내에서 이루어지는 매개변수인 가중치 W와 b의 업데이트 횟수