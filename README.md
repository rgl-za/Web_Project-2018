# Web_Project-2018: 새벽서점 📚

## 프로젝트 설명 
온라인 서점 사이트

- 개발 환경: EditPlus
- 개발 언어: HTML, CSS, PHP
- 데이터베이스: MySQL

팀원 및 역할 분담
- 프론트엔드: 윤영미, 이미진
- 백엔드: 이미진, 지현정

## 프로젝트 구조
#### 사용자 페이지
- 메인 페이지
  - 로그인, 회원가입 
  - 국내 도서
  - 외국 도서
  - 신간 도서
  - 수험 정보
- 도서 상세 페이지 
- 장바구니
- 도서 주문 페이지
- 마이페이지
  - 주문내역
  - 회원정보 수정 
- 공지사항
  - 공지사항
  - 자주 묻는 질문
  - 문의하기  

#### 관리자 페이지
- 현황 분석 
- 게시판 관리
  -  공지사항
  -  자주 묻는 질문
  -  문의 사항
- 도서 관리
  - 도서 목록, 정보 수정
  - 도서 등록 
- 주문 관리
- 회원 관리

#### 데이터베이스 설계 
![그림1](https://user-images.githubusercontent.com/76260153/150551228-88f47958-bdec-4c63-a5bb-4be147f04201.png)
![그림2](https://user-images.githubusercontent.com/76260153/150551493-50fd395d-61d5-4739-9483-1fe26ad8a261.png)
![그림3](https://user-images.githubusercontent.com/76260153/150551525-d6cdedbe-cc8b-43a5-922b-c400507fdd93.png)
![그림4](https://user-images.githubusercontent.com/76260153/150551579-1f2c8518-7cfc-461a-9be9-fdff35e625b6.png)
![그림5](https://user-images.githubusercontent.com/76260153/150551646-d1fec953-8825-4290-925f-c62acc664d4f.png)
![그림6](https://user-images.githubusercontent.com/76260153/150551711-b580b2c1-5aae-439e-9956-721b3420690b.png)
<img width="681" alt="그림7" src="https://user-images.githubusercontent.com/76260153/150551795-04d9a920-d4b2-4184-8b68-509ca1bebe22.png">

    
## 프로젝트 기능 (회원)
### 1. 메인 화면
![그림8](https://user-images.githubusercontent.com/76260153/150554119-cd44a5be-c34a-4c7f-ac75-cc31a4e9045d.png)
- 도서 통합 검색 기능
- 화제의 권장도서, 베스트 셀러, 이 주의 책으로 구분
#### 1.1 회원가입
![그림9](https://user-images.githubusercontent.com/76260153/150554205-b0690a24-fcc7-45b8-893d-b814b8bf33b4.png)
#### 1.2 로그인
![그림10](https://user-images.githubusercontent.com/76260153/150554369-9271f2b6-6ce2-4eed-9d17-418443c70d6b.png)
- 회원가입 후 로그인을 하면 메인화면으로 이동
- 로그인한 상태에서는 상단에 로그인 버튼이 로그아웃으로 변경

#### 1.3 국내 도서
![그림11](https://user-images.githubusercontent.com/76260153/150555558-1f579e7e-cca5-47ac-ba5f-34858f9bfbf7.png)

#### 1.4 외국 도서
![그림12](https://user-images.githubusercontent.com/76260153/150555705-69ac381f-1fb4-4fe6-b76d-743427982726.png)

#### 1.5 신간 도서
![그림13](https://user-images.githubusercontent.com/76260153/150555766-cdf4cc92-2225-4d1a-a752-40bb0f6f9124.png)

#### 1.6 수험정보
![그림14](https://user-images.githubusercontent.com/76260153/150555852-5d6edeb2-f200-4443-9319-92d8dcf4c6d5.png)

- 최근 발행일 순으로 정렬
- 도서별 카테고리는 분야마다 도서 고유번호를 부여하여 분류
- 신간도서, 발행일자, 가격 순으로 책을 분류하여 정렬할 수 있도록 구현

### 2. 도서 상세 페이지
![그림17](https://user-images.githubusercontent.com/76260153/150557459-3727cc18-1d78-4df3-9e19-33778def6b06.png)
- 기본적인 책 정보(제목, 부제목, 출판사, 발행일, 판매가, 포인트, 배송비, 예상 배송 일정, ISBN, 쪽수, 크기) 기재
- 책 소개, 저자 소개, 목차, 출판사 서평, 회원 리뷰, 교환/반품/품절 안내

![그림18](https://user-images.githubusercontent.com/76260153/150557920-ee16beb0-2520-456f-8617-1978ccdc5a32.png)
![그림19](https://user-images.githubusercontent.com/76260153/150557966-e51993ad-05f4-4c1d-b652-c06ca4e1cb90.png)
- 회원 리뷰에서 별점 1~5개를 남길 수 있음 

### 3. 장바구니
![그림15](https://user-images.githubusercontent.com/76260153/150556407-d2e2e699-01e1-48d8-a2a1-db9df65e1339.png)
![그림16](https://user-images.githubusercontent.com/76260153/150556476-68526dd9-a5bf-4976-955c-1c022735cb4a.png)
- 도서 목록 페이지에서 장바구니 담기나 바로 구매하기를 누르면 각각 해당하는 페이지로 이동

![그림20](https://user-images.githubusercontent.com/76260153/150558190-597e169a-bf5d-411f-9e68-62689380e426.png)
- 도서 정보, 수량, 상품 금액, 포인트, 합계 금액, 예상 배송 일정 출력
- 수량을 장바구니에서 조절할 수 있도록 구현
- 도서 수량이 0이라면 해당 도서 항목이 장바구니에서 삭제
- 체크박스를 통해 선택된 도서만 주문하거나 삭제할 수 있음
- 장바구니에 담긴 도서 개수와 배송비가 포함된 총 주문가격이 출력

### 4. 도서 주문 페이지
![그림21](https://user-images.githubusercontent.com/76260153/150558679-84ad87f3-24db-41a9-901b-3fff2bdcf3c7.png)
- 주문 신청한 도서 목록과 주문한 총 도서 개수, 가격이 출력
- 구매자 정보와 배송지 정보를 입력하도록 함
- 로그인한 회면은 회원 정보의 주소를 자동으로 넘겨오도록 구현

### 5. 마이페이지
#### 5.1 주문내역
![그림22](https://user-images.githubusercontent.com/76260153/150559174-ef30256b-7f42-4c83-9f62-cb746c764b25.png)
- 주문한 내역들을 한 눈에 확인할 수 있음

<img width="792" alt="그림23" src="https://user-images.githubusercontent.com/76260153/150559373-fb52ab0f-37a2-46b9-b55c-bfd5dbb2d589.png">

- 도서를 주문한 후의 장바구니는 비어있음

#### 5.2 회원정보 수정
![그림24](https://user-images.githubusercontent.com/76260153/150559574-1c62d9ce-5531-4640-a190-a1dcf84d0d83.png)

### 6. 공지사항
#### 6.1 공지사항
<img width="792" alt="그림25" src="https://user-images.githubusercontent.com/76260153/150560675-1b0c2a8d-e4fe-4b9d-94db-242612282a8a.png">

- 홈페이지 전체 공지사항을 확인할 수 있음

#### 6.2 문의하기
<img width="792" alt="그림26" src="https://user-images.githubusercontent.com/76260153/150560713-4f4514f6-17ab-4ee3-9b36-295680b158b6.png">

![그림27](https://user-images.githubusercontent.com/76260153/150560769-eb3aabcd-0cd8-43d6-a839-796e807da736.png)

- 회원이 개인별로 문의할 수 있음
- 게시글에 비밀번호 구현, 해당 회원만 게시글과 답변을 확인 할 수 있음

#### 6.3 자주 묻는 질문
![그림39](https://user-images.githubusercontent.com/76260153/150568981-e92b13a2-f95a-412d-af7e-9d93b5d83392.png)

- 자주 묻는 질문들을 확인할 수 있음

## 프로젝트 기능 (관리자)
관리자 계정으로 로그인을 하면 관리자 페이지로 이동함
### 1. 현황 분석
<img width="792" alt="그림28" src="https://user-images.githubusercontent.com/76260153/150561829-499dcd35-c908-4c12-a757-59e117a85667.png">

- 오늘의 주문 리스트
  - 오눌 주문한 주문 정보들을 볼 수 있음
- 신규 회원가입 리스트
  - 신규 회원의 정보들을 볼 수 있음
- 상단의 사이트로 이동을 누르면 사용자 페이지로 이동 가능


### 2. 게시판 관리
회원 페이지의 공지사항 페이지와 연동
#### 2.1 공지사항
<img width="793" alt="그림29" src="https://user-images.githubusercontent.com/76260153/150563522-db57a42b-6d9f-4f1d-b5c4-ea88c3f436da.png">

- 공지할 게시글들을 올릴 수 있음

#### 2.2 문의 사항
<img width="793" alt="그림31" src="https://user-images.githubusercontent.com/76260153/150563788-416a2ed4-658c-4ea2-9060-de9d4c8861f8.png">
<img width="792" alt="그림32" src="https://user-images.githubusercontent.com/76260153/150563840-1b15573e-297e-4807-a018-780825617873.png">

- 고객이 문의한 글에 대한 답변 및 수정, 삭제할 수 있음 

#### 2.3 자주 묻는 질문
<img width="793" alt="그림30" src="https://user-images.githubusercontent.com/76260153/150563628-8ff354ee-f9cd-4220-ab73-6612909723fb.png">

- 자주 묻는 질문들을 모아서 게시글로 등록할 수 있음


### 3. 주문 관리
![그림33](https://user-images.githubusercontent.com/76260153/150563984-7e938c62-d56a-4eef-8b0d-86a6aca01120.png)
- 고객이 주문한 주문정보를 받아올 수 있도록 구현


### 4. 도서 관
#### 4.1 도서 목록, 정보 수정
<img width="792" alt="그림34" src="https://user-images.githubusercontent.com/76260153/150564085-accc556f-055d-4776-9aac-c348e96d04bb.png">

- 등록된 도서들의 목록을 볼 수 있음
- 카테고리 분류를 하면 해당 카테고리의 도서들만 확인할 수 있음


![그림35](https://user-images.githubusercontent.com/76260153/150564403-1141048b-5a66-472b-9ab7-e8e11fc52f40.png)
- 도서 목록의 수정을 누르면 해당 도서의 정보를 수정할 수 있도록 구현
<img width="793" alt="그림36" src="https://user-images.githubusercontent.com/76260153/150564498-f2ce2114-c8ad-401d-abeb-8568da270e6c.png">

#### 4.2 도서 등록 
![그림37](https://user-images.githubusercontent.com/76260153/150564973-d4765ade-ddca-44ff-83c3-1c5d0ef68e16.png)
- 도서 등록시 도서 관리 페이지에서 해당 도서를 확인할 수 있음


### 5. 회원 관리
<img width="793" alt="그림38" src="https://user-images.githubusercontent.com/76260153/150565051-7d479fe9-a2c8-4295-bb5a-984db185abe6.png">

- 가입한 회원들의 정보를 확인 할 수 있음
- 회원의 기본 정보인 아이디, 이름, 가입 날짜, 접속한 수를 확인 할 수 있음
