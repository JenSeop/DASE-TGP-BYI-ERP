# DASE-TGP-BYI-ERP

# 1. 개요
<Strong>1-1 개발 배경</Strong><br>
현 재고 관리 시스템은 기업의 요구 조건에 따른 기업 맞춤형 프로세스이다.<br>
소상공인, 그 외 기업은 취급 물품에 따라 호환이 어려워 사용에 제약이 있다.<br>
또한, 독자적인 시스템을 구축하려해도 개발 및 유지보수 비용은 부담하기 어려운 현실이다.<br>
<br>
<Strong>1-2 개발 목적</Strong><br>
위의 문제를 해결하기 위해, 전 산업군을 아우르고 CX/UX관점을 반영한<br>
범용성을 갖춘 재고 관리 시스템을 개발하기로 목표하였다.<br>
BYI만의 ERP 시스템에는 각 ERP시스템의 장점을 녹여내었다.<br>
기업, 거래처 간의 입/출고, 판매와 같은 기본 기능을 포함하였으며,<br>
CX/UX 관점의 설계로 시스템은 사용자의 접근성이 높아진다.<br>
사용자 맞춤형 재고의 카테고라이징 기능 또한 사용이 가능하며,<br>
사용자 관점의 인터페이스와 프로세스, DB, 서비스를 제공한다.<br>

# 2. 팀원
|**팀장**|**팀원**|**팀원**|**팀원**|
| :------: | :------: | :------: | :------: |
|**김정섭**|**나인준**|**한상철**|**안희수**|
|**Front-End<br>(React, MUI)**|**Back-End<br>(Node.js, MySQL)**|**Back-End<br>(Node.js)**|**Design<br>(UI/UX)**|

# 3. 환경 <a href="https://react.dev/" onClick=""><img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=React&logoColor=white"/></a> <a href="https://mui.com/" onClick=""><img src="https://img.shields.io/badge/MUI-007FFF?style=flat-square&logo=MUI&logoColor=white"/></a> <a href="https://nodejs.org/en" onClick=""><img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=Node.js&logoColor=white"/></a> <a href="https://www.mysql.com/" onClick=""><img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=MySQL&logoColor=white"/></a><br>
<Strong>React</Strong><br>
메타에서 개발한 자바스크립트 기반의 오픈 소스 라이브러리이며,<br>
현재 자바스크립트 메인스트림 라이브러리이다.<br>
기본적으로 모듈형 개발이기 때문에 생산성이 상당히 높으며,<br>
SPA를 전제로 하고있어 동적인 현대의 웹에서 빠른 퍼포먼스를 보여주는 장점이 있다.<br>
<br>
<Strong>MUI</Strong><br>
MUI는 구글의 디자인 철학인 Material Design을<br>
구현한 자바스크립트 기반의 오픈 소스 라이브러리이다.<br>
Spotify, amazon, NETFLIX, unity, shutterstock등<br>
에서 사용하며 점차 메인스트림으로 자리잡고 있다. <br>
<br>
<Strong>Node.js</Strong><br>
오픈 소스 JavaScript 엔진인 크롬 V8에 비동기 이벤트처리<br>
라이브러리Iibuv를 결합한 플랫폼이다.<br>
빈번한 I/O처리에 있어서 우수한 성능, 서버 확장의 용이성,<br>
JavaScript 자체가 가지고 있는 장점과 더불어 이를 기반으로<br>
백엔드까지 작성이 가능하다.<br>
<br>
<Strong>MySQL</Strong><br>
1995년 발표된 오픈 소스 RDBMS로 현재까지도 컨텐츠 관리 시스템을<br>
지원하는 업제가 많을 정도로 점유율이 높다.<br>
이후 MySQL를 모태로 MariaDB라는 RDBMS가 만들어질 정도로 범용성이 높다.<br>

# 4. 구성
<strong>4-1 Diretory Tree</strong>
```bash
BYI_Front
├── front
│   └── src
│       ├── Layout
│       │   ├── L_MiddleNav.js
│       │   ├── L_TopNav_Off.js
│       │   ├── L_TopNav_On.js
│       │   ├── L_UserNav_Off.js
│       │   ├── L_UserNav_On.js
│       │   ├── Layout_Login.js
│       │   └── Layout_Logout.js
│       ├── Home
│       │   ├── Company
│       │   │   ├── HC_Total.js
│       │   │   ├── HM_Move.js
│       │   │   └── HM_Graph.js
│       │   ├── Sales
│       │   │   ├── HS_Sales.js
│       │   │   └── HS_Graph.js
│       │   └── H_Main.js
│       ├── Product
│       │   ├── CRUD
│       │   │   ├── P_Create.js
│       │   │   ├── P_Create_ImgUp.js
│       │   │   ├── P_test.js
│       │   │   ├── P_View.js
│       │   │   ├── P_ViewInf.js
│       │   │   └── ex.png
│       │   ├── P_CMain.js
│       │   ├── P_DB.js
│       │   ├── P_Main.js
│       │   ├── P_Menu.js
│       │   └── P_Search.js
│       ├── Sale
│       │   ├── A_CountAdd.js
│       │   ├── A_CountDelete.js
│       │   ├── A_CountRemove.js
│       │   ├── A_LogView.js
│       │   ├── A_Main.js
│       │   ├── A_Sales.js
│       │   ├── A_SalesConfirm.js
│       │   ├── A_SalesLog.js
│       │   ├── A_View.js
│       │   └── ex.png
│       ├── Set
│       │   ├── Attribute
│       │   │   ├── SA_DB.js
│       │   │   └── SA_Update.js
│       │   ├── Client
│       │   │   ├── SC_Create.js
│       │   │   ├── SC_DB.js
│       │   │   ├── SC_Delete.js
│       │   │   ├── SC_Menu.js
│       │   │   └── SC_Update.js
│       │   ├── Store
│       │   │   ├── SS_Main.js
│       │   └── S_Main.js
│       ├── User
│       │   ├── U_DB.js
│       │   ├── U_Delete.js
│       │   ├── U_FindID.js
│       │   ├── U_FindPW.js
│       │   ├── U_Login.js
│       │   ├── U_Register.js
│       │   ├── U_ResetPW.js
│       │   ├── U_Update.js
│       │   └── U_ViewID.js
│       ├── App.js
│       ├── index.css
│       ├── index.js
│       └── setupProxy.js
├── server
│   ├── db
│   │   ├── config.js
│   ├── middleware
│   │   ├── pool.js
│   │   ├── validate.js
│   ├── routes
│   │   ├── auth.js
│   │   ├── Client.js
│   │   ├── find.js
│   │   ├── findID.js
│   │   ├── Move.js
│   │   ├── mypage.js
│   │   ├── product.js
│   │   ├── Sales.js
│   ├── .env
│   ├── app.js
│   ├── package.json
└── └── package-lock.json
``` 
<strong>4-2 Database Tree</strong>
```
BYI-Back
├── Product
│   ├── ProductID INT
│   ├── ProductName VARCHAR
│   ├── ProductCode VARCHAR
│   ├── ProductBarcode VARCHAR
│   ├── ProductImport INT
│   ├── ProductExport INT
│   ├── ProductCount INT
│   ├── ProductDate DATETIME
│   ├── Attribute VARCHAR
│   ├── UserID INT
│   ├── UserPID INT
│   ├── UserType VARCHAR
│   ├── UserCode VARCHAR
│   └── UserInfo VARCHAR
├── Move
│   ├── MoveID INT
│   ├── MoveDate DATETIME
│   ├── InputStore VARCHAR
│   ├── OutputStore VARCHAR
│   ├── MoveInfo VARCHAR
│   ├── MoveCount INT
│   ├── InputDate DATETIME
│   ├── UserID INT
│   ├── UserMID INT
│   ├── MoveDIV VARCHAR
│   ├── UserType VARCHAR
│   ├── UserCode VARCHAR
│   └── Confirm INT
├── User
│   ├── UserID INT
│   ├── UserEmail VARCHAR
│   ├── UserPassword VARCHAR
│   ├── UserName VARCHAR
│   ├── UserAddress VARCHAR
│   ├── UserPhonenumber VARCHAR
│   ├── UserInfo VARCHAR
│   ├── UserType VARCHAR
│   └── UserCode VARCHAR
├── Sales
│   ├── SalesID INT
│   ├── SalesCount INT
│   ├── SalesPrice INT
│   ├── SalesDate DATETIME
│   ├── UserID INT
│   └── UserSID INT
├── Client
│   ├── ClientID INT
│   ├── ClientName VARCHAR
│   ├── ClientNum VARCHAR
│   ├── ClientAddress VARCHAR
│   ├── ManagerName VARCHAR
│   ├── ManagerNum VARCHAR
│   ├── ClientInfo VARCHAR
│   ├── UserID INT
│   └── UserCID INT
├── MoveSales
│   ├── MoveSalesID INT
│   ├── ProductID INT
│   ├── ProductName VARCHAR
│   ├── ProductCode VARCHAR
│   ├── ProductBarcode VARCHAR
│   ├── ProductImport VARCHAR
│   ├── ProductExport VARCHAR
│   ├── SalesCount INT
│   ├── UserID INT
│   ├── UserMSID INT
│   ├── SalesID INT
│   └── ProductCount INT
├── Output
│   ├── OutputID INT
│   ├── OutputDate DATETIME
│   ├── InputStore VARCHAR
│   ├── OutputStore VARCHAR
│   ├── OutputInfo VARCHAR
│   ├── OutputCount INT
│   ├── OutputDIV VARCHAR
│   ├── UserID INT
│   ├── TargetID INT
│   ├── UserOID INT
│   ├── UserType VARCHAR
│   ├── UserCode VARCHAR
│   ├── Confirm INT
│   └── InputDate DATETIME
├── MoveOutput
│   ├── MoveOutputID INT
│   ├── ProductID INT
│   ├── ProductName VARCHAR
│   ├── ProductCode VARCHAR
│   ├── ProductBarcode VARCHAR
│   ├── ProductImport INT
│   ├── ProductExport INT
│   ├── SalesCount INT
│   ├── ProductCount INT
│   ├── UserID INT
│   ├── UserMOID INT
│   ├── OutputID INT
│   ├── UserType VARCHAR
│   ├── UserCode VARCHAR
│   ├── Confirm INT
│   ├── InputStore INT
└── └── Attribute VARCHAR
```
# 5. 시연
![01 login](https://user-images.githubusercontent.com/95238604/235428272-0fe7b3df-e4b9-431f-aad1-b49865a68daa.png)
![02 register](https://user-images.githubusercontent.com/95238604/235428270-2e16a5b0-f8c1-4694-b470-2030fdc7cd9f.png)
![03 본사 메인](https://user-images.githubusercontent.com/95238604/235428056-d70d9c88-bb07-4804-a356-74e26da26dc5.png)
![04 매장 메인](https://user-images.githubusercontent.com/95238604/235428051-afef2561-ef8e-41cf-88d3-797b060f236e.png)
![04  매장 이동](https://user-images.githubusercontent.com/95238604/235428058-8ff34194-fe0d-452c-bc9f-74db8241d69d.png)
![07  본사 전체 재고](https://user-images.githubusercontent.com/95238604/235428070-2a5e742d-4273-48a2-9d51-22c4ea7ba1d8.png)
![06 정보 수정 및 삭제](https://user-images.githubusercontent.com/95238604/235428073-ed3ba5e3-4287-43b1-823d-40cadaaecba6.png)
![07  본사 재고 검색](https://user-images.githubusercontent.com/95238604/235428076-c2969b87-1df2-4b45-aa64-044db3cbf18d.png)
![08  매장 재고](https://user-images.githubusercontent.com/95238604/235428083-a580148e-b026-43cd-919f-6c76533cea04.png)
![08  매장 재고 검색](https://user-images.githubusercontent.com/95238604/235428084-0b0c54df-17af-4e4c-81da-00f1353912b9.png)
![10  본사 출고 등록](https://user-images.githubusercontent.com/95238604/235428091-e93feea7-c5c7-4d41-a581-e6fc05f4dd23.png)
![13 본사 입출고 내역](https://user-images.githubusercontent.com/95238604/235428101-911db36c-fb3a-4370-b800-a154cf951842.png)
![09  본사 입고](https://user-images.githubusercontent.com/95238604/235428093-fdf3ef17-6f98-452b-a42d-21ef4b02df5b.png)

# 6. 참고
https://www.fun-coding.org/mysql_basic1.html<br>
#. RDBMS(Relational Database Management System)의 이해<br>
https://devhints.io/mysql<br>
#. MySQL cheatsheet<br>
https://mui.com/<br>
#. Mui<br>
https://ko.reactjs.org/<br>
#. React<br>
https://nodejs.org/ko/<br>
#. Node.js<br>
https://www.forwarder.kr/bbs/board.php?bo_table=menu9_1&wr_id=2042<br>
#. 재고의 정의와 필요성<br>
#. 재고의 종류<br>
#. 재고관리의 목적<br>
#. 재고관리의 비용<br>
#. 재고관리 관련 지표<br>
#. 재고관리 시스템 (재고 관리 기법)<br>
#. 수요예측기법<br>
https://dynamics.microsoft.com/ko-kr/field-service/inventory-management-system/<br>
#. 재고관리 시스템의 문제 및 이점<br>
https://www.ibm.com/kr-ko/topics/inventory-management<br>
#. 재고관리 정의 및 필요성<br>
#. 재고 가시성<br>
#. 재고관리 시스템<br>
http://www.beautytimes.com/<br>
#. 효과적인 재고관리 방법<br>
http://uonit.co.kr/page1000/<br>
#. 통합고정자산관리 (EAM - Enterprise Asset Management)<br>
