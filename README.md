# Fitpet_B_Read.me

## PLANNER

| Profile | Name | Role |
| :---: | :---: | :---: |
| <a href="https://github.com/go-myang"><img src="https://avatars.githubusercontent.com/u/175245394?v=4" height="120px"></a> | NAYOUNG HAN <br> **go-myang**| Create a Docker Image for Inferring UVR Models <br> Manage AWS S3 buckets, Lambda, and API gateways <br> Managing singtome project model experiments|
| <a href="https://github.com/ssominging"><img src="https://avatars.githubusercontent.com/u/180842955?v=4" height="120px"></a> | SOMIN PARK <br> **ssominging**| Create a Docker Image for Inferring UVR Models <br> Manage AWS S3 buckets, Lambda, and API gateways <br> Managing singtome project model experiments|
| <a href=""><img src="" height="120px"></a> | SARANG YUN <br> **ssominging**||

## FRONTEND

| Profile | Name | Role |
| :---: | :---: | :---: |
| <a href="https://github.com/karnelll"><img src="https://avatars.githubusercontent.com/u/165611407?v=4" height="120px"></a> | SEOHEE CHOI <br> **karnelll**| Create a Docker Image for Inferring UVR Models <br> Manage AWS S3 buckets, Lambda, and API gateways <br> Managing singtome project model experiments|
| <a href="https://github.com/yeyounging"><img src="https://avatars.githubusercontent.com/u/133792082?v=4" height="120px"></a> | YEYOUNG KONG <br> **yeyounging**| Create a Docker Image for Inferring UVR Models <br> Manage AWS S3 buckets, Lambda, and API gateways <br> Managing singtome project model experiments|

## BACKEND

| Profile | Name | Role |
| :---: | :---: | :---: |
| <a href="https://github.com/anselmo228"><img src="https://avatars.githubusercontent.com/u/24919880?v=4" height="120px"></a> | Heechan Chung <br> **anselmo**| Create a Docker Image for Inferring UVR Models <br> Manage AWS S3 buckets, Lambda, and API gateways <br> Managing singtome project model experiments|
| <a href="https://github.com/L-U-Ready"><img src="https://avatars.githubusercontent.com/u/123285545?v=4" height="120px"></a> | YUJOON LEE <br> **L-U-Ready**| Create a Docker Image for Inferring UVR Models <br> Manage AWS S3 buckets, Lambda, and API gateways <br> Managing singtome project model experiments|

## DESIGNER

| Profile | Name | Role |
| :---: | :---: | :---: |
| <a href="https://github.com/lkrko"><img src="https://avatars.githubusercontent.com/u/126140379?v=4" height="120px"></a> | CHAEYEON KIM <br> **lkrko**| |
| <a href=""><img src="" height="120px"></a> | SEOUEN LEE <br> | |

## 🛅ERD
![image](https://github.com/user-attachments/assets/04c55ae8-09d6-4a50-aeb2-ce806cb29bef)


## 🧑‍🔧기술 스택 선정 이유

### **Server**
- **EC2:** AWS EC2를 사용하여 백엔드 서버를 호스팅했습니다.
- **RDS:** AWS RDS를 사용해 MySQL 데이터베이스를 관리했습니다.
- **S3:** AWS S3를 통해 파일 저장소를 구현했습니다.
- **Vercel:** Vercel을 사용하여 프론트엔드 애플리케이션을 배포했습니다.

### **Frontend**

- **Next.js 14:** 서버사이드 렌더링(SSR)과 정적 사이트 생성(SSG)으로 빠른 초기 화면 렌더링과 SEO 최적화가 가능합니다.
    - page router
- **React:** 컴포넌트 기반으로 UI를 모듈화해 빠르고 효율적인 업데이트가 가능하며, 재사용성 높은 코드로 유지보수가 용이합니다.
- **TypeScript:** 정적 타입 검사로 코드 안정성을 높이고 디버깅을 쉽게 합니다.
- **TailwindCSS:** 유틸리티 클래스 기반으로 신속하고 일관된 스타일링이 가능합니다.

> **백엔드 스택 선정과 이유**

### **Backend**

- **Layered Architecture in DDD:** 복잡한 비즈니스 로직을 체계적으로 관리하고 확장성을 높입니다.

```
└─fitpet_be
    ├─application
    │  ├─dto
    │  │  ├─request
    │  │  └─response
    │  ├─exception
    │  ├─service
    │  └─serviceImpl
    ├─common
    │  └─config
    ├─domain
    │  ├─model
    │  └─repository
    ├─infrastructure
    │  ├─jwt
    │  ├─persistence
    │  ├─s3
    │  └─utils
    └─presentation
        └─controller
```
- **CQRS:** 읽기와 쓰기 작업을 분리해 성능과 데이터 일관성을 유지합니다.
- **Java 17:** 안정성과 보안을 제공하며, 최신 LTS 기능을 활용할 수 있습니다.
- **Spring Boot:** 빠른 개발과 표준화된 코드 구조를 지원합니다.
- **Spring Data JPA, Swagger, Logback, AWS 등:** 데이터 접근, API 문서화, 로깅, 클라우드 인프라 활용을 간소화합니다.

- **JWT(Jason Web Token)**: 현대 웹 애플리케이션에서 인증과 권한 부여를 위해 널리 사용되는 기술로, 서버와 클라이언트 간의 데이터를 안전하게 주고받을 수 있도록 해줍니다. 관리자 인증, 인가에 사용했습니다.
- **Aspose.Cells**: 보험료 견적서에 사용된 Microsoft Excel를 생성, 읽기, 조작, 변환 및 보호하기 위한 클라우드 API입니다.
- **Apache POI**: Microsoft Excel 포맷을 순수 자바 언어로서 읽고 쓰는 기능을 제공합니다. 보험료 견적서에 사용자의 정보를 입력하기 위해 사용했습니다.

### **API Documentation**

- **Swagger:** Controller 기반으로 자동화된 API 문서를 생성하여 정확성과 신뢰성을 높입니다. (http://3.35.191.40:8080/swagger-ui/index.html#/)

### **GIT FLOW**
<img width="256" alt="KakaoTalk_Photo_2024-09-08-22-32-07" src="https://github.com/user-attachments/assets/b9c35b22-0473-4e10-acc7-bae9caf36516">

GitHub Flow는 모든 개발을 기능 브랜치에서 독립적으로 진행한 후, 코드 리뷰를 거쳐 master 브랜치로 병합하고, 배포하는 간단하고 효율적인 방식입니다. 이 방법은 빠른 배포 주기가 필요한 프로젝트에 적합합니다.

이 이미지에서 각 색깔의 노드는 브랜치의 각각의 커밋을 나타내며, 병합 화살표는 각 기능 브랜치가 master 브랜치로 병합되는 과정을 설명하고 있습니다.
