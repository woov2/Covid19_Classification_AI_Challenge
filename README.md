# Covid19 Classification AI Challenge
### 코로나19 음성 예측 AI 개발

## 1. MFCC Vector 추출
* 데이터의 다양성을 위해 추출할 MFCC 벡터의 개수를 16,32,64개로 설정
## 2. Data Augmentation
* Audio Data Augmentation 기법 중 shifting 방법을 사용
## 3. Data Pre-processing
* gender column에 one-hot-encoding 적용
* 최종적으로 만들어진 feature value에 절대값 적용
## 4. Pseudo Labeling
* unlabeled dataset을 이용해 pseudo-labeling을 적용
## 5. Model
* ExtraTreesClassifier
## 6. Training
* Feature set : 총 3가지의 feature set(vector count에 따라)
* KFOLD(K=10)
## 7. Inference
* Feature set : 총 3가지의 feature set(vector count에 따라)
* KFOLD(K=10)
## 8. Score(Macro-F1)
* Public(0.62286) 8th
* Private(0.60138) 10th
