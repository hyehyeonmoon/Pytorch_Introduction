## [Ch05_Softmax]

3개 이상의 선택지로부터 1개를 선택하는 문제인 다중 클래스 분류(Multi-Class classification)를 풀기 위한 소프트맥스 회귀에 대해서 학습합니다. 

## [Summary]

- one-hot encoding과 label encoding의 차이를 배웁니다.
- Softmax regression 함수와 특징을 이해합니다.
- 비용함수인 cross entropy function에 대해 이해하고, 이진 분류였을 때와 비교해 봅니다.
- 소프트맥스 회귀를 PyTorch로 구현해 봅니다.
- MNIST데이터를 softmax를 사용하여 학습 및 평가해 봅니다.

## [Point]

소프트맥스 함수(Softmax function)

<img src="https://user-images.githubusercontent.com/55529617/104328133-de37fd80-552e-11eb-8b04-7f34ef74c682.png" width=400 height=100>

크로스 엔트로피(Cross Entrophy)

소프트맥스 함수의 최종 비용 함수에서 k가 2라고 가정하면 결국 로지스틱 회귀의 비용함수와 같다.

<img src="https://user-images.githubusercontent.com/55529617/104328130-dd06d080-552e-11eb-9758-991810000891.png" width=700 height=100>

### [Referrence]

[PyTorch로 시작하는 딥러닝](https://wikidocs.net/book/2788)
