# ORANGE 3
## 무엇을 배울까?
* 오렌지는 기본적으로 표를 다룬다.
* 표는 그 자체로 훌륭하지만 연관성을 살펴보기에는 그래프가 유리하다.
오렌지는 시각화를 제공한다.
* 머신러닝 가능!

## orange3 설치
[Orange Data Mining - Download](https://orangedatamining.com/download/#macos)

## 기본사용법
1. 입력
- 좌측 메뉴바에서 원하는 위젯 끌어다 놓기(OR 화이트보드에서 더블클릭 후 위젯 선택)
- data 입력은 위젯 더블클릭 후 파일 선택 OR URL 기입하기

2. 출력
- 위젯의 오른쪽 부분을 드래그하고 놓으면서 원하는 형태 선택
* 필터링 : Select Rows 위젯을 활용하여 조건 선정가능, 필터의 반대값을 얻으려면 Line을 클릭하여 옵션 선택 가능

  

## 표 다루기

### 용어 정리
* 세로 : 열, column
* 가로 : 행, row
- 표  == 데이터셋

#### 행 을 나타내는 표현
* 개체 (instance)
* 관측치 (observed value)
* 기록 (record)
* 사례 (example)
* 경우 (case)

#### 열 을 나타내는 표현
* 특성 (feature)
* 속성 (attribute)
* 변수 (variable)
* field

## 통계와 시각화
### 데이터의 대표값
- 평균
- 중앙값
- 최빈값

대표값을 통해서 데이터의 성격을 어느정도 가늠할 수 있다.

### boxplot위젯을 통한 시각화
1분위 수 - 25%
2분위 수 - 중앙값
3분위 수 - 75%
4분위 수 - 100%

- 시각화 된 데이터를 통해서 분포도를 어느정도 확인가능하다.
- 표준편차도 제공
**표준편차 : 평균값으로부터 각각의 값이 얼마나 떨어져있는가 에 대한 평균

### 산점도와 상관관계- Scatter plot
Data - Scatter plot 을 선택하고
x축과 y축에 해당하는 값을 설정 후, 시각화 된 그래프를 통해 상관 관계를 살펴볼 수 있다.  
* show regression line을 사용하면 규칙성을 확인하기 더 편하다.

### 상관관계와 인과관계
온도의 변화에 따라 판매량이 변화하는 경우,
온도는 원인이고, 판매량은 결과이다.(원인 : 독립변수, 결과 : 종속변수)

상관관계인데, 원인과 결과로 나눠서 볼 수 있다면 인과관계이기도 하다.
(모든 상관관계가 인과관계인 것은 아니다. 인과관계는 성립하기 어렵다.)

관계 파악을 마쳤다면, **예측**을 할 수 있게 된다.
  
   

## 오렌지3로 머신러닝 다루기
데이터의 속성 간 규칙을 찾아낸다면 새로운 원인에 대한 결과값을 예측할 수 있다.
하지만 결과값에 원인이되는 값들이 엄청나게 많다면?? 
  
인간의 힘으로는 규칙을 쉽게 찾아내지 못할지도 모른다.
  
하지만 컴퓨터는 가능하지.

### 데이터롤(role) 지정
- meta - 필요한 값은 아니지만 참고할 값
- feature - 필요한 값
- target - 구해야하는 값
- skip - 필요없는 값

### Orange 3 위젯 구성 및 역할 소개

<img width="562" alt="스크린샷 2021-07-23 오전 12 08 15" src="https://user-images.githubusercontent.com/61059893/126682596-f0c04c02-f0aa-4096-96ef-82934956b597.png">


#### 데이터 파일
* train_data = 과거 데이터(학습할 대상이 되는 데이터)
* prediction_data = 예측하고자하는 데이터 (독립변수가 정의되어있음)

#### 학습
* Linear Regression = 선형회귀를 통한 규칙 정의(모델 생성)
* Prediction = Linear Regression 결과와 prediction_data의 입력을 받아 결과 반환(당연하게도 입력이 2개)


#Dev/AI/머신러닝야학3기
