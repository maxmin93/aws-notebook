# AWS-SageMaker notebook 사용해보기

구글의 colab 대체가 가능한 딥러닝 도구

## 설정

- 인스턴스 : `ml.t3.xlarge`
  - [ml.t3.xlarge 요금](https://aws.amazon.com/ko/sagemaker/pricing/):	4CPUs	16GiB	0.25 USD (1시간에 4백원)
  - 구글 colab 과 비슷하거나 약간 더 나은 성능 나옴
- Git 리포지토리 : 깃허브 연결
- 커널: `conda_amazonei_tensorflow2_p36`
  - 모델 훈련을 시키려면 반드시 `amazonei`가 들어간 커널을 사용해야 함 (안들어 간 커널은 모델 평가용)
  - `ml.t3.medium` 과 `ml.t3.xlarge` 은 `amazonei` 커널이 있는데, `ml.t3.large` 은 없다

## 테스트

- CNN : 코랩보다 2배 느림 ==> 동일 또는 약간 더 빠름 
- LSTM : 코랩보다 약간 빠름 (약 85%?) ==> 더 빠름 (70%?)

