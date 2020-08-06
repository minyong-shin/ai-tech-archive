# EDA   
Assembled by Sohyeon Yim (2020-08-06)   

## GOAL   
1. EDA 정의   
2. EDA를 하는 이유   
3. EDA 도구들   

## EDA 정의   
- 데이터를 분석하기 전 그래프나 통계적인 방법으로 자료 분석   

## 👀 EDA를 하는 이유   
- garbage in, garbage out 하기 위해 필요   

- 데이터 설명서가 없을 때, 모델 학습 시 전처리가 필요한 데이터 파악 및 전처리    
  * 수치형으로 입력되어 있지만 실체는 명목형인 변수 -> one-hot encoding 필요   
  * 명목형으로 입력되어 있지만 실제는 순서상의 의미를 가지는 변수 -> 수치형 데이터로 변환   
  * 합쳐서 하나로 만들 수 있는 변수 -> 합쳐서 하나의 변수로 만들기     
  * 쪼개서 나눌 수 있는 변수 -> 쪼개서 새로운 변수 만들기   
  * 결측값인지 0인지 헷갈리는 관측치 -> 결측값이면 data imputation 또는 제거     

- 상관관계 분석 -> 다중공선성 제거 등   

- 이상치 파악 -> 이상치 제거 등   

- 새로운 feature 탐색  -> 새로운 feature 만들기     

## EDA 도구들    
- seaborn 이용    
- matplotlib 이용   
- plotly 이용   

## Reference & Additional Resources      
[eda 데이터 설명서에서 시작하기](https://medium.com/mighty-data-science-bootcamp/eda-%EB%8D%B0%EC%9D%B4%ED%84%B0-%EC%84%A4%EB%AA%85%EC%84%9C%EC%97%90%EC%84%9C-%EC%8B%9C%EC%9E%91%ED%95%98%EA%B8%B0-230060b9fc17)
