# Machine Learning Overview

## **What is Machine Learning? (머신러닝이란?)**

* A new approach to solving problems.
* Answering complex questions.
* Creating new content.
* Making recommendations.
* Predicting outcomes.

## **How Does Machine Learning Work? (머신러닝의 작동 원리)**

**Basic Process:**

* Utilizing data → Training models → Learned patterns → Predictions or discovering patterns.

**Key Terms:**

* **Model (모델)**: Defines mathematical relationships (patterns) between input data (features) and output data (labels).
* **Training/Learning (학습)**: Improving model prediction performance by reducing loss values based on data.
* **Pattern (패턴)**: Relationships that a model learns through training.
* **Inference (추론)**: Applying a trained model to unlabeled input data to make predictions or analyze patterns.

## **Types of Machine Learning (머신러닝의 유형)**

There are two representative methods based on feedback provided:

### 1. Supervised Learning (지도학습)

**Definition:** Learning from datasets containing correct answers (labels).

**Goal:** Discover relationships between input features and labels to predict outcomes for new data.

* **Features (피처)**: Input data used for learning.
* **Label (레이블)**: Output data, the target for prediction.

**Analogy:** Studying past exams (features and labels) to prepare for new exams.

#### Types of Supervised Learning:

* **Regression (회귀)**

  * Predicting numeric continuous outcomes.
  * e.g., electricity usage, rainfall, house prices, sales projections.

* **Classification (분류)**

  * Predicting categorical outcomes.
  * e.g., Cat vs. non-cat (image classification), spam vs. non-spam emails, benign vs. malignant tumors.

  **Sub-types:**

  * **Binary classification (이진 분류)**: Two categories of results (positive 양성 or negative 음성).
  * **Multiclass classification (다중 분류)**: Multiple categories of results (handwritten letters, weather conditions: sunny/rainy/snowy, risk levels: high/medium/low).

### 2. Unsupervised Learning (비지도학습)

**Definition:** Learning from datasets without predefined answers (labels).

**Goal:** Identify meaningful patterns and groupings within the data.

#### Types of Unsupervised Learning:

* **Clustering (군집화)**

  * Finding groups of similar data naturally separated from others.
  * e.g., Customer data grouped by age, spending patterns.

* **Dimensionality Reduction (차원 축소)**

  * Removing noise and compressing data while maintaining essential information, reducing computational resources and storage.

* **Association Rules (연관 규칙)**

  * Identifying relationships between variables and extracting them as rules.
  * e.g., "Customers Who Bought This Item Also Bought" (Amazon), "Discover Weekly" (Spotify).

### Commonalities (공통점):

* Both methods aim to uncover hidden patterns within datasets.
* Require large and diverse datasets for accurate pattern recognition and prediction.

## **Additional Terms**

* **Reinforcement Learning (강화학습)**: Learning optimal strategies through trial-and-error by receiving rewards or penalties. Commonly used in game AI, robot control, and autonomous driving to actively respond to environmental changes. Combines aspects of supervised (feedback provided) and unsupervised learning (no initial direct answers). [AI Learns Insane Way to Jump](https://youtube.com/shorts/hgjsLmFSkxo?feature=shared)

* **Generative AI (생성형 AI)**: Creating new content (text, images, audio, video) based on user input through various methods. Supervised learning for summarization and unsupervised learning for data mimicry.

## **Practical Example (상품 추천 시스템 예시)**

* **Supervised learning**: Using purchase history and specific product purchase outcomes for recommendations.
* **Unsupervised learning**: Grouping consumers with similar tastes.
* **Reinforcement learning**: Providing recommendations and adjusting strategies based on consumer reactions (click behavior).

## **Summary Table (학습 방식 요약)**

| Learning Type (학습 유형)         | Data Type (데이터 유형)          | Feedback (피드백)              | Objective (목표)                        |
| ----------------------------- | --------------------------- | --------------------------- | ------------------------------------- |
| Supervised Learning (지도학습)    | Labeled Data (레이블 데이터)      | Direct feedback (직접적 피드백)   | Predict outcomes (결과 예측)              |
| Unsupervised Learning (비지도학습) | Unlabeled Data (레이블 없음)     | No direct feedback (피드백 없음) | Find hidden patterns (숨겨진 패턴 찾기)      |
| Reinforcement Learning (강화학습) | Interaction-based (상호작용 기반) | Rewards/Penalties (보상/패널티)  | Determine optimal strategy (최적 전략 도출) |

## **c.f. Clarification of Commonly Confused Terms (헷갈리는 용어정리)**

* **Feature = Predictor Variable (입력 변수)**: Variables used for prediction, e.g., predicting house prices based on location and size.
* **Input Data (입력 데이터)**: Actual values entered into features.
* **Output Data = Target = Label (출력 데이터, 타겟, 레이블)**: Values you want to predict, e.g., house price.

## **References (참고자료)**

* IBM What is unsupervised learning? [Link](https://www.ibm.com/think/topics/unsupervised-learning)
* Google Machine Learning foundational courses: [Link](https://developers.google.com/machine-learning/intro-to-ml/what-is-ml#generative_ai)
* 김장현, 김민철, ⌜문과생을 위한 인공지능 입문⌟, 에이콘출판, 2023.04.27.
* 세바스찬 라시카, 바히드 미자리리, ⌜머신 러닝 교과서 with 파이썬, 사이킷런, 텐서플로⌟, 박해선 옮김, 길벗, 2021.03.31, 개정 2판.

 ---
 ---

# Machine Learning Overview

## **What is Machine Learning? (머신러닝이란?)**

* 문제 해결을 위한 새로운 접근 방식입
* 복잡한 질문에 답변 가능
* 새로운 콘텐츠를 **생성** 가능
* **추천** 시스템을 만들 수 있습니다.
* 결과 **예측** 가능

## **How Does Machine Learning Work? (머신러닝의 작동 원리)**

**기본 과정:**

* 데이터 활용 -> 모델 학습 -> 학습된 패턴 => 예측 or 패턴 발견 등

**주요 용어:**

* **Model (모델)**: 입력 데이터(features)와 출력 데이터(lables) 간의 수학적인 관계(pattern)
* **Training/Learning (학습)**: 데이터에 기반-> 오차 값 줄여 => 모델 예측 성능 개선
* **Pattern (패턴)**: 학습을 통해 모델이 배우는 수학적인 관계
* **Inference (추론)**: 학습된 모델을 사용해 라벨이 없는 입력 데이터에 대해 예측을 수행하거나 패턴 분석을 하는 것

## **Types of Machine Learning (머신러닝의 유형)**

피드백 유무에 따라 대표적으로 두 가지 방식으로 나뉨

### 1. Supervised Learning (지도학습)

**정의:** *정답(label)이 포함*된 데이터셋을 기반으로 학습합니다.

**목표:** feature-label 관계 발견 -> 새로운 데이터 결과 예측

* **Features (피처)**: 학습에 사용되는 입력 데이터
* **Label (레이블)**: 예측하고자 하는 출력 데이터
  (c.f. 기출문제 -> 새로운 시험을 준비하는 것과 비슷)

#### 지도학습의 유형:

* **Regression (회귀)**

  * 숫자형 데이터(연속적인 종속변수) 예측
  * 예: 전기 사용량, 강수량, 집값, 매출 예측 등

* **Classification (분류)**

  * 범주형 결과 예측
  * 예: 이미지 분류(고양이냐 아니야), 텍스트 분류(스팸 메일이냐 아니냐) 등

  **세부 유형:**

  * **Binary classification (이진 분류)**: 두 가지 범주로 결과가 나옵니다 (예: 종양 진단 -> 악성 또는 양성).
  * **Multiclass classification (다중 분류)**: 세 가지 이상 범주로 결과가 나옵니다 (예: 손글씨 문자, 날씨 상태: 맑음/비/눈, 위험 수준: 높음/중간/낮음)

### 2. Unsupervised Learning (비지도학습)

**정의:** *정답(레이블)이 없는* 데이터셋을 기반으로 학습합니다.

**목표:** 데이터 안에 존재하는 의미 있는 패턴이나 그룹을 식별

#### 비지도학습의 유형:

* **Clustering (군집화)**

  * 다른 데이터들과 구분되면서 자연스럽게 묶이는 비슷한 데이터 그룹 찾기
  * 예: 나이, 소비 패턴 등으로 분석해 묶인 고객 데이터

* **Dimensionality Reduction (차원 축소)**

  * 노이즈 제거 & 핵심 정보를 유지 & 데이터 압축 => 계산 자원과 저장 공간 줄여

* **Association Rules (연관 규칙)**

  * 데이터 내 변수들 간의 관계 -> 규칙 형태로 도출
  * 예: *Customers Who Bought This Item Also Bought* (Amazon), *Discover Weekly* (Spotify)

### 공통점:

* 데이터 안의 숨겨진 패턴 찾기
* (가능한) 다양하고 방대한 데이터셋 필요 -> 정확한 패턴 인식 및 예측에 사용

## **Additional Terms**

* **Reinforcement Learning (강화학습)**: 여러 번의 시행착오 -> 각 행동에 대해 보상 or 패널티를 받으며 최적의 전략을 스스로 학습하는 방식. 주로 게임AI, 로봇 제어, 자율 주행 등 환경 변화에 능동적으로 대응할 필요가 있는 학습. 지도학습(피드백o)과 비지도학습(정답 제시x)의 요소가 결합[AI Learns Insane Way to Jump](https://youtube.com/shorts/hgjsLmFSkxo?feature=shared)
 
* **Generative AI (생성형 AI)**: 사용자 입력을 기반으로 다양한 방식을 통해 텍스트, 이미지, 오디오, 비디오 등 새로운 콘텐츠를 생성. 요약에는 지도학습이, 데이터 모방에는 비지도학습이 활용될 수 있음

## **Practical Example (상품 추천 시스템 예시)**

* **지도학습**: 구매 이력과 특정 제품 구매 결과 -> 추천
* **비지도학습**: 비슷한 취향을 가진 소비자 그룹화
* **강화학습**: 추천 후 소비자의 반응(클릭 여부)을 보고 전략 조정

## **Summary Table (학습 방식 요약)**

| Learning Type (학습 유형)         | Data Type (데이터 유형)          | Feedback (피드백)              | Objective (목표)                        |
| ----------------------------- | --------------------------- | --------------------------- | ------------------------------------- |
| Supervised Learning (지도학습)    | Labeled Data (레이블 데이터)      | Direct feedback (직접적 피드백)   | Predict outcomes (결과 예측)              |
| Unsupervised Learning (비지도학습) | Unlabeled Data (레이블 없음)     | No direct feedback (피드백 없음) | Find hidden patterns (숨겨진 패턴 찾기)      |
| Reinforcement Learning (강화학습) | Interaction-based (상호작용 기반) | Rewards/Penalties (보상/패널티)  | Determine optimal strategy (최적 전략 도출) |

## **c.f. Clarification of Commonly Confused Terms (헷갈리는 용어 정리)**

* **Feature = Predictor Variable (입력 변수)**: 예측에 사용되는 변수들 (예: 집값을 예측할 때 위치, 면적 등)
* **Input Data (입력 데이터)**: 특징에 입력되는 실제 값들
* **Output Data = Target = Label (출력 데이터, 타겟, 레이블)**: 예측하고자 하는 값 (예: 집값)

## **References (참고자료)**

* IBM What is unsupervised learning? [Link](https://www.ibm.com/think/topics/unsupervised-learning)
* Google Machine Learning foundational courses: [Link](https://developers.google.com/machine-learning/intro-to-ml/what-is-ml#generative_ai)
* 김장현, 김민철, ⌜문과생을 위한 인공지능 입문⌟, 에이콘출판, 2023.04.27.
* 세바스찬 라시카, 바히드 미자리리, ⌜머신 러닝 교과서 with 파이썬, 사이킷런, 텐서플로⌟, 박해선 옮김, 길벗, 2021.03.31, 개정 2판.
