# 영화 평점 데이터
##  1. 프로젝트 개요
### 1-1 추천 시스템 주제 선정 동기
> + 요즘 넷플릭스, 쿠팡 , 유튜브를 보면 사용자의 취향에 따라 흥미로운 영상이나 서비스를 추천해준다.
> + 앞으로 친사용자 서비스이며 동시에 친기업 서비스로 강력한 시스템이 될 수 있다고 생각하여 추천 시스템을 주제로 선정하게 되었다.

### 1-2 추천 시스템이란?
> + 정보 소비자가 "원하는" 정보를 찾아 소비자에게 추천하는 시스템
> + 검색과의 차이점
>   + 검색은 소비자가 관심사를 표현하는 "검색"이라는 행위를 해야함 
>   + 추천은 특별한 행위 없이도 정보 전달이 가능 (passive)
> + 추천 시스템의 분류 중 사용할 방식
>   +  업데이트 주기에 따른 분류
>       + 정적 추천 시스템(Offline) :  특정 시점의 데이터를 사용해 추천 결과를 계산하는 방식
>       + 동적 추천 시스템(Online) :  지속적으로 사용자의 데이터를 받아 추천 결과를 업데이트 하는 방식
>       + 현업에서는 다양한 추천 로직이 섞인 하이브리드 추천 시스템을 많이 사용

### 1-3 추천 알고리즘
> + 콘텐츠 기반 필터링(content based filtering)
>   + 콘텐츠 정보를 분석하거나, 정리된 메타 정보를 활용해 콘텐츠별로 특징 정보를 만들고 이를 활용해 추천
>   +	즉, 사용자가 특정 아이템을 선호하는 경우 그 아이템과 비슷한 콘텐츠를 가진 다른 아이템을 추천해주는 방식
>   + 굉장히 단순한 아이디어
>   + 예를들어 사용자 A가 itemA에 굉장히 높은 평점을 주었는데 그 item이 액션영화이며 '봉준호'라는 감독이었으면 '봉준호'감독의 다른 액션 영화를 추천해주는 것
>   + 추천 시스템의 기본적인 알고리즘

## 2. 데이터 수집 및 분석 개요
### 2-1 데이터 수집 대상
> + Movielens의 영화 평점 데이터
### 2-2 데이터 수집 방법
> + Movielens DataSet
## 3. 데이터 읽고 기초 분석
### 3-1 개봉연도 분석(1_Movies.ipynb)
### 3-2 개봉연도 시각화
### 3-3 장르 분석
### 3-4 텍스트 데이터를 숫자형으로 변환
### 3-5 장르 간 관계 찾기와 시각화
### 3-6 기초 통계(2_ratings.ipynb)
### 3-7 평점의 분포
### 3-8 유저별 평점 패턴 분석
### 3-9 나의 평점 데이터 기록

## 4. 간단한 추천 시스템 만들기(Simple_Recommendation.ipynb)
### 4-1 평가지표 RMSE
### 4-2 학습 데이터와 평가 데이터
### 4-3 가장 간단한 예측하기
### 4-4 예측 예제 문제 풀이

## 5. Content based filtering을 이용한 평점 예측 및 모델 평가(Content_Based_Recommendation_v1.ipynb)
### 5-1 데이터 전처리
### 5-2 유저 프로필 만들기
### 5-3 샘플 유져의 평점 예측
### 5-4 전체 유저의 평점 예측과 모델 평가

## 6. Linear Regression(선형회귀)를 이용한 평점 및 예측 및 모델 평가(Content_Based_Recommendation_v2.ipynb)
### 6-1 샘플 유저의 평점을 학습 데이터와 평가 데이터로 나누기
### 6-2 샘플 유저의 프로필 만들기
### 6-3 전체 유저의 평점 예측과 모델 평가
### 6-4 오버피팅
### 6-5 Lasso 모델 적용

## 7. 나와 친구를 위한 영화 추천 (Content_Based_Recommendation_v3.ipynb)
### 7-1 나의 데이터 EDA
### 7-2 나와 친구의 데이터 EDA
### 7-3 Lasso 하이퍼 파라미터 튜닝
