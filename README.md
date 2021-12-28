# FOSS_Final Project
## 2반/소프트웨어학과 201820772 김우진
## Transifex/open-edX/edX-platform 번역 프로젝트
### 1. transifex open-edx/edx-platform 주소:<br> https://www.transifex.com/open-edx/edx-platform/language/ko_KR/
### 2. 제가 번역한 문장들만 확인하실 수 있는 링크:<br> https://www.transifex.com/open-edx/search/?q=translator%3AWooJinKim

open-edx 프로젝트 중에서도 edx-platform 영역에서의 미번역 문장들을 번역했다.<br>
결론적으로, 약 1000개의 string을 번역하였으며, Words 단위론 8622개의 단어를 번역했다.<br><br>
![words](https://user-images.githubusercontent.com/89639926/147556815-096da3dd-4c73-4c70-b071-b909b534dd6d.PNG)<br>


---
# 서론

## edX란?
![words](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRXfxEf1OJvP6eVbFwZxpGDmp3vcNiessHAy0rlSbO4pj8TDsZpYv1BpVlG2yjXcc5KJD8&usqp=CAU)<br>
언제 어디서나 대학 강의를 들을 수 있는 대규모 온라인 공개강좌인 MOOC(Mass Open Online Course)을 서비스하는 대표적인 교육기관 중 하나이다.

edx에는 자유롭게 강의를 들을 수 있는 일반 과정과, 실제 대학 수강신청처럼 정해진 기간동안 강의를 시청한 후 학점을 취득하는 과정이 있다.
또한 하버드, 메사추세츠 등 세계 유수의 대학들 뿐만 아니라 MS나 LINUX 재단 등 영향력있는 단체들또한 양질의 강의를 무료로 제공해준다.<br>

## edX-Platform의 역할?
 제가 번역한 edX-Platform은 플랫폼이란 이름에서 알 수 있듯, edx 사이트의 행정 업무를 담당하고 있다.<br>
 - credentials(자격 증명)
 - ecommerce(전자 상거래)
 - account(계정 관리)
 - dashboard(학습 관리판)
 - course_discovery(강좌 탐색)<br><br>
 등 수강생이 본격적인 학습에 돌입하기 전 사용자가 필수적으로 수행해야할 이벤트가 주로 발생하는 공간이다.<br>
 
 ## edX/edX-platform 프로젝트를 선택한 이유
  edX는 필자가 생각하는 오픈 소스의 선한 영향력을 가장 잘 보여주는 사례라 생각한다. 비록 이번 학기에 열심히 학습한 SW와 관련된 오픈 소스는 아니지만, 
  교수님이 말씀해주셨듯 오픈 소스의 본질인 누구나 양질의 컨텐츠를 제공 받아 집단 지성을 이용해 이를 더 발전시킨다는 궁극적 목표를 잘 보여준다 생각한다.
  그래서 edX에 기여를 함으로써 더 많은 학우분들이 edX를 통해 양질의 컨텐츠를 제공받는데 도움을 주고 싶었다. 
  
  이 중에서도 edX-platform을 고른 이유는, 번역 전 edx-platform의 미번역 string이 2350개로 순위권에서 한참 밀려나 있었기 때문이다.<br>
  대충 원본 resource와 그 내용들을 훝어보니 edX의 가장 기초이자 중요한 내용(e.g. 계정 관리, 강좌 탐색)을 다루고 있다는 걸 알 수 있었다.
  처음엔 2350개의 string이 너무 많아 돌아갈까 했지만, 다행히 필자 포함 총 3명의 학우분이 edx-platform을 선택해서 도전해볼만 하다 생각했다.<br><br>
 
 # 번역 수행 내용
 
 ## 선택한 Resource
 총 10개의 Resouce를 번역했다.  
 - 이 중 6개는 강좌 탐색, 학습판 관리, 자격 증명, 전자상거래, 계정 관리와 관련된 내용이었다.
 - 나머지 4개는 django framework와 javascript 언어와 연관되어 있었다.

 ## 번역 방법
 
 ### 1. 번역한 자막의 문장 종결법
 문장 종결 어미는 화자의 말투나 느낌을 결정짓는 중요한 요소이다. 그러므로 resource 종류에 상관없이 종결 어미를 어떤 걸 사용할지 고려해야 했다. 필자는 platform의 특성상 사용자에게 특정 행동(e.g. 로그인, 결제)을 요구하는 경우가 많기 때문에, 사용자에게 최대한 정중하게 부탁하는 어투를 사용해야 된다 판단했다. 그래서 종결 어미는 격식체인 "~하십시오" 보단 비격식체인 "~해주세요"를 채택해 사용자에게 좀 더 부드러운 인상을 줄 수 있도록 통일했다. <br><br>
 
 ![0 jpg](https://user-images.githubusercontent.com/89639926/147548614-4029db60-c7fc-4ceb-a6ca-0e67f019af8f.PNG)<br><br>

 
 ### 2. '외래어'나 '대명사/통상적으로 쓰이는 영어 단어', '네트워크/프로그래밍 용어'는 그대로 사용
 결제 방식을 선택하거나 주의사항을 설명할 때, American Express, SKU, HUbSpot과 같은 해외 사이트나 Embago 같은 외래어들이 종종 나올 때가 있었다. 그래서 이런 명사들은 세계적으로 인지도가 높은 용어이기도 하며, 한글로 번역하면 사용자에게 혼란을 주는 경우도 있을 거 같아 영단어 그대로 사용했다.<br><br>
![1](https://user-images.githubusercontent.com/89639926/147550338-bddefdc0-fdf0-47d0-a8c4-34f3b3e4fd56.PNG)<br><br>
또한 django나 Js같은 프로그래밍 관련 내용을 번역할 땐 아무래도 백엔드와 관련된 내용이라 그런지 UTM, heartbeat, JSON, Payload같은 네트워크 용어나 import, this, super과 같은 문법 용어가 자주 사용되었다. 이런 전문적인 용어도 외래어처럼 해석을 하지 않고 그대로 사용하되, 전문 프로그래밍 용어집을 살펴보며 정말 프로그래밍 용어가 맞는지 꼼꼼히 확인했다.<br><br>

![2](https://user-images.githubusercontent.com/89639926/147550232-330dfeec-bdf6-44fb-9a34-88ba71d44f46.PNG)<br><br>
---
![3](https://user-images.githubusercontent.com/89639926/147552078-6baf77d7-4510-4a87-ab34-9dc640e129e6.PNG)<br><br>



 ### 3. 목적어/주어 생략
  원본에 'your', 'it'과 같은 주어나 목적어를 포함하는 경우가 있어도 한국어로 번역하는 과정에선 문맥상 지칭하는 물체가 확실한 경우 간결성을 위해 과감히 생략했다.
  예를 들어, 다음 문장처럼 "your ID card"라 적혀있어도 회원가입 과정은 수강생 본인 한명을 대상으로 진행하는 것이기 때문에 "귀하의 신분증 사진 업로드"가 아닌 "신분증 업로드"라 표현했다.<br><br>
 ![8](https://user-images.githubusercontent.com/89639926/147552144-6ed5975d-5bfe-4e4f-90f0-94b4b9651f41.PNG)<br><br>

  
 ### 4. TAG 안 영단어는 해석하지 않음
  다음과 같이 tag 안에 영단어가 들어있는 경우가 많았다.<br><br>
  ![9](https://user-images.githubusercontent.com/89639926/147552155-431a6999-1d12-4abb-a82d-6a327e51f4f0.PNG)<br><br>

  이는 인덱싱된 html 요소이거나 지정된 수식일 수도 있기 때문에 번역을 하지 않았다.
  
 ### 5. 시제 표현
  시제는 '과거', '현재', '미래' 총 3개로 나눠진다. 그리고 이 3개는 -ed, -ing, -will ~로 구분지었다.<br>
  - will be deleted~ : ~에서 삭제될 예정
  - Deleting.. : 삭제하는 중...
  - Deleted: 삭제되었음<br><br>

 ## 어려었던 점
 
 ### 1. 같은 단어, 다른 의미
  번역을 하면서 certificate, offer, purchase란 단어가 많이 나왔다. 하지만 resource마다 두 단어의 해석이 달라져 어떤 한국말을 선택해야 될지 많이 고민됐었다. 예를 들어, 다음과 같이 offer이 '제공하다'라는 뜻으로 쓰일 수도 있는 반면, '할인'이란 뜻으로 쓰일 수도 있었다.<br><br>
  ![5](https://user-images.githubusercontent.com/89639926/147551705-63d936bb-c96d-43c9-b12d-75db788a12e6.PNG)<br><br>
  또한 certificate는<br><br>
  ![6](https://user-images.githubusercontent.com/89639926/147551472-d10452c8-a764-455a-be4d-151c70d8f8cb.PNG)<br><br>

  강좌와 관련된 얘기를 할 때는 '이수증'의 의미로 많이 쓰이지만, 결제나 계정 정보와 관련된 얘기를 할 땐 '증명서'의 의미로 많이 사용됐다.
  이외에도 purchase또한 강좌 관련에선 '학점'의 의미를, 결제나 계정 정보와 관련해선 '구매하다'라는 의미로 사용됐다.
  비록 헷갈리긴 했지만, 경제 용어 사전의 예문을 참고하며 최대한 해석이 매끄럽게 되도로 노력했다.<br>
  
 ### 2. 단어만 주어져 문맥 파악이 힘든 경우
  다음과 같이 단어만 띡 던져진 경우가 오히려 문장이 여러개 붙어있는 경우보다 해석하기 더 힘들었다. 앞 뒤 문맥 파악을 하기 힘드므로, 이 단어가 어떤 의미로 사용될지 예측하기가 힘들었기 때문이다. 그래서 이런 단어가 있을 땐 그 resource의 전체적인 해석 방향을 생각해본 후 사전집에서 가장 적합한 뜻을 찾아 번역했다.<br><br>
 ![7](https://user-images.githubusercontent.com/89639926/147551928-5a7927a1-7a67-4893-ac41-3837a9fe5b34.PNG)<br><br>
  
  또한 다음과 같이 open이 "열다"의 동사와 "Open-edx"라는 명사 중 어떤 의미로 쓰일지도, 앞 뒤 문맥을 보고 파악했다.<br><br>
  ![8](https://user-images.githubusercontent.com/89639926/147551952-fd2611f5-0f02-4480-a43b-3ca630cb55fd.PNG)<br><br>
  
  ## 프로젝트 결과
  ### 번역 전
  ![번역 전](https://user-images.githubusercontent.com/89639926/147556233-08a989d1-3ec6-4a7d-bde8-87606c21c691.PNG)<br><br>

  ### 번역 후
  ![번역 후2](https://user-images.githubusercontent.com/89639926/147556569-b1a9567c-1f9d-4b4d-bcc1-80efee160244.PNG)<br><br>
  
  ### 개인 Reports
  ![words](https://user-images.githubusercontent.com/89639926/147556883-6ab445ee-2905-4c1c-a4d0-fef1adb3f510.PNG)<br><br>
  다른 학우가 번역한 string을 제외하면, 약 1000개의 string을 번역했다. words 단위로는 8622개의 단어를 번역했다<br><br>
  하지만 아직도 약 1000개의 string이 남아있는데, edx-platform을 번역하는 학우가 2명 더 있으므로, edx-platform의 완전 번역을 기대하고 있다.<br>
  

  ## 느낀 점
  처음엔 오픈소스인 edX를 더 완벽하게 현지화시켜 많은 학우들이 양질의 강의를 얻었으면 좋겠다는 마음에서 시작했다. 하지만 번역을 하는 과정에서 다양한 비즈니스 상황에서 쓰일 수 있는 어휘를 공부할 수 있었고, 이들을 해석하는 연습을 통해 점수를 위한 영어 공부가 아닌 실제 언어로써의 영어를 공부할 수 있었다. 또한, 문장 단위로 번역을 할 수 있으므로 공부와 뿌듯함을 동시에 잡을 수 있는 좋은 취미 활동을 얻은 것 같다. 앞으로도 꾸준히 번역을 통해 오픈소스의 부흥에 기여하고싶다.<br><br>
  그리고 이번 번역 프로젝트를 진행하면서 가장 크게 느낀 점은, 오픈 소스에 기여하는 사람들이 생각보다 정말 많다는 것이었다. 곰곰히 생각해보면 내가 지금까지 사용한 오픈소스의 번역 문장들은 누군가 자신의 시간을 할애하면서 정성스럽게 번역해준 문장들이었을 것이다. 솔직히 지금까진 이와 관련해 아무 생각이 없었기에 감사함을 느끼지 못했지만, 이번 번역 프로젝트를 진행하며 이들에게 큰 감사를 느꼈고 오픈소스 정신을 몸소 느낄 수 있었다. 이러한 정신을 바탕으로 미래에는 타인의 프로그램을 번역해주는 것 뿐만 아니라 내가 만든 프로그램이 사람들에게 널리 이롭게 쓰일 수 있는 프로그램을 만들고 싶다.
  
  ## Reference
  
  Cambridge English Dictionary: https://dictionary.cambridge.org/ko/%EC%82%AC%EC%A0%84/%EC%98%81%EC%96%B4/<br>
  TTA 정보통신용어사전: http://word.tta.or.kr/main.do<br>
  레드키위 영어학습컨텐츠: https://redkiwiapp.com/ko

