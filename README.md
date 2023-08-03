# SSTV[PL]

한 줄 소개: 누구나 자신만의 방송을 송출 하거나 다른 사람의 스트리밍을 시청 할 수 있는 서비스                          후원과 광고를 통해 수익창출까지 가능한 웹 서비스
진행기간: 2023년 3월 28일 → 2023년 6월 5일
사용 Skill: Docker, Express, Java, JavaScript, Jenkins, MyBatis, MySQL, NaverCloud, Node.js, React.js, Redis, SpringBoot


## 📝 상세 내용

---
### 시연영상
[![Video Label](http://img.youtube.com/vi/ClLhoWd68eo&t=2s/0.jpg)](https://www.youtube.com/watch?v=ClLhoWd68eo&t=2s)


<aside>
💡 **“[네이버클라우드] 클라우드 기반의 AIaaS 개발자 과정”** 부트캠프에 참여하면서 개발한 팀 프로젝트입니다. 회원가입만 한다면 누구든지 자신만의 스트리밍을 송출하고 다른 회원들의 스트리밍을 시청 가능하며 서브 시스템으로는 스트리밍·후원·광고·정지·신고·커뮤니티·채팅·SNS로그인·결제 등이 있습니다.

</aside>

## 🛠️  사용기술 및 라이브러리

---

### Front

- JavaScript
- React.js
- Axios
- socket.io-client

### Back

- Java, JavaScript
- SpringBoot
- Node.js, Express
- socket.io
- MyBatis
- Redis
- MySQL

### DevOps

- Docker, Jenkins

## 👽 내 담당 기능

---

### 스트리밍 서브시스템 구현

- NaverCloud LiveStation API를 통한 스트리밍 생성 및 송출 구현
- 스트리밍 종료시 NaverCloud ObjectStorage에 녹화본 업로드 구현
- socket.io를 통한 실시간 시청자수, 실시간 제목, 카테고리 변경 구현

### **광고 서브시스템 구현**

- LiveStaion API의 LiveCurtain기능을 통해 사이트에서 재생중인 모든 스트리밍에 광고 송출 구현
- NaverCloud ObjectStroage를 통해 광고영상을 Cloud에서 관리
- 광고 시청 회원수, 재생횟수 구현

### **후원 서브시스템 구현**

- Clova Voice를 통해 후원 메시지를 음성으로 변환
- socket.io를 통해 같은 스트리밍 시청중인 모든 회원들에게 후원영상 송출 구현

### **정지 서브시스템 구현**

- 정지 서비스에 대한 CRUD 구현

### **신고 서브시스템 구현**

- 신고 서비스에 대한 CRUD 구현

### **운영서버 구축**

- NaverCloud Server와 Docker를 사용하여 React, Node.js, SpringBoot Web Application Server 구축

### **CI/CD**

- Jenkins 사용하여 GitHub push시 운영서버에 자동으로 배포되는 환경 구축

### **ETC**

- 프로젝트 문서 정리 및 발표 시연동영상 제작

## 👁️  프로젝트 기여도

---

|  | 이동욱[PL] | 전지창 | 이재익 | 김영훈 |
| --- | --- | --- | --- | --- |
| SpringBoot Git Repo Commit | 1회 | 31회 | 84회 | 12회 |
| SpringBoot Git Repo Commit SourceCode | 57라인 | 2,650라인 | 2,028라인 | 1,029라인 |
| React.js Git Repo Commit  | 53회 | 31회 | 36회 | 12회 |
| React.js Git Repo Commit SourceCode | 126,295라인 | 329,410라인 | 99,283라인 | 2,979라인 |
| Node.js Git Repo Commit  | 41회 | 7회 | 0회 | 0회 |
| Node.js Git Repo Commit SourceCode | 10,941라인 | 472라인 | 0라인 | 0라인 |
| 참여 모듈 개수(총 10개) | 5개 | 2개 | 1개 | 1개 |
| 개발문서 작성횟수 | 76회 | 67회 | 46회 | 24회 |

## 💡느낀 점

---

- **첫 개발문서 작업**
    
    처음 프로젝트를 시작할때 구현에 투자하는 시간보다 분석, 설계에 투자하는 시간이 훨씬 길어 의아하였지만 요구사항정의서, 화면정의서, VOPC, UseCase Diagram, ERD 등의 문서를 직접 작성해 보면서  그 이유를 알게되었다. 
    
    구현 단계의 후반에서 분석, 설계때 놓쳤던 부분을 임의로 추가하다보니 해당 기능의 개발 시간이 목표 한 시간보다 길어졌고 이를 통해 구현단계의 코드들은 모두 분석, 설계의 문서를 통해 작성 되며 구현 단계의 시간을 단축 시킨다는것을 알게 되었다. 
    
- **과유불급**
    
    제대로 된 첫 팀 프로젝트이고 팀장의 역할을 맡다보니 의욕이 넘쳐서 5개의 모듈을 담당하게 되었다. 각 모듈들의 제일 핵심적인 기능들은 다 구현 하였으나 페이지 새로고침 시 검색어 및 페이지 유지, 일반 회원이 URL을 통해 관리자 페이지 접근 차단 등 기타 중요한 부분들을 구현 못해 완성도가 떨어지는 모듈을 개발하여 아쉬움이 남았다.
    

- **팀장은 어렵구나…**
    
    이번 프로젝트는 총 4명의 팀으로 진행하였다. 코드나 개발 문서에 대한 1차 피드백 이후 고쳐지지 않은 부분이 있으면 지속적으로 피드백을 주어야 하지만 팀원 중 막내이고 성격상 아쉬운 말에 익숙하지 않은 성격이다보니 2차 피드백 없이 내가 직접 고쳤다. 그렇다보니 작업량이 늘어나 나의 담당 부분에도 영향을 주었고 이를통해  처음에는 약간 시간이 걸리더라도 지속적인 피드백을 통해 같이 고쳐나가는것이 훨씬 빠르고 중요하다는 것을 알게 되었다.  
    

## ℹ️  참고 링크 및 참고 자료

---

### **👉🏻[프로젝트 정보](https://ncamp.magicecole.com/Home/Project/d31fc2a2-9ba8-446d-992e-e24ab19a4ba1?page=1&groupId=0)**

### **👉🏻[GitHub](https://github.com/Function3333/SSTV)**

### **👉🏻[개발문서](https://drive.google.com/file/d/16rpcxlEaF1jE1zu4NNm2QKRmzrr3ziXH/view?usp=sharing)**

### **👉🏻[발표영상](https://www.youtube.com/watch?v=1nqyNu48TiA&t=1136s)**
