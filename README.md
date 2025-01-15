# 중고땅땅 - 중고물품 경매입찰 시스템

<p align="center">
  <img src="/docs/ic_JTT.png"/>
</p>


**중고땅땅**은 사용자가 중고물품의 가치를 잘 모를 경우, 경매 시스템을 통해 공정한 가격으로 물품을 판매할 수 있도록 돕는 서비스입니다.  
중고 거래 시장의 문제점을 해결하고 사용자들에게 더 나은 거래 환경을 제공합니다.

<br>

## 📑 목차
1. [개발 인원](#-개발-인원)
2. [팀원별 역할](#-팀원별-역할)
3. [개발 환경](#-개발-환경)
4. [시스템 구성도](#-시스템-구성도)
5. [주요 기능](#-주요-기능)
6. [프로젝트 수행 기간 및 개발 일정](#-프로젝트-수행-기간-및-개발-일정)
7. [참고 자료 및 사용 도구](#-참고-자료-및-사용-도구)
8. [배운 점 및 회고](#-배운-점-및-회고)
9. [문서 및 자료](#-문서-및-자료)

<br>

## 👥 개발 인원

<div align="center">

| 조경남 | 최진웅 | 신상민 | 이명기 |
|:---:|:---:|:---:|:---:|
| <img src="https://avatars.githubusercontent.com/u/63902992?v=4" height="150" width="150"> <br> [@GyeongNam](https://github.com/GyeongNam) | <img src="https://avatars.githubusercontent.com/u/64189518?v=4" height="150" width="150"> <br>[@dorumamu](https://github.com/dorumamu) | <img src="https://avatars.githubusercontent.com/u/62735118?v=4" height="150" width="150"> <br>[@zztto1](https://github.com/zztto1) | <img src="https://avatars.githubusercontent.com/u/64415555?v=4" height="150" width="150"> <br>[@toropong](https://github.com/toropong) |

</div>

<br>

## 🔧 팀원별 역할

### 조경남
- **개발환경 구축** 및 **DB 구조 설계** 
- **채팅 서비스** 개발
- **낙찰 시스템** 개발

### 이명기
- **통계 서비스** 개발
- **관리자 사이트** 개발

### 신상민
- **관리자 사이트** 개발 
- **회원 관리 서비스** 개발

### 최진웅
- **위치 기반 서비스** 개발
- **게시판 서비스** 개발

<br>

## ⚙️ 개발 환경

![CI/CD](https://img.shields.io/badge/CI%2FCD-Enabled-brightgreen)
![운영체제](https://img.shields.io/badge/OS-CentOS%206.10-blue)
![웹 서버](https://img.shields.io/badge/웹%20서버-Apache%202.2.15-orange)
![데이터베이스](https://img.shields.io/badge/DB-MySQL%205.1.73-blue)
![프레임워크](https://img.shields.io/badge/Framework-Laravel%207.10.3-lightgrey)
![언어](https://img.shields.io/badge/언어-PHP%2C%20HTML%2C%20CSS%2C%20JavaScript%2C%20jQuery-yellow)

<br>

## 🖼 시스템 구성도

<p align="center">
  <img src="https://user-images.githubusercontent.com/63902992/143731056-401abcd5-d72e-46ac-8a95-096aa6ccfee2.png"/>
</p>

<br>

## 🛠 주요 기능

1. **경매 서비스**
    - 판매자가 물품을 등록하고 구매자가 경매를 통해 입찰.
    - **타이머** 기능: 경매 시작과 종료 시간 설정, 경매 종료 시 자동으로 낙찰자 결정.
    - **스케줄러** 기능: 경매 종료 시간에 맞춰 자동으로 낙찰자가 결정되고, **Laravel 스케줄러**를 사용하여 경매 상태 업데이트.
    - 낙찰된 물품은 구매자와 판매자 간 거래로 연결.


2. **회원 관리**
    - 사용자별 정보 저장 및 수정.
    - 관리자 페이지를 통해 회원 관리 및 경고 기능 제공.


3. **채팅 서비스**
    - 판매자와 구매자가 실시간으로 소통할 수 있는 **채팅 시스템** 제공.
    - **웹소켓**과 **Pusher**를 이용한 실시간 메시지 전달.


4. **통계 및 데이터 분석**
    - 관리자 페이지에서 거래 통계, 방문자 수, 경매 현황 확인.
    - **구글 애널리틱스**를 사용하여 사이트 접속자 수 및 이용 현황을 분석.


5. **위치 기반 서비스**
    - **카카오 지도 API**를 이용하여 경매 물품의 위치를 지도에서 확인하고, 사용자가 반경 내 가까운 경매를 찾아볼 수 있는 기능 제공.

<br>    

## 📅 프로젝트 수행 기간 및 개발 일정
- **총 개발 기간**: 16주
- **주요 일정**:
    1. 아이디어 구상 및 기획 (1~2주차)
    2. 데이터베이스 설계 및 초기 화면 구성 (3~6주차)
    3. 기능 개발 (7~14주차)
    4. 테스트 및 배포 (15~16주차)

<br>

## 📚 참고 자료 및 사용 도구

- **Laravel 문서**: [laravel.7.x](https://laravel.kr/docs/7.x)
- **Pusher 채널**: [pusher](https://pusher.com/channels)
- **구글 애널리틱스**: [Google Analytics](https://analytics.google.com)
- **카카오 지도 API**: [Kakao Maps](https://developers.kakao.com/docs/latest/ko/map)

<br>

## ✨ 배운 점 및 회고

- **협업의 중요성**: 팀원 간 원활한 소통과 협력이 프로젝트 성공의 핵심임을 깨달음.
- **기술 학습**: Laravel 프레임워크와 PHP를 활용하여 MVC 구조의 효율성을 경험.
- **문제 해결 능력**: 실제 중고 거래 시스템의 요구사항을 분석하고 해결 방안을 제시하는 역량 강화.

<br>

## 📂 문서 및 자료

- **[스토리보드](./docs/스토리보드.pptx)**
- **[발표자료](./docs/중고땅땅%20발표자료.pptx)**
