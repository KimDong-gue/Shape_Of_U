# ○ Subject: Shape_Of_U
 성인 여성의 얼굴형에 따른  헤어스타일 추천 모델

# ○ Contributer
팀원|역할|
------------|-----------------------
배진혜(팀장) | 서비스 기획, 데이터 수집 
　　　　　　　| 모델링, PPT제작   
김동신(팀원) | 서비스 기획, 데이터 수집         
　　　　　　　|  모델링, PPT제작              
이우성(팀원) | 데이터 수집, PPT 제작

## Skills : Augmentation, Face Dectection , CallBacks(Early Stopping, ReduceLROnPlateau) , Fine tuning , Bacth_normalization, Drop_out

## Model : Resnet50

### Dataset: https://www.kaggle.com/datasets/niten19/face-shape-dataset/data

### ProjectSchdule: 23/10/11 ~ 23/10/29 (약 3주)

***

# 기획

![image](https://github.com/KimDong-gue/Shape_Of_U_/assets/116249934/9104118b-9775-4397-92f3-d14ee8adb5b4)

- 얼굴형을 알면 쉽게 스타일링이 가능하다.

***

# FlowChart

![image](https://github.com/KimDong-gue/Shape_Of_U_/assets/116249934/761a018f-78bf-44c0-bfce-188910124ada)

***

# 성능개선노력

- Drop out을 층에 적게 주면 리소스 부족 문제가 발생
- Batch Normalization과 Drop out을 해주면 
Overfitting 방지로 성능이 올라감을 느낌
- Drop out은 앞에 층에서 크게 주고, 
뒤 은닉층으로 갈수록 작게 줘야 한다는 것을 느낌
- 데이터 핸들링 (Face Dectection, Augmentation)
- 모델 핸들링 (Fine tuning)

# Model 선정이유

- 마이크로소프트에서 제안하고 2015년 이미지넷에서 우승한 모델
- 50개 계층으로 구성된 컨벌루션 신경망
- 최근까지 가장 많이 사용됨
- ImageNet 데이터베이스의 1백만 개가 넘는 이미지에 대해 훈련된 신경망의 사전 훈련된 버전을 불러올 수 있음

***

# Model Evaluation

![image](https://github.com/KimDong-gue/Shape_Of_U_/assets/116249934/94d9b34e-c4b1-43ee-a850-3d48aa224196)
