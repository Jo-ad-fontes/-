# 2021 주식 종가예측 대회 11.10 ~ 11.29

## public 4위 → private 43위

FinanceDataReader 패키지를 통해서 국내 및 해외 주식의 정보를 얻을 수 있었다.  [FinanceDataReader 사용법](https://financedata.github.io/posts/finance-data-reader-users-guide.html)

원달러 환율, 비트코인, 증권거래소 관련 정보도 존재한다.

대회는 KOSPI-200과 KOSDAQ-150의 주어진 기간 중 마지막으로 거래된 가격(종가) 예측하는 것이 었는데, 종목이 많다보니 빠르고 성능좋은 LGBM을 사용하였다.

feature engineering 부분에서 이전 날 정보를 주는 부분이 오히려 결과예측에 안좋은 영향을 미친 것 같다. 
