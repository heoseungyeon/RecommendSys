# RecommendSys_server_django
2020-1 창의학기제  프로젝트 : 딥러닝 기반  장소 추천 시스템  - DjangoServer 

## 프로젝트 개요

---

- NOLLE는 Notifiy only likes, Let’s enjoy로 좋아하는걸 알리고 같이 나누자라는 의미입니다.
- 창의학기제 과목으로 진행한 딥러닝 기반 개인화 맛집 추천 서비스입니다.
- 밀레니얼 세대의 관심사 공유하고자 하는 특징에  착안하여  Vertical형 SNS를 개발하고자 하였습니다.
- 사용자가 업로드한 음식점 리뷰에 대한 이미지와 텍스트, 검색 기록 등을 딥러닝으로 분석하여 성향을 추출 후 나와 유사도가 높은 다른 사용자가 갔던 음식점을 추천합니다.
- Yolov3 모델의 경우 총 42가지의 한식, 일식, 중식, 양식 음식에 대한 분류가 가능하며 객체인식 모델 정확성 평가의 경우 TOP-1 정확도 88.61%, TOP-5 정확도 90.13%를 보여주었습니다.
- BiLSTM을 이용하여 구현한 감성분석 모델의 경우 음식에 대한 표현과 장소에 대한 분위기를 범주에 나눠 총 14가지의 텍스트 분류가 가능하며 F1-Score은 90.93%, Accuracy는 90.99%를 보여주었습니다.

## 프로젝트 사용 기술 및 라이브러리

---

### ✔️Language

- Java, Python

### ✔️Server

- Django

### ✔ Client

- Android

### ✔ 협업

- GitHub

### ✔ Data Base

- MySQL

### ✔ Open API

- Naver Blog Search API
- Google Maps API

### ✔ Library

- Retrofit2

### ✔ Deep-Learning

- Yolov3 (Tensorflow)
- BiLSTM (Tensorflow)

## 주요 기능

---

- 딥러닝 기반 성향 분석 및 성향 기반 추천
- 텍스트, 음성, 이미지로 다양하고 간편한 검색 및 추천 요청
- 실시간 리뷰, 인기 리뷰 및 태그를 통한 추천
- 사용자가 가고 싶은 장소를 저장하는 PICK
- SNS의 순기능인 팔로우, 팔로잉, 좋아요 및 포스팅 기능

## 나의 역할

---

- Android 구현
    - Google MAP API를 활용한 지도 화면
    - Google STT API를 활용한 검색 화면
- Django 백엔드 API 서버 구현
    - Feed, Posting, Map, Place_detail, Pick API 개발
- 딥러닝 모델 구현을 위한 데이터 수집 및 정제
    - 감성 카테고리 체계 구축
    - 형태소 분석기를 활용한 자연어 처리
- AWS EC2 Ubuntu 서버 / MySQL 서버 구축
- Platform 형태 전체 시스템 구조 설계
