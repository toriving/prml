---
layout: default
title: Chapter 1
nav_order: 3
has_children: true
has_toc: false
use_math: true
---

# Chapter 1. 소개
{: .no_toc }

---
{: .no_toc }

주어진 데이터에서 어떤 특정한 패턴을 찾아내는 것은 때때로 아주 중요한 문제다.

패턴 인식은 컴퓨터 알고리즘을 활용하여 데이터의 규칙성을 자동적으로 찾아내고, 이 이용하여 데이터를 각각의 카테고리로 분류하는 등의 일을 하는 분야다.

손글씨로 쓰인 숫자를 인식하는 문제에서는 직접 작성한 규칙이나 휴리스틱 알고리즘을 통해 생성된 규칙을 사용하여 문제를 해결 할 수 있다.

하지만 이러한 방식은 많은 예외와 수 많은 규칙이 필요하다.

머신 러닝을 적용하면 더 나은 결과를 얻을 수 있다.

---

머신 러닝 알고리즘의 결과물은 함수 $y(x)$ 로 표현할 수 있다. 

$y(x)$는 새로운 $x$를 입력값으로 받았을 때 대상 벡터와 같은 방식으로 부호화된 벡터 $y$를 출력하는 함수다.

$y(x)$의 형태는 **훈련단계 (Training phase) / 학습단계 (Learning phase)**에서 훈련 집합을 바탕으로 결정 된다.

한번 훈련되고 난 모델은 **시험 집합 (Test set)**에 대해 활용될 수 있다.

이러한 함수는 훈련 단계에서 사용되지 않았던 새로운 예시들을 올바르게 분류하는 능력인 **일반화(Generalization)** 을 가져야 한다.

또한 문제를 더 쉽게 표현하거나 축소하기 위해 **차원 감소 (Dimensionality reduction)**과 같은 **전처리 (Preprocessed) / 특징 추출 (Feature extraction)**을 하기도 한다.

해당 과정은 훈련 집합에서 뿐만 아니라 시험 데이터에서도 똑같이 이루어져야 한다.

---

기계 학습은 다음과 같이 분류할 수 있다.

- **지도 학습 (Supervised learning)** : 일반적으로 Labeled data에서 label과 $x$(Feature)를 모두 사용하는 경우
    - 분류 문제 (Classification)
    - 회귀 문제 (Regression) 

- **비지도 학습 (Unsupervised learning)** : 표적 벡터 (label) 없이 오직 입력 벡터 $x$로만 주어지는 경우
    - 집단화 (Clustering)
    - 밀도 추정 (Density estimation)
    - 시각화 (Visualization)
    
- **강화 학습 (Reinforcement learning)** : 주어진 상황에서 보상을 최대화하기 위한 행동을 찾는 문제를 푸는 방법
    - 탐사 (Exploration)과 이용 (Exploitation) 간의 trade off 존재
    - DQN, A3C, ...
 