# Machine Learning Overview

---
---

## **What is Machine Learning? (머신러닝이란?)**

* A new approach to solving problems.
* Answering complex questions.
* Creating new content.
* Making recommendations.
* Predicting outcomes.

---

## **How Does Machine Learning Work? (머신러닝의 작동 원리)**

**Basic Process:**

* Training software models using data.
* Generating useful predictions or creating new content based on learned patterns.

**Key Terms:**

* **Model (모델)**: Defines mathematical relationships (patterns) between input data (features) and output data (labels).
* **Pattern (패턴)**: Relationships that a model learns through training.
* **Training/Learning (학습)**: The process by which a model improves its predictions by updating loss values based on data.

  * e.g., Human analogy: Touching boiling water (input data) → getting burned (output data) → learning not to touch boiling water again (knowledge).
* **Inference (추론)**: Applying a trained model to unlabeled features to make predictions.

---

## **Types of Machine Learning (머신러닝의 유형)**

There are two representative methods based on feedback provided:

### 1. Supervised Learning (지도학습)

**Definition:** Learning from datasets with correct answers (labels).

**Goal:** Discover relationships between input features and labels to predict outcomes for new data.

* **Features (피쳐)**: Input data used for learning.
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

  * **Binary classification (이진 분류)**: Outputs two categories (positive 양성 or negative 음성).
  * **Multiclass classification (다중 분류)**: Outputs multiple categories (handwritten letters, weather conditions like sunny/rainy/snowy, risk levels high/medium/low).

### 2. Unsupervised Learning (비지도학습)

**Definition:** Learning from datasets without predefined answers (labels).

**Goal:** Identify meaningful patterns and groupings within the data.

#### Types of Unsupervised Learning:

* **Clustering (군집화)**

  * Finding natural groupings within data.
  * e.g., Weather data grouped by temperature and humidity, consumer segmentation.

* **Dimensionality Reduction (차원 축소)**

  * Compressing data by removing noise and keeping essential information, reducing computational and storage requirements.

* **Topic Modeling (토픽 모델링)**

  * Automatically categorizing textual data like product reviews.

### Commonalities (공통점):

* Both methods aim to uncover underlying patterns within datasets for modeling.
* Require large, diverse datasets to ensure accurate pattern recognition and predictions.

## **Additional Terms**

* **Reinforcement Learning (강화학습)**: Learning optimal strategies through trial-and-error, receiving rewards or penalties. Combines supervised (feedback provided) and unsupervised (initially no direct answers) aspects.

* **Generative AI (생성형 AI)**: Creating new content (text, images, audio, video) from user input. Can involve supervised learning for summarization or unsupervised learning for data mimicry.

## **Practical Example (상품 추천 시스템 예시)**

* **Supervised learning**: Requires historical purchasing data and specific product purchase outcomes.
* **Unsupervised learning**: Groups consumers based on traits, identifying similar tastes.
* **Reinforcement learning**: Provides recommendations, observes consumer responses (clicks), and adapts strategy accordingly.

## **Summary Table (학습 방식 요약)**

| Learning Type (학습 유형)         | Data Type (데이터 유형)          | Feedback (피드백)              | Objective (목표)                        |
| ----------------------------- | --------------------------- | --------------------------- | ------------------------------------- |
| Supervised Learning (지도학습)    | Labeled Data (레이블 데이터)      | Direct feedback (직접적 피드백)   | Predict outcomes (결과 예측)              |
| Unsupervised Learning (비지도학습) | Unlabeled Data (레이블 없음)     | No direct feedback (피드백 없음) | Find hidden patterns (숨겨진 패턴 찾기)      |
| Reinforcement Learning (강화학습) | Interaction-based (상호작용 기반) | Rewards/Penalties (보상/패널티)  | Determine optimal strategy (최적 전략 도출) |

---

## **c.f. Clarification of Commonly Confused Terms (헷갈리는 용어정리)**

* **Feature = Predictor Variable (입력 변수)**: Variables used for prediction, e.g., predicting house prices based on location and size.
* **Input Data (입력 데이터)**: Actual values entered into features.
* **Output Data = Target = Label (출력 데이터, 타겟, 레이블)**: Values you want to predict, e.g., house price.

---
---

## **References (참고자료)**

* Google Machine Learning foundational courses: [Link](https://developers.google.com/machine-learning/intro-to-ml/what-is-ml#generative_ai)
* 김장현, 김민철, ⌜문과생을 위한 인공지능 입문⌟, 에이콘출판, 2023.04.27.
* 세바스찬 라시카, 바히드 미자리리, ⌜머신 러닝 교과서 with 파이썬, 사이킷런, 텐서플로⌟, 박해선 옮김, 길벗, 2021.03.31, 개정 2판.
