# ML_DL_Project 

### 이 물은 먹을 수 있는 물..?
<br>

## 👉 USE

- <img src="https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white"> <img src="https://img.shields.io/badge/Numpy-F013243.svg?style=for-the-badge&logo=Numpy&logoColor=white"> <img src="https://img.shields.io/badge/Pandas-F150458.svg?style=for-the-badge&logo=Pandas&logoColor=white"> <img src="https://img.shields.io/badge/TensorFlow-FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white">

- <img src="https://img.shields.io/badge/Jupyter-F37626.svg?style=for-the-badge&logo=Jupyter&logoColor=white">



Kaggle 사이트 에서 수질검사 관련 데이터를 찾아보았다

![스크린샷 2022-11-16 오전 12 36 28](https://user-images.githubusercontent.com/105684835/201960881-eeff1207-43d1-4daa-b1cb-7c156c58aafb.png)

<br>

![스크린샷 2022-11-16 오전 12 57 38](https://user-images.githubusercontent.com/105684835/201966103-ee348dab-34c9-441f-98fa-c695ed92fc5e.png)

데이터를 불러와 예측하려는 모델을 위해서는 어떤 컬럼이 필요한지 인터넷 검색, 팀원들과의 회의 후 결정하여 ETL을 진행하기로 하였다
<br>



<br>

![스크린샷 2022-11-16 오전 1 04 03](https://user-images.githubusercontent.com/105684835/201967610-17125d83-606c-41cd-8dc9-496141b170e5.png)

상관관계 확인

<br>

![스크린샷 2022-11-16 오전 1 11 54](https://user-images.githubusercontent.com/105684835/201969542-cf81dd54-2f8d-4820-88f0-46ea5a45353d.png)
![스크린샷 2022-11-16 오전 1 12 30](https://user-images.githubusercontent.com/105684835/201969656-9035d1de-06e0-4dc5-b142-f13e878d2942.png)
![스크린샷 2022-11-16 오전 1 13 12](https://user-images.githubusercontent.com/105684835/201969840-0aa4d712-c113-4049-b16a-735df35831da.png)
![스크린샷 2022-11-16 오전 1 13 30](https://user-images.githubusercontent.com/105684835/201969908-c62454a7-e143-4c01-a3d7-10d0634079b2.png)

양극단으로 튀는 데이터들이 생각보다 많다..?

<br>

## 결측치 처리

<br>

![스크린샷 2022-11-16 오전 1 27 45](https://user-images.githubusercontent.com/105684835/201973472-adf7ac10-42f3-426e-80b7-e357371cbf4d.png)

<br>

![스크린샷 2022-11-16 오전 1 36 18](https://user-images.githubusercontent.com/105684835/201975315-934b2661-95e1-4d5b-842a-493058c24e02.png)

머신러닝 전 전처리

<br>

## Machine Learning

<br>

![스크린샷 2022-11-16 오전 1 39 59](https://user-images.githubusercontent.com/105684835/201976193-37164ab2-c19e-4fa6-96b8-96fcaa497e4b.png)

랜덤포레스트가 젤 높다!

<br>

![스크린샷 2022-11-16 오전 1 44 45](https://user-images.githubusercontent.com/105684835/201977329-5be1554e-50d7-40b7-9762-8a3d6d3f16d4.png)

<br>

![스크린샷 2022-11-16 오전 1 46 57](https://user-images.githubusercontent.com/105684835/201977839-29163e95-1c2e-4336-806c-c1d4b991463c.png)

최대한 높여보는중...

<br>

![스크린샷 2022-11-16 오전 1 47 54](https://user-images.githubusercontent.com/105684835/201978077-77796e6a-7124-461a-abce-9a45807876a4.png)

![스크린샷 2022-11-16 오전 1 48 01](https://user-images.githubusercontent.com/105684835/201978096-8a292648-bf9b-4535-89d6-deafa843600a.png)

아주 이쁜 이진분류 그래프가 나왔다!

<br>

![스크린샷 2022-11-16 오전 1 48 20](https://user-images.githubusercontent.com/105684835/201978195-a71cd798-ee51-4be3-9a74-e362b46e1f51.png)

나의 생각으론 PH가 젤 관계가 높을줄 알았는데 아니였다 sulfate(황산염) 이 제일 중요한걸로!

<br>

## Deep Learning

<br>

![스크린샷 2022-11-16 오전 1 55 13](https://user-images.githubusercontent.com/105684835/201979593-b5e01077-cdb5-44d8-9b4d-84742c4b08e0.png)

드디어 TenserFlow 사용!

<br>

![스크린샷 2022-11-16 오전 1 57 23](https://user-images.githubusercontent.com/105684835/201980057-13ab63bf-805a-452f-bb59-f11363e432d7.png)

하이퍼 파라미터 설정해주고 train, test set으로 나누기

<br>

![스크린샷 2022-11-16 오전 1 59 25](https://user-images.githubusercontent.com/105684835/201980482-a7e2d20d-e9b9-410e-8be2-e2d0f0ddd989.png)

Scaled, transform 처리

<br>

![스크린샷 2022-11-16 오전 2 04 25](https://user-images.githubusercontent.com/105684835/201981490-e0e54214-9208-4fe4-839a-c86fcf1b32fa.png)

train set 을 위한 dataset 생성

<br>

![스크린샷 2022-11-16 오전 2 05 09](https://user-images.githubusercontent.com/105684835/201981656-5a47e4f1-7d64-41fd-91d5-4ebefd966a60.png)

모델 생성

<br>

![스크린샷 2022-11-16 오전 2 05 46](https://user-images.githubusercontent.com/105684835/201981794-33eecb8e-6ec4-42f1-bcea-141307620dba.png)

학습 하는중!

<br>

![스크린샷 2022-11-16 오전 2 06 46](https://user-images.githubusercontent.com/105684835/201981994-903bebf1-d45b-4575-8242-b41accbd6e67.png)

에폭을 늘리니 loss 값이 줄긴 한다만... 머신러닝 할때가 더 값이좋았다 아마 그 이유는 딥러닝 하기에는 부족한 데이터수가 아닐까 생각한다.
