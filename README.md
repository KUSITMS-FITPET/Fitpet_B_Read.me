# Fitpet_B_Read.me


## 🛅ERD
![image](https://github.com/user-attachments/assets/04c55ae8-09d6-4a50-aeb2-ce806cb29bef)


## 🧑‍🔧기술 스택 선정 이유

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
