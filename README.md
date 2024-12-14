# PAS Project - Artion
클라우드 웹앱 개발자 양성 과정에서 진행된 두번째 프로젝트입니다. 
</br>SpingBoot 와 React 를 활용하여 Restful 형식의 그림경매 사이트를 구현하였습니다.
## 👨‍🏫 프로젝트 소개
- 온라인으로 모든것이 가능한 시대, 집에서 그림을 경매하기 위한 사이트입니다.
- 그림을 구매하기전 AR 기능을 통해 미리 장식해볼 수 있습니다.
- 온라인 구매의 단점을 보완하고 다양한 미술작품을 쉽게 구매할 수 있습니다.
## 🧑‍🤝‍🧑 멤버구성
- Backend 3명, Frontend 4명
## ⏲️ 개발기간
- 2024.10.01(화) ~ 2024.10.28(월)
## ⚙️ 개발 환경
- **Language** : <img src="https://img.shields.io/badge/java-007396?style=for-the-badge&logo=java&logoColor=white"> <img src="https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">
- **Framework** : <img src="https://img.shields.io/badge/springboot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white"> <img src="https://img.shields.io/badge/react-61DAFB?style=for-the-badge&logo=react&logoColor=black"> 
- **Server** : <img src="https://img.shields.io/badge/firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=white"> <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=AWS&logoColor=white">
- **DataBase** :  <img src="https://img.shields.io/badge/mariaDB-003545?style=for-the-badge&logo=mariaDB&logoColor=white">
- **ETC** : <img src="https://img.shields.io/badge/git-F05032?style=for-the-badge&logo=git&logoColor=white">
## 📝 시스템 아키텍쳐
+ 프로그램 아키텍쳐
![image](https://github.com/user-attachments/assets/e437ce76-f925-4c18-b7e5-c9cef2810b02)

## 📌 주요기능
1. **로그인 및 회원정보 등록**
   + 카카오 로그인(연동 동작 처리)
   + 로그인 진행 후 개인정보 등록 진행
   + 회원정보 등록시 필요사항
      + 프로필 이미지 : 카카오톡 프로필 사진 연동 가능
      + 닉네임 : 카카오톡 프로필 닉네임 연동 가능
      + 계좌정보 : 그림 구매 및 판매 시 이용 계좌 정보 등록
      + 주소 : 그림 낙찰 시 그림을 배송받을 주소지 검색 및 등록
2. **메인피드**
   + 로그인 후 접속하게 되는 페이지
   + 메인페이지에서 인기작 및 최신작 감상 가능
   + 작품 아래 작품명, 작가명, 좋아요 갯수 확인 가능
   + 작품 클릭시 작품 상세페이지 이동
3. **작품등록**
   + 작품명 : 작품 이름 등록
   + 작가명 : 작가 이름 등록
   + 작품설명 : 작품에 대한 설명 등록
   + 작품제작년도 : 작품이 제작된 년도 등록 (현재 날짜 이전의 시간만 선택 가능하게 설정)
   + 작품크기 : 넓이, 높이, 두께 사이즈 등록
   + 그림 카테고리 : 그림의 종류 등록 (복수 선택 가능)
   + 작품 경매기간 : 최소 3시간, 최대 일주일 기간으로 설정 가능, 경매기간 넘어갈 시 alert 에러
   + 최소 판매가 : 그림의 경매 시작가 등록
   + 즉시 판매가 : 경매와 상관없이 바로 구매 가능한 금액 등록
   + 작품사진 : 첫번째 등록 사진은 대표이미지로 설정, 이미지 선택시 삭제
4. **검색기능**
   + 좌측 메뉴 버튼을 통해 카테고리 검색
   + 원하는 카테고리 및 가격 필터링 가능
   + 정렬방식 선택 : 좋아요 많은순, 높은 가격순, 낮은 가격순, 최신순
   + 검색결과 무한스크롤 제공
5. **좋아요/팔로잉/팔로워**
   + 좋아요 : 개인페이지에서 좋아요 누른 작품 리스트 확인 가능
   + 팔로잉 : 팔로잉 리스트 추가, 팔로잉 취소, 팔로잉 작가 페이지 이동
   + 팔로워 : 팔로워 리스트 추가, 팔로워 작가 페이지 이동
6. **AR 전시**
   + 공간인식 AR 카메라 연동
   + 선택한 작품의 이미지와 크기 적용
   + 원하는 장소에 작품 설치 가능
7. **구매내역**
   + 전체 : 입찰 중, 낙찰완료(결제대기), 경매종료
   + 입찰 : 내 입찰 내역
   + 낙찰 : 낙찰 완료 (결제대기)
   + 종료 : 낙찰 여부 상관없이 경매 종료 내역
8. **판매내역**
   + 전체 : 경매 시작 전, 입찰 중, 낙찰완료(입금대기), 경매종료
   + 입찰 : 내 작품 입찰 내역
   + 낙찰 : 내 작품 낙찰 완료(입금대기)
   + 종료 : 내 작품 경매 종료 내역
9. **경매페이지**
   + 남은시간표시
   + 지정된 최대가와 현재가 사이 금액 입찰
   + 웹소켓을 통한 실시간 경매 진행
   + 즉시 판매가 입력시 즉시 낙찰
10. **결제페이지**
    + 주소, 연락처, 구매자 이름, 배송방식 설정
