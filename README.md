

# TRAIN Project
KG아이티뱅크에서 주간하는 프로젝트로, Eclipse 를 사용해서 GUI(Graphical User Interface)로 구현한 '기차예매'프로그램입니다. GUI로 만들기 위해서 JavaFx를 사용해서 버튼, 텍스트박스, 테이블, 이미지 뷰어, 창(윈도우) 기반 프로그램을 구축해봤습니다.



## 🗂️ 프로젝트 소개 🗂️

- 기차를 예매하기 전 로그인 또는 회원가입을 한다.
- 기차 종류(KTX, 새 마을, 무궁화) 중 원하는 기차를 선택한다.
- 기차를 선택 후 해당하는 열차를 조건으로 그에 해당하는  출발과 도착지, 출발 시간, 도착 시간, 소요 시간, 요금을  보고 선택한다.
- 원하는 좌석을 선택 후 결제한다.

## 👩‍💻 개발자 소개 👨‍💻

### 👑 팀장
- 💎 **양평근**
  
  -[GitHub](https://github.com/ypk0680)

### 🛠️ 팀원
- 🧩 **김수경**
  - [GitHub](https://github.com/Kim-suk)

## 🔎 주요 기능

<details>
<summary>✅ 로그인 (Login)</summary>
  
1. [Sign Up] 버튼
  
2.[Cancel] 버튼

3.[Login] 버튼


+  로그인을 하는 과정
  
+ 아이디(TextField)와 비밀번호(PasswordField)의 fx:id를 lookup 해서 그 필드에 해당하는 값을 가지고 데이터 베이스에 저장되어 있는 [회원 정보 테이블]에 접근하여, 조회되는 아이디와 비밀번호가 존재한다면 true, 존재 하지 않는다면 false 값을 출력해준다.
![image](https://github.com/user-attachments/assets/0e05ece0-f338-4769-9720-01d135d51195)

+ 버튼을 눌렀을 때, 로그인이 되어 있지 않으면 ‘로그인 오류’ 라는 MSG박스를 나타내고, 로그인 페이지로 넘어간다.
  
+  로그인 전 메인 페이지
  
+ 로그인을 하지 않은 상태에서는 로그인, 회원가입 버튼을 제외한 모든 버튼 기능 사용 불가
  
![스크린샷 2025-04-28 160653](https://github.com/user-attachments/assets/751da45e-03bc-464f-826c-91b67607f0db)

</details>

<hr style="border: 3px solid #000;">

<details>
<summary>✅ 내 정보 (My page)</summary>

+ 회원 정보 수정  
: 이름, 나이, 이메일

![image](https://github.com/user-attachments/assets/b1624cdb-8f3e-4478-a085-122e2dd10217)

+ 비밀번호 변경  
: 기존 비밀번호 입력 후 새 비밀번호 입력

![image](https://github.com/user-attachments/assets/df7844ea-8f56-4da5-8ff7-79e4ae28abe5)

+ 회원 탈퇴  
: 현재 비밀번호 입력 후 회원탈퇴 가능

![image](https://github.com/user-attachments/assets/9e2ce22f-4f0b-4eca-802b-130a2b1511b3)

</details>

<hr style="border: 3px solid #000;">

<details>
<summary>✅ 열차 조회 (Train search)</summary>

+ 현재 위치 기반으로 반경 1km에 있는 동물병원 위치 확인 가능

![image](https://github.com/user-attachments/assets/81039edf-e25c-475c-9c22-65d1443570b1)

+ 마킹 되어있는 동물병원 클릭 시 상세 정보 확인 가능

![image](https://github.com/user-attachments/assets/042a80ef-4af7-45ee-bd05-93d09adf6595)

</details>

<hr style="border: 3px solid #000;">

<details>
<summary>✅ 구매 내역 (Board)</summary>

+ 게시글 등록

![write](https://github.com/user-attachments/assets/da062942-b746-4dda-ad53-fa3c0940e229)

+ 게시글 수정

![modify](https://github.com/user-attachments/assets/359bd10b-320c-425b-a63c-209b29028c2d)

+ 게시글 삭제

![delete](https://github.com/user-attachments/assets/e361e00e-e510-43bb-8890-687b01cd74ba)

+ 게시글 좋아요, 댓글, 조회수

![like](https://github.com/user-attachments/assets/7050481d-cfd3-40a0-9254-2442c89791ed)

</details>

<hr style="border: 3px solid #000;">

<details>
<summary>✅ 결제 (Payment)</summary>

+ 카테고리별 상세 검색 가능

![image](https://github.com/user-attachments/assets/d99b60d0-d184-4824-bf72-aa76c896c922)

+ 장바구니

![장바구니](https://github.com/user-attachments/assets/b1fd8e91-61b1-4d59-b98e-c12b4032da22)

+ 결제

![결제 성공](https://github.com/user-attachments/assets/7a0f5066-5d21-47c6-8a16-f39774a4fbfc)

</details>
<hr style="border: 3px solid #000;">

## 🔍 참고 사이트 
- 코레일 : https://www.royalcanin.com/kr](https://www.korail.com/)

<hr style="border: 3px solid #000;">

## ⚙ 사용 기술

| 구분 | 내용 | 설명 |
|:---|:---|:---|
| **Backend** | ![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white) ![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)  | Java 11, Spring 3.1.1, MyBatis |
| **Frontend** | ![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white) ![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E) | JSP, HTML5, CSS3, JavaScript |
| **Database** | ![Oracle](https://img.shields.io/badge/Oracle-F80000?style=for-the-badge&logo=oracle&logoColor=white) | Oracle (ojdbc8) |
| **Version Control** | ![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white) ![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white) | Git, GitHub |


## 🛠️ 개발 도구

| 구분 | 도구 | 설명 |
|:----:|:----:|:----|
| IDE | ![STS3](https://img.shields.io/badge/STS3-F7DF1E?style=for-the-badge&logo=Spring&logoColor=black) | Spring Tool Suite 3 |
| Database Tool | ![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=MySQL&logoColor=black) | Oracle, MySQL 등 사용 가능 |
| Server | ![Apache Tomcat](https://img.shields.io/badge/Apache_Tomcat-F8DC75?style=for-the-badge&logo=ApacheTomcat&logoColor=black) | Tomcat 서버 |
| Build Tool | ![Maven](https://img.shields.io/badge/Apache_Maven-C71A36?style=for-the-badge&logo=ApacheMaven&logoColor=white) | Maven 프로젝트 빌드 관리 |

<hr style="border: 3px solid #000;">

## 📅 프로젝트 기간
2025년 2월 3일 → 2025년 2월 13일

<hr style="border: 3px solid #000;">

## 🧭스토리 보드

![image](https://github.com/user-attachments/assets/9efe8fef-65d6-42e9-9f43-8d19b5d18e6d)

<hr style="border: 3px solid #000;">

## 🗃 PRESENTATION
### 📎[trainproject](https://docs.google.com/presentation/d/1hI2vCLWFTWVr8YAIpfm7Xa4CDafsCqKX/edit?usp=sharing&ouid=115265115342844139543&rtpof=true&sd=true)


## 🧶ERD ( DB 설계)


