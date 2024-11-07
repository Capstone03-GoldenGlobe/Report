# Team-Info
| (1) 과제명 | GoldenGlobe : 시니어를 위한 LLM과 RAG 기반 맞춤형 여행 챗봇, 체크리스트 서비스
|:---  |---  |
| (2) 팀 번호 / 팀 이름 | 03-이대뎅김 |
| (3) 팀 구성원 | 김근주 (2071006): 리더, 백엔드, AI, 배포 <br> 김현수 (2073100): 팀원, 프론트엔드, 와이어프레임 및 디자인  </br> 원재영 (2176225): 팀원, 백엔드, AI	|
| (4) 팀 지도교수 | 이형준 교수님 |
| (5) 팀 멘토 | 김동수 / CTO / 엘핀 |
| (6) 과제 분류 | 산학과제 |
| (7) 과제 키워드 | 여행, 시니어, 챗봇, RAG, LLM  |
| (8) 과제 내용 요약 | 시니어와, 시니어를 가족 구성원으로 둔 나머지 가족들의 효율적인 여행 준비를 돕는 서비스입니다. <br><br> 챗봇 기능을 통해 시니어가 주도적으로 여행을 파악하고 준비할 수 있도록 돕고,<br>여행지 맞춤 생성형 공유 체크리스트 기능을 통해 여행 준비의 효율성을 증대시킵니다. |

# Project-Summary
| 항목 | 내용 |
|:---  |---  |
| (1) 문제 정의 | **[본 과제를 통하여 해결 / 완화하고자 하는 문제]** <br>- 시니어 개인 혹은 시니어와 함께하는 가족이 여행을 준비할 때 겪는 여러 어려움<br><br> 1. **시니어** : 가족 여행, 해외 여행, 패키지 여행을 가고자 하는 시니어<br>	- 검색 시간 소요 : 인터넷에 익숙하지 않아 여행에 필요한 정보에 접근하는 데 시간이 많이 소요됨. 여행 관련 문서에서 필요한 정보를 찾는데 시간이 소요됨.<br> - 정보 부족 : 세부 일정을 확인하기 위해 가족의 답변을 기다리거나, 전화 상담이나 Q&A 게시판을 이용해야 하는 등 여러 절차를 거쳐야 함.<br> <br>2. **가족** : 시니어와 함께하는 여행을 떠나려는, 혹은 여행을 보내드리려는 가족(자녀 입장)<br>- 정보제공의 어려움 : 시니어와 함께 여행을 가거나 시니어의 여행을 도울 때 추가적인 설명이나 정보를 제공해야 함<br> - 준비물 공유 : 시니어와 함께 여행 준비물 목록을 한번에 공유하고 확인할 수 있는 플랫폼이 없어 불편함.<br><br>실제로 시니어와의 여행 준비 과정에서 겪는 어려움을 주제로 설문조사를 진행한 결과, <br> - 여행 관련 문서를 정리하고, 관련 정보를 찾는데 어려움을 겪었다는 응답 : **89.3%** <br>- 그 외에, 정보 제공의 어려움을 겪었다는 응답 : **48%** <br> - 준비물 준비 및 확인으로 어려움을 겪었다는 응답 **41.3%** <br>
| (2) 기존연구와의 비교 | **[유사한 과제 / 연구 / 서비스 / 시스템]** <br> - **아고다** : 고정된 키워드(ex.'캐쉬백 리워드','Acoda Cash')로만 문의 가능<br> - **익스피디아**  : 챗봇 파일 첨부 지원X -> 사용자 개개인 맞춤형 답변 제공 불가 <br> - **스카이 스캐너** : 챗봇 서비스 제공X, QnA 문의를 남기는 서비스만 존재<br> - **하나투어** : ‘AI 채팅상담 서비스'가 있으나 최신 정보 답변 X <br> - **트리플** : 챗봇 서비스 제공X, 공유 체크리스트가 있으나 기본 템플릿만 제공 <br><br><br> **[본 과제가 유사 과제에 비해 갖는 장점]** <br> **공통** : 챗봇 서비스와 체크리스트 서비스 동시에 제공한다. <br> <br> 1. **챗봇** <br> - 일반적 답변이 아닌, 관련 PDF를 기반으로 한 사용자 맞춤형 답변 제공 <br> - 고정된 키워드가 아닌, 자유로운 의사소통 기반 <br> - RAG를 기반으로 답변하기에, 거짓 없는 정확한 답변 제공 <br> <br> 2. **체크리스트** <br> - 기본 템플릿이 아닌, 여행지 날씨와 관련 PDF를 기반으로 한 맞춤형 체크리스트 제안
| (3) 제안 내용 | 시니어와 그 가족이 주도적으로 여행을 즐기고, 준비 과정을 간편하게 관리할 수 있도록 돕는다. <br> <br> **공통** : 가족 단위의 여행에 따르는 소통 부담과 피로를 덜어 더 만족감 높은 여행을 경험할 수 있다. <br><br>1. **시니어** <br> - RAG,LLM을 활용한 챗봇을 활용해 여행할 때 필요한 정보 검색 시간을 줄이고 보다 정확한 답변을 제공받는다. <br> - 체크리스트 제안 기능과 공유 체크리스트 기능을 통해 준비물 준비 시간을 줄이고, 효율적인 준비를 할 수 있다. <br><br> 2. **시니어의 가족** <br> - 체크리스트 기능을 통해 여행 준비물을 한 페이지에서 편리하게 관리할 수 있다. <br> 
| (4) 기대효과 및 의의 | - 시니어가 주도적으로 여행에 참여할 수 있다.<br>- 시니어는 챗봇을 통해 검색시간을 줄이고, 보다 정확한 답변을 제공받을 수 있다. <br>- 시니어가 여행하고자 하는 나라의 상황(날씨, 관광지, 음식 등)에 적합한 준비물을 챙겨 예상하지 못한 상황을 대비할 수 있게 된다.<br>- 시니어와 가족은 체크리스트를 통해 여행 준비물을 한꺼번에 편리하게 관리할 수 있다.<br>- 가족 단위의 여행에 따르는 소통 부담과 피로를 덜어 더 만족감 높은 여행 경험을 제공할 수 있다.
| (5) 주요 기능 리스트 | 1. '챗봇' 기능<br>- LLM, RAG를 활용하여 pdf 기반 챗봇을 생성한다.<br>- 여행 전자 영수증, 패키지 화면 pdf, 액티비티 예약 캡쳐본 등 여행 관련 문서를 저장해 두면 언제든지 해당 문서의 내용을 추출하여 정확한 질의응답을 할 수 있다.<br><br>2. '체크리스트' 기능<br>- 날씨 api와 생성형 ai를 사용해, 여행지의 특성에 맞는 맞춤형 준비물을 기본적으로 생성한다.<br>- 사용자가 업로드한 pdf 분석을 통한 준비물을 추천한다.<br>- 가족들이 함께 체크리스트를 작성하여, 시니어가 꼼꼼하게 준비물을 챙길 수 있도록 돕는다.<br>- 체크리스트에서, 가족들이 시니어에게 메모를 남겨 중요한 부분을 다시 한 번 강조할 수 있다. 


<br>
 
# Project-Design & Implementation
| 항목 | 내용 |
|:---  |---  |
| (1) 요구사항 정의 | - **요구사항 정의서** (기획의 전반적인 설명)<img width="800" alt="기능명세서1" src="./document/기능명세서1.png"><br><img width="800" alt="기능명세서2" src="./document/기능명세서2.png"><br><img width="800" alt="기능명세서3" src="./document/기능명세서3.png"><br><br>- **ui 디자인** (프론트의 전반적인 설명)<br><img width="500" alt="디자인1" src="./document/디자인1.png"><br><img width="500" alt="디자인2" src="./document/디자인2.png"><br><img width="800" alt="디자인3" src="./document/디자인3.png"><br><br>- **ER 다이어그램** (백앤드의 전반적인 설명)<br><img width="800" alt="ERD" src="./document/ERD.png"> <br><br>- **API 명세서**<br><img width="800" alt="API" src="./document/API.png">
| (2) 전체 시스템 구성 | <img width="1316" alt="SW 구조도" src="./document/시스템구성도.png">  <br> **CLIENT** <br> - Vercel : 서버리스 플랫폼으로 프론트엔드 애플리케이션을 배포하고 관리 <br> - React : 사용자가 입력한 데이터를 서버로 전송, 서버에서 받은 응답을 화면에 표시하여 시니어에 최적화된 UI 제공 <br> - Axios : 서버와 프론트엔드 간 요청 처리 <br> <br> **SERVER** <br> - Spring Boot : 프론트 요청에 따라 DB에 데이터를 저장하거나 필요한 데이터를 찾아서 응답 <br> - Flask : 프론트에서 받은 사용자의 질문을 토대로 챗봇 답변 생성 <br> - Docker : Spring Boot, Flask 서버 컨테이너화 <br> - EC2 : Docker로 패키징된 애플리케이션 호스팅 <br> - GithubActions : 코드 변경 시 배포 자동화 <br> <br> **AI** <br> - PyPdf2 : PDF 텍스트 인식<br> - LangChain : 텍스트 임베딩, 벡터화 <br> - OpenAI : 챗봇 답변 생성, 체크리스트 제안 | 
| (3) 주요 엔진 및 기능 설계 | - **회원가입/로그인**<br><img width="800" alt="회원가입로그인기능" src="./document/회원가입로그인기능.png"><br>(1) 유저에게서 회원 가입 정보(이름, 생년월일, 전화번호, 비밀번호, 닉네임, 프로필, 성별)를 입력받는다. <br>(2) 유저 정보를 담아 React에서 서버로 POST 요청을 보낸다.<br>(3) 서버에서는 사용자의 정보를 MySQL의 user 테이블에 저장한다. 이후 클라이언트 측에서 서버로 요청을 보내면 유저 정보를 조회하고 수정, 삭제할 수 있다.<br>(4) 유저가 로그인을 하게 되면 프론트에서 아이디(전화번호)와 비밀번호를 서버로 POST 한다.<br>(5) 서버에서는 이 정보를 MySQL의 user 테이블의 정보와 비교해서, 회원이 맞는지 확인하고, 맞다면 JWT 토큰을 만들어 response 메시지로 클라이언트 측에 넘겨준다.<br>(6) 이후 클라이언트는 이 토큰을 헤더에 붙여서 서버에 해당 유저가 인증된 사용자임을 확인시켜준다.<br><br>- **여행지 관리**<br><img width="800" alt="여행지관리기능" src="./document/여행지관리기능.png"><br>(1) 유저는 국가/도시/날짜를 입력해 여행지를 생성할 수 있다. 프론트는 해당 정보를 입력받아 서버에 POST 요청을 보낸다. <br>(2) 서버는 MySQL의 travelList 테이블에 해당 여행 정보를 저장한다. 이 정보를 바탕으로 여행지가 생성되며 동시에 해당 여행지와 연동된 체크리스트와 챗봇이 자동 생성된다.<br>(3) 유저는 가족의 전화번호를 입력하여 여행지를 공유할 수 있다. 여행지에 가족을 추가하면 해당 여행은 sharedList에 저장되어 공유된 모든 사용자에게 나타나게 된다.<br><br> - **챗봇** <br><img width="800" alt="챗봇기능" src="./document/챗봇기능.png"><br>(1) 유저가 챗봇에서 사용될 PDF를 업로드할 수 있다. 프론트는 해당 PDF를 서버에 POST 한다.<br>(2) 서버는 AWS S3 bucket에 PDF를 저장한다.<br>(3) 저장된 bucket 경로를 MySQL의 pdfList 테이블에 저장한다.<br>(4) 저장이 완료되면 사용자는 챗봇을 사용할 수 있다. 사용자가 질문을 던지면 서버에서는 PyPDF2를 통해 PDF의 텍스트를 인식한다.<br>(5) 인식된 텍스트는 LangChain과 HuggingFace 라이브러리를 통해 벡터화한다.<br>(6) OpenAI API를 사용해 질문에 대한 답변을 추출한다.<br>(7) 추출된 답변은 MySQL의 chatBotLog 테이블에 저장되며, 서버에서는 이 로그를 사용자에게 전달한다.<br><br> - **체크리스트**<br><img width="800" alt="체크리스트기능" src="./document/체크리스트기능.png"><br>(1) 체크리스트는 사용자가 자유롭게 그룹을 추가하고 그룹 내에 아이템(항목)을 추가할 수 있다. (예: 그룹: 세면도구 / 아이템: 칫솔, 치약)<br>(2) 그룹과 아이템은 각각 서버에 POST 된다. 각각의 그룹과 아이템은 유저가 원할 때 언제든 생성/수정/삭제할 수 있다. 각각의 API는 유저의 호출에 따라 서버에 전달된다.<br>(3) 체크리스트에는 메모 기능도 있다. 메모는 실제 포스트잇처럼 UI를 구성하였고 메모 안에 텍스트를 입력하면 서버에 전달된다. 해당 메모는 체크리스트와 함께 언제든 조회/생성/삭제할 수 있다.<br>(4) 또한 체크리스트는 자동으로 템플릿을 제공해 유저의 피로를 덜어준다. 챗봇에서 업로드한 PDF를 통해 자동으로 맞춤형 준비물을 추천하여 체크리스트를 제공한다.<br>
| (4) 주요 기능의 구현 | - **챗봇** <br><img width="800" alt="챗봇상세" src="./document/챗봇상세.png"><br>목적 : 저장된 PDF를 바탕으로, 사용자의 질문에 맞는 정확한 답변을 제공한다.<br>사용 모듈 :  React - SpringBoot(챗봇) - Database(chatBogLog, pdfList, S3 bucket) - Flask(PyPDF2, LangChain, OpenAI)<br><br>(1) 사용자가 질문을 입력한다.<br>(2) React는 사용자가 입력한 질문과, 챗봇 ID를 서버로 전송한다.<br>(3) chatBotLog 테이블에 질문을 저장하고, 챗봇 ID를 통해 pdfList 테이블에 저장된 PDF의 경로를 확인한다.<br>(4) 위에서 얻은 PDF 경로를 통해 AWS S3 bucket에서 PDF를 확인한다.<br>(5) Flask에서 PyPDF2 라이브러리를 이용해 PDF에서 텍스트를 인식한다.<br>(6) LangChain으로 인식한 텍스트를 임베딩하고, 벡터화한다.<br>(7) 벡터화된 텍스트를 가지고, OpenAI API를 이용해 입력받은 질문에 대한 답변을 생성한다.<br>(8) 생성한 답변을 chatBotLog에 저장한다.<br>(9) Spring Boot에서 생성된 답변이 포함된 챗봇 로그를 조회한다.<br>(10) 조회한 로그(답변)을 React에 전송한다.<br>(11) React에서 응답받은 로그 및 답변을 유저에게 반환한다.<br><br>- **체크리스트**<br><img width="800" alt="체크리스트상세" src="./document/체크리스트상세.png"><br>목적:저장된 PDF를 바탕으로, 사용자가 보다 편리하게 필요한 준비물을 챙길 수 있도록, 항목을 제안한다.<br>사용 모듈 : React - Database(checkList, S3 bucket) - Flask(PyPDF2, LangChain, HuggingFace, OpenAI)<br><br>(1) 사용자가 체크리스트 페이지를 조회한다.<br>(2) React는 사용자 정보와, 사용자가 접속한 체크리스트의 여행지 ID를 서버에 전송한다.<br>(3) 여행지ID로 pdfList 테이블에 저장된 PDF의 경로를 확인한다.<br>(4) 위에서 얻은 PDF 경로를 통해 AWS S3 bucket에서 PDF를 확인한다.<br>(5) Flask에서 PyPDF2 라이브러리를 이용해 PDF에서 텍스트를 인식한다.<br>(6) LangChain으로 인식한 텍스트를 임베딩하고, 벡터화한다.<br>(7) 벡터화된 텍스트를 가지고, OpenAI API를 이용해 필요한 준비물 항목을 생성한다.<br>(8) 제안된 준비물 항목을 React에 전송한다.<br>(9) React에서 응답받은 항목을 유저에게 반환한다.<br>
| (5) 기타 |  |

<br>
