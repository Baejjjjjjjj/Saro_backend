# SARO

## Safe RoadMap: 시각장애인 보행 안내 서비스

> SARO는 음향신호기를 이용하는 길 안내와 AI를 이용한 보행 장애물 판단 기능을 통해 
시각장애인을 위한 보행 안내 서비스를 제공합니다.
> 

## 📷시연 연상

---

아래 영상을 클릭해 SARO의 시연 영상을 확인해주세요. 

## 👋🏻 프로젝트 소개

---

## 1️⃣ 개발 배경

- 시각장애인 보행 안전실태조사(2020.12)월에 따르면 시각장애인 중 50%는 보행에 필요한 편의시설 부족으로 인해 외출에 불편함을 느끼고 있다. 또한, 시각장애인이 이용하는 교통수단은 장애인 택시 제외 도보가 약 23%로 높은 비중을 차지하고 있다.
- 서울 시 교통안전시설물관리시스템에 따르면 서울시에 존재하는 비신호 횡단보도의 경우 약 2만 6000개 이상으로 실제로 많은 비신호 횡단보도를 사용해야만한다.
- 2021년 실시한 장애인보도환경 실태조사 결과 점자블록 파손, 보도블록 파손에 의한 시설 불편이 약 40%, 음향 신호기 부족으로 인한 시설 불편이 약 20%로 해당 시설물들의 정비의 필요성이 대두되고 있다.

## 2️⃣ 개발 목적

- 보행에서의 어려움을 인지하고 보도환경에 있어서 시설 파손을 감지하고 예방하도록 해 시설 불편을 감소시키며 음향 신호기로 이루어진 길안내 기능을 통해 보다 안전한 환경에서의 보행을 돕기 위한 것이 본 서비스의 목적이다.

## ⚒️ 시스템 구성 및 아키텍처

---

### 클라우드 기반 아키텍처

- 클라우드 프로바이더: AWS, Google Cloud Platform
- CI/CD 파이프라인 구축

### 웹 어플리케이션 아키텍처

- 웹 서버: Apache
- 애플리케이션 서버: Node.js + Express 로 구축
- 데이터베이스 서버: MySQL
- 클라이언트: Web Brower

## 🪖적용 기술

---

### 1️⃣ 개발 환경
<img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=Linux&logoColor=111111"/> | <img src="https://img.shields.io/badge/windows10-0078D4?style=flat-square&logo=windows10&logoColor=111111"/>

 WINDOW11, WINDOW10

### 2️⃣ 개발 도구

VISUAL STUDIO CODE, MYSQL, DataGrip, AQuery

### 3️⃣ 개발 언어

JAVASCRIPT, CSS, HTML

## 🎁 프로젝트 기능

---

### 1️⃣ 음향 신호기 도보 길 안내 기능

- 출발지& 목적지 입력
    - 현재 위치 자동 입력
    - 음성 인식 등을 통한 입력
- 길 안내 로직 선택
    - 최소 시간, 큰길 우선, 안전 우선, 최소 도보 중 하나의 로직을 선택
- 음향신호기 길 안내 서비스 로직
    - 일반 횡단보도 대신 음향신호기가 설치 되어 있는 횡단보도로 길 안내를 진행한다.
    - 단, 일부 횡단보도의 경우 기존 신호기로 안내를 진행한다.
    - 건널목, 장애물, 계단 등의 경우 위험 신호를 통해 알려준다.
- 지도 UI
    - 실제로 확인 가능 하도록 경로를 보여준다.
    - 전체 경로의 요약정보를 확인 가능하다.
- 음성 안내 기능
    - 사용자의 위치에 따라 음성으로 길을 안내한다.
    - 음성 다시 듣기, 음성 중지 가능

### 2️⃣ 음향 신호기 대중교통 안내 기능

- 음향신호기 도보 길 안내 기능 포함 추가 기능들 제공
- 버스, 지하철, 버스& 지하철을 포함한 길 안내 기능 제공
- 버스 도착 정보 안내 기능, 지하철 도착 정보 안내 기능 포함

### 3️⃣ 버스 도착 정보 안내 기능

- 경로 상의 탑승 가능한 버스들에 대해 도착 정보를 알려 준다.
    - 각 버스 당 현재 남은 정류장 개수, 남은 시간, 운행 종료 여부 등을 알려준다

### 4️⃣ 지하철 도착 정보 안내 기능

- 경로 상의 탑승 가능한 지하철에 대해 도착 정보를 알려준다.
    - 해당 지하철에 대해 현재 남은 역 등의 정보를 알려준다.

### 5️⃣ AI기반 보도 상태 분석 기능

•  보행 중 느껴지는 점자 블록 파손, 보도 블록 파손, 각종 장애물, 인도 위 차량 등에 대해 카메라로 사진을 찍고 사진을 등록 시 AI를 기반으로 해당 물체 혹은 보도 상태를 분석해 준다.

### 6️⃣ 신고 기능

•  앞선 AI 분석 이후 보행에 방해되는 물체 혹은 파손이 느껴질 경우 신고하기 버튼을 통해 신고 의사를 밝힐 수 있다.

### 7️⃣ 음성 안내 기능

•  자동 재생, 클릭을 통해 음성으로 서비스를 안내 받을 수 있다. 
****

## 🎨 최종 화면

---

- 안내 화면

![화면_캡처_2023-09-07_223603](/uploads/1cd596d5d335a46ec989473cb0c2c7b5/화면_캡처_2023-09-07_223603.png) | ![화면_캡처_2023-09-07_223707](/uploads/d5e78d9dbfe1634de94fdcd6811dd8b5/화면_캡처_2023-09-07_223707.png) |![55](/uploads/8879a2ef4becbbd6ff59db8c36cb908d/55.png)
--- | --- | --- |

- 길 안내 서비스

![KakaoTalk_20230907_222837389_04](/uploads/f127fc4194d8f9a13885a2f5f0cc65fb/KakaoTalk_20230907_222837389_04.png) | ![KakaoTalk_20230907_222837389](/uploads/61626d2e08fc70b777477ba31bd248f0/KakaoTalk_20230907_222837389.png) | ![KakaoTalk_20230907_222837389_01](/uploads/c502806391ffdcd28f586abf64d9358e/KakaoTalk_20230907_222837389_01.png)
--- | --- | --- |

![KakaoTalk_20230907_222837389_02__1_](/uploads/026cbec57e79c50ac3e5ffa8438a951a/KakaoTalk_20230907_222837389_02__1_.png) | ![KakaoTalk_20230907_222837389_03__1_](/uploads/3b8fa81d788fa63711c714525d883a60/KakaoTalk_20230907_222837389_03__1_.png) | ![KakaoTalk_20230907_224704660](/uploads/12e4af3cc60eaaf90cbfbc2e605c0541/KakaoTalk_20230907_224704660.png)
--- | --- |  --- |


## 🌺 기대 효과

---

### 1️⃣  기대효과 - 사회 경제적 측면

- 시각장애인들의 안전한 보행을 도와 사고율을 절감하며 원활한 일상생활을 도와 건강과 삶의 질 향상에 크게 기여 가능하다.
- 추가적인 음향신호기 건설 대신 기존의 음향신호기를 효율적으로 사용해 사회적 비용을 절감할 수 있다.
- 보행 장애물에 대한 빠른 신고를 통해 추후 발생할 수 있는 사고를 예방해 비장애인 포함 안전한 보행에 기여 가능하다.

### 2️⃣ 기대효과 - 사용자 측면

- 신호 상태를 확인할 수 없는 일반 횡단보도 대신 음성으로 안내 받을 수 있는 음향신호기를 사용해 보다 훨씬 안전한 보행이 가능하다.
- 계단, 건널목 등의 시설을 미리 파악하고 부딪힘 사고 등을 예방할 수 있다.
- 보행 시 느껴지는 장애물에 대해 직접적으로 판별할 수 있다.
- 시각장애인의 보행권 개선
