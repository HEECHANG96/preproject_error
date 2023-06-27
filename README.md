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
  - [ ] svg 파일 정리
![image](https://github.com/HEECHANG96/preproject_progress/assets/70733630/3c340720-d2d9-431e-9bf0-7d4cba213784)
![image](https://github.com/HEECHANG96/preproject_progress/assets/70733630/ee06ba6f-7d58-490d-b9d2-bf473207fa03)


---
- Git 관련
  - [ ]  작업중인 브랜치를 add , commit하고 branch 변경하기가 애매한 상황 (https://whoyoung90.tistory.com/9)
  - [ ]  프론트엔드 작업물 합치기
       - GitHub repository의 dev branch를 Local dev branch에서 git pull
       - 새로운 branch test 생성
       - test branch에서 예를 들어 내가 작업한 feat/signup branch를 git merge
       - test = dev + feat/signup이 합쳐짐
  
---
- SIGNUP 기능
  - [ ]  "proxy": "http://teamdev.shop/"
       - 클라이언트 애플리케이션이 개발 서버에서 실행될 때, 클라이언트의 요청을 프록시 서버로 전달하는 역할을 한다.
       - 프록시 : 클라이언트와 서버 사이에서 중계 역할을 하는 서버
       - 장점 : 개발 서버에서 프록시 설정을 사용하면 클라이언트 애플리케이션에서 API 요청을 보낼 때, 프록시 서버를 경유하여 요청을 전달한다. 이는 개발 중에 발생할 수 있는 CORS(Cross-Origin Resource Sharing) 문제를 우회하고, 개발 서버와 API 서버 간의 도메인이 다른 경우에도 요청을 보낼 수 있도록 해준다. 프록시 설정은 주로 개발 환경에서 사용되며, 실제 배포 환경에서는 적용되지 않는다. 배포 환경에서는 API 서버와 클라이언트 애플리케이션이 동일한 도메인에서 호스팅되는 것이 일반적이다.
  - [ ] CORS 에러
       - "proxy": "https://teamdev.shop/"으로 수정
       - npm i 후 npm start 

  - [ ] displayname, email, password
       - 서버 POST 요청 시 필요한 데이터 : name, username, email, password => displayname, email, password => username, email, password
---
 - LOGIN 기능
   - [ ] email, password
       - 서버 POST 요청 시 필요한 데이터 : email, password => 로그인할 때 유효성 검사(X) => Main Project할 때는 하기
   - [ ] Oauth 로그인
       - 백엔드에서 로직을 다 구현해주고 프론트에서 axios로 해당 url에 GET 요청 => CORS 에러 및 302, 40X 에러 다양하게 발생
   - [ ] HEADER LOGIN 버튼
       - 로그인 버튼 클릭하면 login page로 이동
---
 - LOGOUT 기능
   - [ ] HEADER에서 LOGOUT 버튼
       - 버튼 클릭하면 LocalStorage에 있는 accessToken, memberId 삭제
       - 버튼 클릭하면 store에 저장되어 있는 memberId 값을 null로 설정 
---
 - Zustand
   - [ ] store.ts 구현

![image](https://github.com/HEECHANG96/preproject_progress/assets/70733630/b2d08927-318d-4e7c-8d1b-0cde0366bed3)

---
 - 배포 환경
   - [ ] 로그인을 하면 헤더가 바뀌지 않음
       - CORS 에러
       - config.addExposedHeader("Authorization"); config.addExposedHeader("memberId");
       - https://kingchan223.tistory.com/230
       - ![CORS 에러](https://github.com/HEECHANG96/preproject_progress/assets/70733630/f6c7ca90-2ad0-4a38-8bc2-facbad732718)
   - [ ] 회원가입
       - if (res.status !== 200) throw res; => if (res.status !== 201) throw res; 서버에서 201코드로 보내줌!

---
 - 프리 프로젝트 하면서 느낀점
      - [ ] 프론트 - 백엔드 소통 너무 중요하다..
      - [ ] 수면 시간의 균일화.. (생각보다 중요)
