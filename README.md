# DASE-TGP-BYI-ERP

# 1. 프로젝트 개요
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
# 2. 개발환경 <a href="https://react.dev/" onClick=""><img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=React&logoColor=white"/></a> <a href="https://mui.com/" onClick=""><img src="https://img.shields.io/badge/MUI-007FFF?style=flat-square&logo=MUI&logoColor=white"/></a> <a href="https://nodejs.org/en" onClick=""><img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=Node.js&logoColor=white"/></a> <a href="https://www.mysql.com/" onClick=""><img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=MySQL&logoColor=white"/></a><br>

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
# 3. 시스템 구성
```bash
BYI_ERP
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
│       │   │   └── HC_Total.js
│       │   │   │       │   │   ├── HM_Move.js
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
