## 👋 프로젝트 정보
Numble에서 제공한 사이드 프로젝트 가이드라인을 수행한 내용을 기재했습니다.<br>
프로젝트 이름은 **Spring Batch를 이용한 토스 서버**이며 프론트엔드 없이 백엔드로만 작성된 코드입니다.

<br>
<br>

## 📅 프로젝트 제작
- 제작 : 1인 개발
- 개발 기간 : 2024.04.15 ~ 2024.05.30

<br>
<br>

## 🔍 개발 환경
- Server : AWS LIGHTSAIL
- Database : AWS RDS
- Langauge : JAVA

<br>

- 간단한 API로 구성되어 있기 때문에 EC2보다 Aws Lightsail를 통해 가벼운 서버를 만들었습니다.
- Lightsail에 Database 기능이 있지만, 범용성을 위해 RDS를 사용하였습니다.

<br>
<br>

## ⚒ 프로젝트 소개
프로젝트는 Spring Boot에서 Java언어를 사용해 만들었습니다.
위 프로젝트는 실제 주식을 사고파는 과정이 아닌 가상의 주식을 사고 파는 간단한 API들로 구성되어 있습니다.

<br>

   ### 주요기능
- JWT 기능을 활용하여 회원정보를 보호했습니다.
- Spring Batch을 활용하여 예약 결제, 주식 가격 변동이 정기적인 작업을 수행하도록 했습니다.
- Github actions을 활용하여 CI/CD가 가능하도록 했습니다.

<br>
<br>

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

<br>
<br>

## 📌 API 명세서
가이드라인에서 제시된 Method와 Param을 활용해 만든 API들은 PostMan을 이용해 명세서로 만들었습니다.
<br>
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white) : <https://documenter.getpostman.com/view/25368623/2sA3JKehmR>
