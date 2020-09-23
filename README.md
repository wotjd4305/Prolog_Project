# 프론트 실행 순서
1) Visual Studio Code 설치

2) 노드js 설치
https://nodejs.org/en/

3) Visual Studio Code 실행
 View > Terminal
 밑의 select Default Shell > Command Prompt
 npm install
 npm run serve
 
 
# 백 실행 순서

1) Viusal Studio Code 설치

2) Exention 설치
Java Extension Pack
Lombok Annotations Support
Spring boot Tools
Spring boot DashBoard

3) DB 설정하기
WorkBench 다운로드하고, 루트계정과 비밀번호 입력
스키마 생성
 - 이름 : daou
 - charset/collation : utf8/utf8_general_ci
SQL 파일을 열고 생성한 스키마 접속
 - use daou;
SQL문 입력!
  - 파일이름 : backend\LP_sql.sql
  - date -> datetime으로 변경(오류뜸;;)

4) application.propertis 추가하기
위치 : src\main\resources\application.properties
```sh
spring.datasource.driverClassName=com.mysql.cj.jdbc.Driver

spring.datasource.url=jdbc:mysql://localhost/ssafy_sk?serverTimezone=UTC

spring.datasource.username=root

spring.datasource.password=abc123

 

# Mail SMTP

spring.mail.host=smtp.gmail.com

spring.mail.port=587

spring.mail.username=ssafyproject124@gmail.com

spring.mail.password=sronbqwcxycongoq

spring.mail.properties.mail.smtp.starttls.enable=true

spring.mail.properties.mail.smtp.auth=true

 

spring.jpa.properties.hibernate.show_sql=true

# spring.jpa.generate-ddl=true

# spring.jpa.properties.hibernate.ddl-auto=create

 

## Multipart properties

# Enable multipart uploads

spring.servlet.multipart.enabled=true

 

# Max file size.

spring.servlet.multipart.max-file-size=200MB

 

# Max Request Size

spring.servlet.multipart.max-request-size=215MB

 

## File Storage Properties

# All files uploaded through the REST API will be stored in this directory

 

## 프로젝트내의 폴더에 업로드 파일을 설정하고 싶으면 16번째 줄처럼 

## 본인 PC의 특정 dir에 업로드 하고 싶으면 17번쨰 줄처럼 설정한다. 

#file.upload-dir=./uploads 

# file.upload-dir=/Users/multicampus/Documents/UPLOAD_FILES/Prolog

file.upload-dir=/home/ubuntu/Documents/UPLOAD_FILES/Prolog

 

 

server.servlet.context-path=/api

```
