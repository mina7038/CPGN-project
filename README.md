# Spring Boot-React 프로젝트 - 꼼파뇨 스튜디오

<div align="center">
    <img width="400" height="176" alt="꼼파뇨스튜디오 jpg" src="https://github.com/user-attachments/assets/41d13135-97eb-4812-96e6-9a8a88c05b68" />
</div>

## 목차

- [개요](https://github.com/mina7038/CPGN-project#-개요)
- [기술 스택](https://github.com/mina7038/CPGN-project#-기술-스택)
- [프로젝트 설계](https://github.com/mina7038/CPGN-project#-프로젝트-설계)
- [주요 기능](https://github.com/mina7038/CPGN-project#-주요-기능)
- [기능 구현](https://github.com/mina7038/CPGN-project#-기능-구현)

## **🚩 개요**

- **프로젝트 목표**
    - **Spring Boot + React** 기반의 풀스택 웹 애플리케이션 개발
    - 사용자 중심의 쇼핑 경험을 위해 회원가입, 로그인, 장바구니, 결제, 리뷰 등 전반적인 커머스 기능 구현
- **진행 기간** : 2025.06.09 ~ 2025.06.23 (2주일)

## **🛠️ 기술 스택**

- Language: `Java (17)`, `JavaScript (ES6)`
- Framework: `Spring Boot (3.x)`, `React`, `Spring Data JPA`
- Database: `MySQL (8.0)`
- Server: `AWS EC2`, `Docker`
- Tool: `IntelliJ IDEA`, `Git`
- API: `Google OAuth 2.0`, `TossPayments`

## **📝 프로젝트 설계**
- **요구사항 정의서**

    <img width="1223" height="540" alt="image" src="https://github.com/user-attachments/assets/d56df965-910a-4943-b2e4-5a8879cf6f8a" />
    
- **유스케이스 명세서**

    <img width="1230" height="635" alt="image" src="https://github.com/user-attachments/assets/b9565ff7-dc6d-48e1-a926-dbde2fc8fef1" />
    <img width="1227" height="637" alt="image" src="https://github.com/user-attachments/assets/109e03ef-fdf0-435e-8353-e713c68afac0" />
    
- **ERD**

    <img width="1123" height="634" alt="image" src="https://github.com/user-attachments/assets/5f01af5d-70d5-4c74-b984-82178d73d4cb" />




## **✨ 주요 기능**

### 1️⃣ Google 로그인

- **Google OAuth 2.0**
    - Google OAuth 2.0 연동을 통해 Google 계정으로 손쉽게 로그인할 수 있습니다.

    <img width="380" height="950" alt="image" src="https://github.com/user-attachments/assets/c80dfa2e-c62c-452d-832e-a043559a8c4f" />
    <img width="380" height="950" alt="image 1" src="https://github.com/user-attachments/assets/c26d67fa-b492-4d60-b228-b49b69be9c16" />


### 2️⃣ Toss Pay 결제

- **TossPayments API**
    - TossPayments API를 통해 카드, 계좌이체, 간편결제 등 다양한 결제 수단으로 쉽고 안전하게 결제할 수 있습니다.

    <img width="380" height="950" alt="image 2" src="https://github.com/user-attachments/assets/26fcc8f8-2873-4c57-960c-dd51fc8f501a" />
    <img width="380" height="955" alt="image 3" src="https://github.com/user-attachments/assets/70c14e9e-afe7-4a18-a2df-9735fc38523b" />

### 3️⃣ 리뷰 요약 mp3 생성
- **OpenAI TTS**
    - OpenAI TTS를 활용해 리뷰를 요약하고 mp3 파일로 변환하여, 상품 상세 페이지에서 음성으로 리뷰를 들을 수 있습니다.

    <img width="380" height="951" alt="image" src="https://github.com/user-attachments/assets/611d69f9-68e6-4ce9-8296-7f06f445f911" />
    <img width="380" height="951" alt="image" src="https://github.com/user-attachments/assets/29a10b28-781c-4475-8a8d-e559087f9db5" />




## **🎬 기능 구현**

### ✔ 회원가입/로그인
- **아이디 중복 체크**: 기존 사용자와 중복 여부 확인 후 안내.
- **비밀번호 확인**: 비밀번호/확인 값 일치 검증 및 오류 메시지 처리.
- **이메일 인증**: 인증 메일 전송 후 승인 시 가입 완료.

    ![cpgn-user](https://github.com/user-attachments/assets/016dfa82-4710-4934-87c9-c99696d992c4)

### ✔ 상품/장바구니/결제
- **상품 관리**: 상품 등록, 수정, 삭제 및 상세 페이지 구현.
- **장바구니**: 상품 담기, 수량 변경, 선택/전체 결제 기능 제공.
- **결제**: **TossPayments API**를 연동해 카드·계좌이체 등 다양한 결제 수단 지원, 결제 성공/실패 시 주문 상태 자동 업데이트.

    ![cpgn-goods](https://github.com/user-attachments/assets/3fd34651-1568-443e-9b53-479ee76e3320)

### ✔ 리뷰 작성
- **구매자 한정**: 실제 구매한 사용자만 리뷰 작성 가능.
- **수정·삭제**: 작성한 리뷰는 수정 및 삭제 가능.
- **리뷰 표시**: 상품 상세 페이지에 리뷰와 평점 표시.

    ![cpgn-review](https://github.com/user-attachments/assets/81cd920e-8d8f-4872-8080-e3c46d5b9358)

### ✔ 공지사항 등록/수정/삭제
- **등록**: 관리자 권한으로 새로운 공지 작성.
- **수정**: 기존 공지 내용 업데이트.
- **삭제**: 불필요한 공지 제거.

    ![cpgn-notice](https://github.com/user-attachments/assets/57ff5695-a710-4f41-8131-ecb362e164f5)

### ✔ Q&A 등록/삭제
- **등록**: 사용자가 질문 작성.
- **삭제**: 불필요한 질문 또는 답변 삭제.

    ![cpgn-qna](https://github.com/user-attachments/assets/f3e84335-b3bd-493e-a530-a51c9fc93723)

### ✔ 관리자 Q&A 답변 등록/수정/삭제
- **등록**: 관리자가 사용자 질문에 대한 답변 작성.
- **수정**: 등록한 답변 내용 수정.
- **삭제**: 불필요하거나 잘못된 답변 삭제.

    ![cpgn-adminqna](https://github.com/user-attachments/assets/822847a5-00e6-4be5-97cc-a4de2118a9da)


### ✔ 자료실 등록/수정/삭제
- **등록**: 관리자 권한으로 새 자료 업로드.
- **수정**: 기존 자료 내용 및 파일 업데이트.
- **삭제**: 불필요한 자료 삭제.

    ![cpgn-dataroom](https://github.com/user-attachments/assets/c96fa528-e450-46cd-acdd-3c57c69acc98)


### ✔ 챗봇/1:1 채팅
- **챗봇(OpenAI 연동)**: AI 기반 자동 응답 및 상품 추천 기능 제공.

    <img width="380" height="953" alt="image" src="https://github.com/user-attachments/assets/625096df-1b56-4a97-b9be-ede34949d113" />
    <img width="380" height="953" alt="image" src="https://github.com/user-attachments/assets/318feb1e-e56d-4d2d-b113-ff6bce18fb39" />
- **1:1 채팅**: 고객이 관리자와 실시간 상담 가능, 대화 내역 관리 지원.

    <img width="380" height="953" alt="image" src="https://github.com/user-attachments/assets/c5969354-8b32-4fe8-b309-59dfd85810fc" />
    <img width="380" height="953" alt="image" src="https://github.com/user-attachments/assets/b320c881-ac87-4805-882c-d337169be6a6" />
- **관리자 1:1 채팅**: 관리자가 고객과 실시간 상담 가능, 대화 내역 관리 지원.

    ![cpgn-adminchat](https://github.com/user-attachments/assets/d5f51117-63cb-48bd-b926-de87aae71648)


### ✔ 리뷰 요약 mp3 생성 및 듣기
- **리뷰 요약 mp3 생성** : OpenAI TTS를 활용해 리뷰 내용을 요약하고 음성(mp3) 파일로 변환.
- **리뷰 요약 mp3 듣기** : 상품 상세 페이지에서 AI가 생성한 리뷰 요약 음성을 재생 가능.

    ![cpgn-tts](https://github.com/user-attachments/assets/84bf79ee-e9f1-443b-a654-1b49fd0f479b)


### ✔ 관리자 대시보드
- 회원 수, 상품 수, 주문 수, 미답변 Q&A 등 주요 데이터를 한눈에 확인할 수 있는 요약 패널 제공
- 최근 Q&A·주문 내역을 리스트로 표시하고 보기 버튼으로 상세 페이지 바로 이동 가능
- 공지/상품/자료실 등록 등 자주 사용하는 기능에 바로가기 버튼 지원
- 좌측 사이드바로 회원, 상품, 주문, 리뷰, Q&A, 채팅, 자료실, 배너 관리 기능을 직관적으로 탐색 가능

    ![cpgn-admin](https://github.com/user-attachments/assets/867743ce-be22-4d2f-8ae2-6bb2f3fc7f0a)



