ExtraTrees, KNeighbors, SVC, Randomforest 이렇게 4가지 분류 모델을 사용하였다.
그리고 classifier들을 결과값의 확률을 평균을 내는 soft voting 함으로써 성능을 높였다.
hyperparameter를 바꾸어 각각의 classifier들의 정확도를 높였고 그 중 n_jobs=-1을 사용하여 머신러닝할 때 모든 코어의 개수를 사용하게 했다.
또한, n_estimators의 수를 높여 결정트리 개수를 늘렸다.
