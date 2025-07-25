# Spring Boot-React 프로젝트 - 꼼파뇨 스튜디오

## 목차

- [개요]()
- [기술 스택]()
- [프로젝트 설계]()
- [주요 기능]()
- [기능 구현]()

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

## **✨ 주요 기능**

### 1️⃣ Google 로그인

- **Google OAuth 2.0**
    - Google OAuth 2.0 연동을 통해 Google 계정으로 손쉽게 로그인할 수 있습니다.

<img width="400" height="950" alt="image" src="https://github.com/user-attachments/assets/c80dfa2e-c62c-452d-832e-a043559a8c4f" />
<img width="400" height="950" alt="image 1" src="https://github.com/user-attachments/assets/c26d67fa-b492-4d60-b228-b49b69be9c16" />


### 2️⃣ Toss Pay 결제

- **TossPayments API**
    - TossPayments API를 통해 카드, 계좌이체, 간편결제 등 다양한 결제 수단으로 쉽고 안전하게 결제할 수 있습니다.

<img width="400" height="950" alt="image 2" src="https://github.com/user-attachments/assets/26fcc8f8-2873-4c57-960c-dd51fc8f501a" />
<img width="400" height="955" alt="image 3" src="https://github.com/user-attachments/assets/70c14e9e-afe7-4a18-a2df-9735fc38523b" />


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

### ✔ 자료실 등록/수정/삭제
- **등록**: 관리자 권한으로 새 자료 업로드.
- **수정**: 기존 자료 내용 및 파일 업데이트.
- **삭제**: 불필요한 자료 삭제.

### ✔ 챗봇/1:1 채팅
- **챗봇(OpenAI 연동)**: AI 기반 자동 응답 및 상품 추천 기능 제공.
- **1:1 채팅**: 고객이 관리자와 실시간 상담 가능, 대화 내역 관리 지원.
<img width="400" height="953" alt="image" src="https://github.com/user-attachments/assets/625096df-1b56-4a97-b9be-ede34949d113" />
<img width="400" height="953" alt="image" src="https://github.com/user-attachments/assets/318feb1e-e56d-4d2d-b113-ff6bce18fb39" />
<img width="400" height="953" alt="image" src="https://github.com/user-attachments/assets/c5969354-8b32-4fe8-b309-59dfd85810fc" />
<img width="400" height="953" alt="image" src="https://github.com/user-attachments/assets/b320c881-ac87-4805-882c-d337169be6a6" />

  


