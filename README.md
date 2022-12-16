sklearn에 존재하는 분류 모델 중 fit 메소드를 사용하여 개별 훈련 시켰을 때 정확도가 90 이상 나오는 classifier들을 선정하였다.
그 결과, NuSVC,ExtraTrees, KNeighbors, SVC, Randomforest,HistGradientBoosting 이렇게 6가지 분류 모델을 사용하였다.
각각의 모델들이 결과를 예측하면 단순하게 가장 많은 표를 얻은 결과를 선택하는 hard voting을 사용하여 성능을 높였다.
hyperparameter를 바꾸어 각각의 classifier들의 정확도를 높였고 그 중 n_jobs=-1을 사용하여 머신러닝할 때 모든 코어의 개수를 사용하게 했다.
n_estimators의 수를 높여 결정트리 개수를 늘렸고 random_state를 고정하여 호출할 때 마다 동일한 학습 데이터 세트를 생성하게 했다. 
