# Ch04_Logistic Regression

Date: 2021년 1월 6일

## [Ch04_Logistic regression]

둘 중 하나를 결정하는 문제를 이진 분류(Binary Classification)라고 합니다. 그리고 이진 분류를 풀기 위한 대표적인 알고리즘으로 로지스틱 회귀(Logistic Regression)가 있습니다.

## [Summary]

- 이진 분류 문제를 다루기 위해 **시그모이드 함수(sigmoid function)**를 배웁니다.
- 비용함수로 **크로스 엔트로피(Cross Entrophy)**에 대해 알아봅니다.
- 파이토치로 로지스틱 회귀를 구현해 봅니다.
- nn.Module과 class를 이용해 로지스틱 회귀를 구현해 봅니다.

## [Point]

시그모이드 함수(Sigmoid function)

![Ch04_Logistic%20Regression%2064829dc66c8f4dfba66bedc22e3a0e9a/Untitled.png](Ch04_Logistic%20Regression%2064829dc66c8f4dfba66bedc22e3a0e9a/Untitled.png)

크로스 엔트로피(Cross Entrophy)

![Ch04_Logistic%20Regression%2064829dc66c8f4dfba66bedc22e3a0e9a/Untitled%201.png](Ch04_Logistic%20Regression%2064829dc66c8f4dfba66bedc22e3a0e9a/Untitled%201.png)

### [Referrence]

[위키독스](https://wikidocs.net/book/2788)