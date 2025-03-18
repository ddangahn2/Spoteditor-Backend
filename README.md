<div align="center">

# 계획된 코스, 그대로 즐기는 완벽한 하루 스팟에디터

![Image](https://github.com/user-attachments/assets/5a1786ab-fc34-4763-bce9-7bca40499b4b)

[Spoteditor 에서 완벽한 하루 추천받기](https://spoteditor-frontend.vercel.app/)

</div>

## 프로젝트 소개


낯선 곳을 여행할 때마다 맛집, 액티비티, 주변 명소를 찾느라 한참을 검색하곤 했어요.<br>
그런데 문득 이런 생각이 들었죠.<br>
'만약 이 도시를 잘 아는 친구가 내 코스를 계획해준다면?'<br><br>
이 작은 호기심에서 우리의 이야기가 시작됐어요.


## 내가 한 일

### 1. ERD 설계
- 유저 및 로그 테이블 구조 정의하고 ERD 설계.

### 2. 카카오 로그인 구현
- Spring Security의 `SecurityFilterChain`을 활용하여 OAuth 2.0 로그인 기능을 구현. 
- 로그인 성공 후, `successHandler`를 이용해 JWT 토큰을 발급하고 클라이언트에 전달하여 인증 시스템 구축.

### 3. Spring Security 기반 JWT 인증 처리
- `JwtFilter`를 구현하여 요청 헤더에서 JWT 토큰을 추출하고, `SecurityContextHolder`에 인증 정보를 등록하여 보안 강화. 
- `WHITE LIST`를 추가하여 JWT 없이도 접근 가능한 API 엔드포인트를 설정. 
- `JwtFilter`에서 발생하는 커스텀 응답이 덮어씌워지는 문제를 해결하여 일관된 응답을 반환하도록 수정.

### 4. AWS ELB를 활용한 HTTPS 적용 
- HTTPS 적용을 위해 도메인을 구입하고, AWS ELB(Elastic Load Balancer)를 설정하여 보안 강화. 
- SSL 인증서를 적용하여 보안 연결(HTTPS) 지원 및 트래픽을 안전하게 관리. 

### 5. Flyway를 활용한 DB 형상 관리 
- 데이터베이스 변경 사항을 체계적으로 관리하기 위해 Flyway를 도입하여 마이그레이션 자동화. 
- 태그 관리를 위한 데이터베이스 스키마 관리 수행. 
- Enum 관련 오류를 해결하여 데이터 일관성을 유지하고 애플리케이션 안정성을 개선.

### 6. 로그 기능 개발
- DB와 S3의 정합성을 유지하기 위해 `@TransactionalEventListener`를 활용하여 트랜잭션 롤백 후, 커밋 전에 정합성 유지 로직 추가.
- 로그 기능의 CRUD(생성, 조회, 수정, 삭제) 기능을 개발.

## 팀원 소개

<table>
  <tr>
    <td align="center"> 디자인</td>
    <td align="center"> 프론트엔드</td>
    <td align="center"> 프론트엔드</td>
    <td align="center"> 백엔드</td>
    <td align="center"> 백엔드</td>
  </tr>
  <tr>
    <td align="center" width="120px">
      <a href="https://github.com/hdj09" target="_blank">
        <img src="https://avatars.githubusercontent.com/u/193453479?v=4" alt="장다혜 프로필" />
      </a>
    </td>
    <td align="center" width="120px">
      <a href="https://github.com/rlaugs15" target="_blank">
        <img src="https://avatars.githubusercontent.com/u/68183848?v=4" alt="김현준 프로필" />
      </a>
    </td>
    <td align="center" width="120px">
      <a href="https://github.com/hayanLee" target="_blank">
        <img src="https://avatars.githubusercontent.com/u/164024424?v=4" alt="이하얀 프로필" />
      </a>
    </td>
    <td align="center" width="120px">
      <a href="https://github.com/dnwls16071" target="_blank">
        <img src="https://avatars.githubusercontent.com/u/106802375?v=4" alt="장우진 프로필" />
      </a>
    </td>
    <td align="center" width="120px">
      <a href="https://github.com/ddangahn2" target="_blank">
        <img src="https://avatars.githubusercontent.com/u/85681261?v=4" alt="한상안 프로필" />
      </a>
    </td>
  </tr>
  <tr>
    <td align="center">
      <a href="https://github.com/hdj09" target="_blank">
        장다혜
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/rlaugs15" target="_blank">
        김현준
      </a>
    </td> 
    <td align="center">
      <a href="https://github.com/hayanLee" target="_blank">
        이하얀
      </a>
    <td align="center">
      <a href="https://github.com/dnwls16071" target="_blank">
        장우진
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/ddangahn2" target="_blank">
        한상안
      </a>
    </td>
  </tr>
</table>

## 기술 스택

### 언어 & 프레임워크

<img src="https://img.shields.io/badge/java-007396?style=for-the-badge&logo=java&logoColor=white"><img src="https://img.shields.io/badge/springboot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white">

[//]: # (<img src="https://img.shields.io/badge/springsecurity-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white">)

### 데이터베이스

<img src="https://img.shields.io/badge/mysql-4479A1?style=for-the-badge&logo=mysql&logoColor=white">

### 인프라

<img src="https://img.shields.io/badge/docker-2496ED?style=for-the-badge&logo=docker&logoColor=white"><img src="https://img.shields.io/badge/amazonec2-FF9900?style=for-the-badge&logo=amazonec2&logoColor=white"><img src="https://img.shields.io/badge/amazonrds-527FFF?style=for-the-badge&logo=amazonrds&logoColor=white"><img src="https://img.shields.io/badge/amazons3-569A31?style=for-the-badge&logo=amazons3&logoColor=white"><img src="https://img.shields.io/badge/awselb-8C4FFF?style=for-the-badge&logo=awselasticloadbalancing&logoColor=white">


[//]: # (<img src="https://img.shields.io/badge/amazonaws-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white">)


### CI/CD

<img src="https://img.shields.io/badge/githubactions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white">

### 협업

<img src="https://img.shields.io/badge/github-181717?style=for-the-badge&logo=github&logoColor=white"><img src="https://img.shields.io/badge/discord-5865F2?style=for-the-badge&logo=discord&logoColor=white">

## ERD

![Image](https://github.com/user-attachments/assets/3568c930-c7aa-4190-bde9-ea919d57e15e)

## 인프라

<img src="https://private-user-images.githubusercontent.com/106802375/418778716-0f934fa2-57cb-4715-a0c7-e50e7872c5a8.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NDIyMDU1NjUsIm5iZiI6MTc0MjIwNTI2NSwicGF0aCI6Ii8xMDY4MDIzNzUvNDE4Nzc4NzE2LTBmOTM0ZmEyLTU3Y2ItNDcxNS1hMGM3LWU1MGU3ODcyYzVhOC5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUwMzE3JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MDMxN1QwOTU0MjVaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT02ZDM5NTk0MDQ4NjNhOGVlMDZmNjBmMTM0YTE0MjA5Y2NhMTM0YTk2NDBmODJkZTc0NTM1M2Y4YzQ4MDY4Yzk4JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.q4g9fHd6ZuiDijBB1RFcMtKydf2z2bdWuL_vqe7XEvQ" alt="인프라">

