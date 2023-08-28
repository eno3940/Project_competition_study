[KDT_AI-프로젝트공모전스터디-1과제](https://www.kaggle.com/competitions/kdtai-1/)

# 과제설명

# Task

코로나 19의 발생도 어연 4년차입니다. 인공지능을 코로나 19 상황에 적용하고자 하는 주제는 산업 전반 및 연구 분야에서 꾸준하게 시도되어왔습니다. 우리는 **수천장의 xray data를 토대로, 임의의 환자의 xray 사진을 토대로 이 환자의 코로나 19 감염 여부를 판단할 수 있는 ML 모델을 수립**하는 것이 목표가 됩니다.

# Dataset Description

본 데이터셋은 총 2400장의 png 이미지 데이터로 구성되어 있습니다. 모든 이미지 파일은 299 x 299 픽셀로 이루어져 있습니다.

## **Files**

- **train** - train 데이터가 담긴 파일입니다. 2000장의 png 파일 및 이들의 label 정보를 담은 label.csv파일로 구성되어 있습니다.
- **test** - test 데이터가 담긴 파일입니다. 400장의 png 파일이 저장되어 있습니다.
- **submission.csv** - 올바른 포맷으로 지정된 submission 파일입니다.
- **labels - sample.csv** - submission 파일의 예시입니다. 본 파일에서는 모든 케이스에 대해 normal로 분류되었습니다. 모든 train 데이터와 test 데이터의 category 비율이 1:1이므로, 본 csv파일을 제출하면 0.5의 점수를 받게 됩니다.

## **Columns**

- `filename` - 파일의 이름을 나타냅니다.
- `label` - 해당 filename의 file이 해당하는 label을 나타냅니다. normal, covid로 구성되어 있습니다.
    
    

# Evaluation

본 binary classification 문제는 accuracy 메트릭을 사용합니다. (https://en.wikipedia.org/wiki/Accuracy_and_precision). 단순하게 생각해서, 테스트 데이터 400장을 올바르게 분류할수록 score가 높아집니다. 400장을 모두 올바르게 판단할 경우 1.0, 모두 틀릴 경우 0.0의 스코어를 받게 됩니다.



# 결과 및 후기

첫 과제로 몸풀기 용으로 선정한 듯 하다.

이진분류에 간단한 task라 torchvision으로 간략하게 Resnet50으로 돌리고 제출해 봤는데 스코어1.00달성. 데이터셋이 너무 정직한 듯 하다.

공동 1위이나 f반이 더 빨리내서 다음번 대회 Dataset은 f반이 고르는걸로 되었다.
![image](https://github.com/eno3940/Project_competition_study/assets/98100556/1468dfbe-7562-4b60-93ca-11037376b99c)
