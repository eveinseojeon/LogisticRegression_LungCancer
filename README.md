## 로지스틱 회귀 분석 - 폐암 재발 여부 예측

### ✔ 주제

: 환자별 CEA post, lymphatic(림프계), vascular(혈관), p stage, pt, pn, perineural, age(연령) 데이터를 사용하여 폐암 재발(relapse) 여부를 예측하는 로지스틱 회귀 분석 모델 빌드 및 학습

### ✔ 데이터

: train, valid (변수 - relapse, CEA post, lymphatic, vascular, p stage, pt, pn, perineural, age)

### ✔ 수행 방법

1. train 데이터 가져오기
1. 먼저 8개 변수를 모두 사용하여 로지스틱 회귀 분석 실시
1. 유의미한(p-value<0.05) 변수 CEA_Post, Lymphatic, Vascular 3개만 추출하여 로지스틱 회귀 분석 모델 생성
1. 각 변수들의 계수에 exponential 취하여 odds ratio 계산하여 모델 해석
1. validation 데이터 사용하여 모델 성능 평가(ROC curve 그려서 AUC 계산)

### ✔ 사용 라이브러리

: Pandas, Numpy, Matplotlib, Seaborn, Statsmodels, Sklearn

