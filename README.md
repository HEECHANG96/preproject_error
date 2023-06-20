# preproject_progress

- project 세팅
  - [ ] DELETE `CR`  : windows에서 발생하는 오류 (https://guiyomi.tistory.com/134)
  ![image](https://github.com/HEECHANG96/preproject_error/assets/70733630/5d02bd3a-5646-4576-88bf-0f72c405f9b3)

  - [ ] "editor.defaultFormatter": "esbenp.prettier-vscode" : Visual Studio Code에서 기본적으로 사용할 코드 포맷터를 지정하는 설정, Visual Studio Code의 편집기에서 코드를 자동으로 포맷팅하는 동작을 결정
     - 코드를 저장할 때 자동으로 포맷팅된다.
     - 명시적으로 "Format Document" 또는 "Format Selection" 명령을 실행할 때 사용된다.
     - 편집기에서 코드를 작성하는 동안 실시간으로 포맷팅될 수 있다.
---
- CSS 관련
  - [ ] svg 이미지 가져오기 : (https://sunshine7e7.tistory.com/26)  
---
- Git 관련
  - [ ]  작업중인 브랜치를 add , commit하고 branch 변경하기가 애매한 상황 (https://whoyoung90.tistory.com/9)
---
- SIGNUP 기능
  - [ ]  "proxy": "http://teamdev.shop/"
       - 클라이언트 애플리케이션이 개발 서버에서 실행될 때, 클라이언트의 요청을 프록시 서버로 전달하는 역할을 한다.
       - 프록시 : 클라이언트와 서버 사이에서 중계 역할을 하는 서버
       - 장점 : 개발 서버에서 프록시 설정을 사용하면 클라이언트 애플리케이션에서 API 요청을 보낼 때, 프록시 서버를 경유하여 요청을 전달한다. 이는 개발 중에 발생할 수 있는 CORS(Cross-Origin Resource Sharing) 문제를 우회하고, 개발 서버와 API 서버 간의 도메인이 다른 경우에도 요청을 보낼 수 있도록 해준다. 프록시 설정은 주로 개발 환경에서 사용되며, 실제 배포 환경에서는 적용되지 않는다. 배포 환경에서는 API 서버와 클라이언트 애플리케이션이 동일한 도메인에서 호스팅되는 것이 일반적이다.

  - [ ] displayname, email, password
       - 서버 POST 요청 시 필요한 데이터 : name, username, email, password => displayname, email, password ()
