![image](https://github.com/user-attachments/assets/97875e38-2ba5-4e33-af05-7897c51b420e)

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
  
+ 아이디(TextField)와 비밀번호(PasswordField)의 fx:id를 lookup 해서 그 필드에 해당하는 값을 가지고 데이터 베이스에 저장되어 있는 [회원 정보 테이블]에 접근하여, 조회되는 아이디와 비밀번호가 존재한다면 true, 존재 하지 않는다면 false 값을 출력해준다.

+ 버튼을 눌렀을 때, 로그인이 되어 있지 않으면 ‘로그인 오류’ 라는 MSG박스를 나타내고, 로그인 페이지로 넘어간다.
  
+ 로그인을 하지 않은 상태에서는 로그인, 회원가입 버튼을 제외한 모든 버튼 기능 사용 불가
  
![스크린샷 2025-04-28 160653](https://github.com/user-attachments/assets/751da45e-03bc-464f-826c-91b67607f0db)

</details>

<hr style="border: 3px solid #000;">

<details>
<summary>✅ 회원 가입 (Sign up)</summary>

+ 정보 입력

회원가입 할 이름, 아이디, 비밀번호, 전화번호, 성별, 이메일, 주소를 입력한다.

+ [중복 확인] 버튼

아이디는 유일한 값으로 잡아준다.
중복 확인 버튼을 눌렀을 때, 기존에 아이디가 존재하면 중복이 된다는 설명을 MSG박스로 알려준다.
아이디 Text field 부분의 내용을 지우고  requestfocus로 맞춰준다.

+ 비밀번호

아이디는 유일한 값으로 잡아준다.
중복 확인 버튼을 눌렀을 때, 기존에 아이디가 존재하면 중복이 된다는 설명을 MSG박스로 알려준다.
아이디 Text field 부분의 내용을 지우고  requestfocus로 맞춰준다.

+ [이메일 선택] 버튼

comboBox를 이용하여 이메일을 직접 입력 또는 선택할 수 있도록 한다.

+ [Success] 버튼

Success 버튼을 눌렀을 때, 회원 가입이 성공하였다는 MSG박스로 나타내고 로그인 페이지로 넘어가게 된다. 

+ [Cancel] 버튼

Cancel 버튼을 눌렀을 때, 다시 메인 페이지로 넘어가게 된다. 

![image](https://github.com/user-attachments/assets/7663bd71-8f70-4106-86fb-8b0d1b056508)

</details>

<hr style="border: 3px solid #000;">
<details>
<summary>✅정보 수정 (My Page)</summary>
  
![스크린샷 2025-04-28 162501](https://github.com/user-attachments/assets/612e92c3-b222-4b02-84c3-e14bbde206e2)
1. 사용자 정보
  
사용자의 정보를 보여주는 페이지, 이름, 아이디, 주소, 전화번호를 순서대로 보여준다. 

2. [My Ticket] 버튼

사용자의 정보를 보여주는 페이지, 이름, 아이디, 주소, 전화번호를 순서대로 보여준다. 

4. [Mileage] 버튼

History 버튼을 눌렀을 때, History 페이지로 넘어간다. 여기서 말하는 History는 이때까지 구매했던 기차표를 조회할 수 있다.

5. [Logout] 버튼

Logout 버튼을 눌렀을 때, MSG박스로 로그아웃이 되었다는 사실을 알려주고 로그아웃이 된다. 로그아웃이 된 후에는 자동으로 로그아웃이 된 메인 페이지로 넘어가게 된다.  

7. [회원 탈퇴] 버튼

MSG박스로 회원탈퇴가 완료되었다고 알려준 후, 로그인이 되어있지 않은 상태의 메인 페이지로 넘어간다.
회원 탈퇴한 정보의 아이디로 로그인을 시도할 시, 로그인이 불가하다.

</details>
<hr style="border: 3px solid #000;">
<details>
<summary>✅ 열차 조회 (Train search)</summary>
  
![스크린샷 2025-04-28 162859](https://github.com/user-attachments/assets/5b0f469e-d6c2-4c4a-9d34-5a89f74be2b3)

1. [조건 선택] 버튼
  
해당하는 조건의 선택 버튼을 눌렀을 때, ComboBox로 열차의 종류를 보여주고 선택할 수 있다. 

2. 검색 버튼

해당하는 열차의 이름과 출발지를 조건으로 그에 해당하는 열차이름, 출발지, 도착지, 출발시간, 도착 시간, 소요시간, 좌석, 요금을   보여준다.

3.선택

해당하는 열차의 이름과 출발지를 조건으로 그에 해당하는 열차이름, 출발지, 도착지, 출발시간, 도착 시간, 소요시간, 좌석, 요금을   보여준다.

4.[Seat] 버튼

seat 버튼을 눌렀을 때, 해당하는 열차의 좌석을 고를 수 있는 ChoiceSeat 페이지로 넘어간다.

</details>

<hr style="border: 3px solid #000;">

<details>
<summary>✅ 좌석 석택 (Choice Seat)</summary>

1. 열차 이름

seat 버튼을 눌렀을 때, 해당하는 열차의 좌석을 고를 수 있는 ChoiceSeat 페이지로 넘어간다.

2. 좌석

![스크린샷 2025-04-28 163857](https://github.com/user-attachments/assets/aa9c4c6b-815e-4b9b-b257-668f67deef62)

Check Box로 선택할 수 있는 좌석을 중복이 되지 않게 골라 원하는 좌석을 선택한다.

3. [Pay] 버튼

Pay 버튼을 눌렀을 때, Pay 페이지로 넘어간다.

</details>

<hr style="border: 3px solid #000;">

<details>
<summary>✅ 구매 내역 (Payment)</summary>
  
![스크린샷 2025-04-28 163445](https://github.com/user-attachments/assets/915d2613-2dba-4b04-a506-ab6d9601fce4)

1. 구매내역
지금까지 구매 했던 기차표의 정보를 가져온다.
구매 날짜, 출발지, 도착지, 금액, 좌석 번호를 보여준다.

2. [조회] 버튼

조회 버튼을 누르면, 전체 구매 날짜와 출발지, 도착지, 금액, 좌석번호를   보여준다.

3. [Train Search] 버튼 

조회 버튼을 누르면, 전체 구매 날짜와 출발지, 도착지, 금액, 좌석번호를   보여준다.

</details>
<hr style="border: 3px solid #000;">

<details>
<summary>✅ 내 티켓 (My Ticket)</summary>
  
  ![image](https://github.com/user-attachments/assets/44539455-7883-4018-b941-c5ed1fc0b485)

+  내 티켓
미사용 티켓 정보를 보여준다.
소요 시간, 열차 명, 탑승자 명, 좌석 번호, 출발지, 도착지, 출발시간, 도착시간을 순서대로 보여준다.

</details>
<hr style="border: 3px solid #000;">

## 🔍 참고 사이트 
- 코레일 : https://www.royalcanin.com/kr](https://www.korail.com/)

<hr style="border: 3px solid #000;">

## ⚙ 사용 기술

| 구분 | 내용 | 설명 |
|:---|:---|:---|
| **Backend** | ![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white) ![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)  | Java 17, MyBatis |
| **Frontend** | ![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white) ![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E) | JSP, HTML5, CSS3, JavaScript |
| **Database** | ![Oracle](https://img.shields.io/badge/Oracle-F80000?style=for-the-badge&logo=oracle&logoColor=white) | Oracle (ojdbc8),Oracle SQL Developer(23.1.347) |
| **Version Control** | ![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white) ![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white) | Git, GitHub |


## 🛠️ 개발 도구

| 구분 | 도구 | 설명 |
|:----:|:----:|:----|
| IDE | ![STS3](https://img.shields.io/badge/STS3-F7DF1E?style=for-the-badge&logo=Spring&logoColor=black) | Spring Tool Suite 3 |
| Database Tool | ![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=MySQL&logoColor=black) | Oracle,Oracle SQL Developer(23.1.347） |
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


