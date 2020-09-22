# XGBoost-for-gait-analysis
XGBoost 알고리즘을 활용하여 보행 분석에 사용하는 코드입니다.


## 라이브러리
Python 3.8.3 에서 작동을 확인하였으며
사용된 라이브러리로는 xgboost, pandas, sklearn, shap 라이브러리를 활용하였습니다.


## 사용방법
동일 폴더에 있는 csv 파일을 불러들여서 작업을 하는 구조이며
Vicon 사의 Nexus 프로그램을 활용하여 plug in gait 모델을 바탕으로
계단 보행을 하는 데이터를 전처리 후 활용해서 분석을 하였습니다.
사용된 데이터는 각각의 부분에 대해서 최대치, 평균치, 1st half의 최대치, 2nd half의 최대치를 사용하였습니다.
해당 코드에서 hr_df = pd.read_csv("파일이름.csf")와 colnames를 수정한다면 통상적인 엑셀 파일의 XGBoost에도 사용할 수 있습니다.
