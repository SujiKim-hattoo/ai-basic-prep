# EDA (Exploratory Data Analysis)란 무엇인가

---

## 1. 정의

### 1.1 개념 소개

EDA는 \*\*1970년대 미국 수학자 John Tukey(존 튜키)\*\*가 제안한 개념

* **Exploratory**: 탐색적
* **Data**: 데이터
* **Analysis**: 분석

### 1.2 의미

데이터를 **탐색적**으로 분석하는 **과정 또는 그 결과**를 의미
> (참고) IBM에서의 EDA 정의: *“**Analyze and investigate** data sets and **summarize** their main characteristics, often employing **data visualization** methods.”*

* **좁은 의미**:
  AI 모델을 학습하거나 분석하기 전에 **데이터의 특성을 이해하기 위한 과정**

* **넓은 의미**:
  데이터의 주요 구조와 특징을 **직관적으로 이해하기 위한 모든 활동**

### 1.3 역할

EDA는 데이터 분석의 **첫 번째 단계**로, 전체 데이터 분석 흐름은 다음과 같다.

```
Raw Data → EDA → Conclusions
```

---

## 2. 특징

* 데이터 자체: 데이터 구조, 패턴, 특성 파악
* 데이터 분석: 데이터 기반 **의문과 인사이트 유도**
* 데이터 시각화: 시각화 도구를 활용해 **데이터를 직관적으로 요약**
* 데이터 - 모델링: 이상치, 결측치 등 **모델링에 영향을 줄 수 있는 요소 탐색** => 전처리의 기초로 작용됨

---
  
## 3. 단계별 수행 절차(6단계)
- 데이터의 특성과 분석 목적에 따라 단계는 달라질 수 있음

### 3.1 문제 및 데이터 이해

* 비즈니스 목표와 데이터의 특성을 파악
* 분석 한계 및 목적 설정

### 3.2 데이터 불러오기 및 전반적인 분포 확인
* 통계 분석에서 주로 사용되는 언어와 도구: Python, R, SQL 등
* 데이터 추출 및 구조 확인
* 주요 기술 통계 확인: `describe()` 등

### 3.3 데이터 다듬기
  #### 3.3.1 결측치(Missing Data) 처리
  * 결측값을 무시할지, 보완할지 결정
  * 보완 방법: 평균, 중앙값 대체 / 삭제 / 예측 기반 대체 등

  #### 3.3.2 이상치(Outlier) 처리
  * Boxplot
  * IQR 방식
  * Z-score
  * Percentile 기반
  (중요) 이상치를 무조건 제거하기보다는 데이터별로 어떻게 처리할지 판단하는 것이 중요하다.

### 3.4 데이터 분석
  #### 3.4.1 데이터 특성 파악
  * 평균, 분산, 표준편차, 왜도(skewness) 등 계산
  * 데이터 분포의 형태 이해
  
  #### 3.4.2 데이터 변환
  * 분석 또는 모델링에 적합한 형식으로 변환
  * 범주형 → 수치형, 로그 변환 등 다양한 방식 활용

### 3.5 시각화 (Visualization)

**대표 도구**: Matplotlib, Seaborn (Python)

* 단변량(Univariate):
  `histplot`, `boxplot`, `violinplot`, `countplot` 등
* 이변량(Bivariate):
  `scatterplot`, `regplot`, `heatmap`, `barplot`, `stripplot`, `swarmplot` 등
* 다변량(Multivariate):
  `pairplot`, `scatterplot`(+hue) 등

### 3.6 인사이트 도출 및 공유

* 데이터 분석을 통해 얻은 **주요 발견 및 통찰 정리**
* 보고서, 시각화, 프레젠테이션 등으로 결과 공유

---

## 4. 효과 및 활용 가치

* 모델링 이전 단계에서 **데이터의 전반적인 이해** 제공
  * 데이터 품질을 높이고 분석 기반 마련
* 오류나 이상치, 결측치를 파악하고 정제
* => 더 정확한 모델 선택과 설계 가능

---

## 5. 요약

### 5.1 한 줄 요약

EDA는 **전반적인 데이터 이해와 정확한 모델링 설계를 위한 필수적인 데이터 탐색 과정**이다.

### 5.2 세 줄 요약

1. raw data를 *탐색*하며 이상치와 결측치를 파악하고 *정제*한다.
2. 정제된 데이터를 *시각화*하여 핵심 패턴과 인사이트를 발견한다.
3. 분석 목적에 맞게 *모델링*을 준비하기 위한 *기반을 마련*한다.

---

## 6. 참고자료

* IBM: [https://www.ibm.com/think/topics/exploratory-data-analysis](https://www.ibm.com/think/topics/exploratory-data-analysis)
* GeeksforGeeks: [https://www.geeksforgeeks.org/data-analysis/what-is-exploratory-data-analysis/](https://www.geeksforgeeks.org/data-analysis/what-is-exploratory-data-analysis/)
* Medium: [https://medium.com/data-science/a-data-scientists-essential-guide-to-exploratory-data-analysis-25637eee0cf6](https://medium.com/data-science/a-data-scientists-essential-guide-to-exploratory-data-analysis-25637eee0cf6)
* 김장현 & 김민철 (2023). *문과생을 위한 인공지능 입문*. 에이콘출판사
