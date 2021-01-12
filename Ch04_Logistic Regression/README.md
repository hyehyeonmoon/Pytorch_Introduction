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

<img src="https://user-images.githubusercontent.com/55529617/103802408-6d0dcb80-5092-11eb-9072-5d8c4bc7ec0c.png" width=800 height=180>

크로스 엔트로피(Cross Entrophy)

<img src="https://user-images.githubusercontent.com/55529617/103802412-6e3ef880-5092-11eb-9bd9-d966574d7a5b.png" width=800 height=180>

### [Referrence]

[PyTorch로 시작하는 딥러닝](https://wikidocs.net/book/2788)
