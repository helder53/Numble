## 👋 프로젝트 정보
Numble에서 제공한 사이드 프로젝트 가이드라인을 수행한 내용을 기재했습니다.<br>
프로젝트 이름은 **Spring Batch를 이용한 토스 서버**이며 프론트엔드 없이 백엔드로만 작성된 코드입니다.

## 📅 프로젝트 제작
- 제작 : 1인 개발
- 개발 기간 : 2024.04.15 ~ 2024.05.30

## 🔍 개발 환경
- Server : AWS LIGHTSAIL
- DATABASE : AWS RDS
- LANGAUGE : JAVA

## ⚒ 프로젝트 소개
프로젝트는 Spring Boot에서 Java언어를 사용해 만들었습니다.
위 프로젝트는 실제 주식을 사고파는 과정이 아닌 가상의 주식을 사고 파는 간단한 API들로 구성되어 있습니다.

주요 기능은 JWT을 활용하여 회원정보를 보호하고, Spring Batch을 사용해 주기적인 작업을 반복하도록 만들었습니다.
자세한 내용은 다음을 참고해주시면 됩니다.

## 📚 프로젝트 구조
```
├── README.md
├── .gitignore
├── .github
|    ├── workflow
│        └──CI_CD.yml
├── src
|    ├── Bank
│    │     ├── Reservation
│    │     ├── Transactions
│    │     └── UserAccount
|    ├── Batch
│    │     ├── Chunk
│    │     ├── Config
│    │     └── Schedule
|    ├── JwtToken
│    │     ├── Jwt
│    │     └── Token
|    ├── Stock
│    │     └── StockDetail
|    ├── StockTrading
|    ├── User
|    └── resource
           ├── Data
           │   └── StockData.json
           └── application.yml
```

## 📌 API 명세서
---
가이드라인에서 제시된 Method와 Param을 활용해 만든 API들은 PostMan을 이용해 명세서로 만들었습니다.
<br>
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white) : <https://documenter.getpostman.com/view/25368623/2sA3JKehmR>

## 참고자료
---
