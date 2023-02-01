# Dacon [월간 데이콘 음향 데이터 COVID-19 검출 AI 경진대회](https://dacon.io/competitions/official/235910/overview/description)에서 진행된 코드입니다.
## MFCC Vector 추출
* 데이터의 다양성을 위해 추출할 MFCC 벡터의 개수를 16,32,64개로 설정
## Data Augmentation
* Audio Data Augmentation 기법 중 shifting 방법을 사용
## Data Pre-processing
* gender columns에 one-hot-encoding 적용
* 최종적으로 만들어진 feature value에 절대값 적용
## Pseudo Labeling
* unlabeled dataset을 이용해 pseudo-labeling을 적용
## Model
* ExtraTreesClassifier
## Training
* Feature set : 총 3가지의 feature set(vector count에 따라)
* KFOLD(K=10)
## Inference
* Feature set : 총 3가지의 feature set(vector count에 따라)
* KFOLD(K=10)
## Score(Macro-F1)
* Public(0.62286) 8th
* Private(0.60138) 10th
