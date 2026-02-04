# 노션 ai 자동

2025 주간 회의록들만 따로 보면, **역할/기술/프로젝트 흐름**이 꽤 뚜렷하게 보여요. 이력서용 관점에서 핵심만 추려서 정리해볼게요.

---

### 1. 2025년에 무슨 일을 했는지 한 줄 요약

- **헬스케어 플랫폼(스마트보드, 케어웹, 인핸드매니저앱, 백오피스)** 전반에서
    - 모바일 앱 로그인·환경 전환·푸시메시지
    - 백오피스(백엔드+프론트) 디버깅 및 안정화
    - 카프카·DB·멀티테넌시 인프라 개선
    - Vercel 전환으로 클라우드 비용 절감
    
    같은 **플랫폼 레벨의 안정화·성능·비용 최적화**를 주도적으로 하고 있습니다.
    

---

### 2. 프로젝트/도메인별로 보면

**1) 관리자/운영 플랫폼 · 백오피스 / 스마트보드 / 케어웹 쪽**

- 백오피스(백엔드: NestJS, MongoDB, Kafka, AWS, 멀티테넌시)
    - JWT/JWKS 기반 인증 구조 개선, HybridJwtGuard 도입, CORS 보완 등 보안·인증 체계 강화.[[1]](https://www.notion.so/2025-4-2-2b03d5e4375f818abc95f3164e03651e?pvs=21)[[2]](https://www.notion.so/2025-4-3-2b03d5e4375f81408c43ceb8584a27ad?pvs=21)
    - MongoDB 멀티 테넌트 구조, DocumentDB·PostgreSQL 연결 안정화, 커넥션 캐시/TTL 관리 등 인프라 레벨 최적화.[[1]](https://www.notion.so/2025-4-2-2b03d5e4375f818abc95f3164e03651e?pvs=21)[[3]](https://www.notion.so/2025-4-4-2b03d5e4375f81a98e69e1f2e332d958?pvs=21)
    - Kafka 토픽 생성 권한 정리, 브로커 연결 진단, 메시지 처리 안정화.[[2]](https://www.notion.so/2025-4-3-2b03d5e4375f81408c43ceb8584a27ad?pvs=21)[[4]](https://www.notion.so/2025-7-2-2b03d5e4375f8148bab9ddaad2716d8b?pvs=21)
    - 프로젝트 생성 시 DB user 없어서 감지 안 되던 문제를 원인 분석 후 수정.[[5]](https://www.notion.so/2025-6-3-2b03d5e4375f81b3876ad5fd279e1e50?pvs=21)[[6]](https://www.notion.so/2025-6-4-2b03d5e4375f81cd834cffc2c14df522?pvs=21)
- 스마트보드 / 케어웹(웹 프론트)
    - 참여자 정보·워치 할당 등 스마트보드 관련 버그 수정, 데이터 동기화 이슈 해결.[[2]](https://www.notion.so/2025-4-3-2b03d5e4375f81408c43ceb8584a27ad?pvs=21)[[7]](https://www.notion.so/2025-7-1-2b03d5e4375f815c844bffb41456be31?pvs=21)
    - 워치 히스토리 로그가 한 박자 늦게 쌓이던 문제를 서비스 로직·트랜잭션 레벨에서 수정.[[3]](https://www.notion.so/2025-4-4-2b03d5e4375f81a98e69e1f2e332d958?pvs=21)

**2) 인핸드매니저앱(모바일 앱, Android/iOS)**

- 로그인 상태 유지, sharedPreferences 이용 자동 로그인 처리.[[8]](https://www.notion.so/2025-2-1-2b03d5e4375f818aae65c700e331e814?pvs=21)
- QA용 서버 전환 기능(아이디 접미사로 dev/test 분기) 설계 및 구현.[[9]](https://www.notion.so/2025-2-4-2b03d5e4375f81199b7affc127e91307?pvs=21)
- iOS 심사 1회 리젝 후 원인 분석 및 재심사 제출, 사이드이펙트(안드로이드 영향) 검토 계획 수립.[[10]](https://www.notion.so/2025-3-5-2b03d5e4375f8139be37ce35aeec0f34?pvs=21)

**3) 인프라/비용 절감/운영 자동화**

- 2년간 방치된 서버 발견 → 용도 변경·자동 청소 설정, 월 72% 비용 절감(연 약 15만 원 절약).[[11]](https://www.notion.so/2025-4-1-2b03d5e4375f814ca328ccf02c69d45a?pvs=21)
- ECS 기반 프론트(12개) → 전부 Vercel 서버리스로 전환, 연간 약 450만 원 절감 가능한 구조 설계·구현.[[12]](https://www.notion.so/2025-8-3-2b03d5e4375f81cdb4e5d1c9bcb0e4c4?pvs=21)
- dev/test/release 환경 분리, 로그인 페이지 환경 분리로 릴리즈 안정성 확보.[[12]](https://www.notion.so/2025-8-3-2b03d5e4375f81cdb4e5d1c9bcb0e4c4?pvs=21)

---

### 3. 기술 스택/역할 관점으로 정리

**A. 기술 스택**

- **프론트/웹**
    - Next.js, React, 국제화(i18n) 포맷 이슈 디버깅 및 해결.[[13]](https://www.notion.so/2025-5-6-2b03d5e4375f81049a82fcfc21301815?pvs=21)[[14]](https://www.notion.so/2025-6-1-2b03d5e4375f810e8ec4f865cecb299a?pvs=21)
    - Vercel 배포, 환경 분기(dev/test/release), 국제화 파일 경로 문제 해결.[[14]](https://www.notion.so/2025-6-1-2b03d5e4375f810e8ec4f865cecb299a?pvs=21)[[15]](https://www.notion.so/2025-6-2-2b03d5e4375f815093b2e8bc7baf203e?pvs=21)
- **백엔드/인프라**
    - NestJS 백오피스, MongoDB/DocumentDB, PostgreSQL, KafkaJS, AWS MSK, AWS Secrets Manager, ECS → Vercel 전환.[[1]](https://www.notion.so/2025-4-2-2b03d5e4375f818abc95f3164e03651e?pvs=21)[[2]](https://www.notion.so/2025-4-3-2b03d5e4375f81408c43ceb8584a27ad?pvs=21)[[12]](https://www.notion.so/2025-8-3-2b03d5e4375f81cdb4e5d1c9bcb0e4c4?pvs=21)
    - 멀티테넌시 DB 연결, 인증서(TLS) 자동 관리, 헬스체크·배포 스크립트 개선.[[1]](https://www.notion.so/2025-4-2-2b03d5e4375f818abc95f3164e03651e?pvs=21)
- **모바일**
    - Android 앱(sharedPreferences 로그인 상태 유지), iOS 앱 스토어 심사 대응.[[8]](https://www.notion.so/2025-2-1-2b03d5e4375f818aae65c700e331e814?pvs=21)[[10]](https://www.notion.so/2025-3-5-2b03d5e4375f8139be37ce35aeec0f34?pvs=21)

**B. 역할**

- **문제 해결형 디버거/플랫폼 스페셜리스트**
    - 국제화 포맷 오류로 인한 페이지 블랙아웃, DB user 미생성으로 인한 이벤트 미전파, 카프카 연동 불안정 등
        
        “**재현 어렵고 원인 모호한 장애**”를 직접 추적·분석·해결한 사례 다수.[[13]](https://www.notion.so/2025-5-6-2b03d5e4375f81049a82fcfc21301815?pvs=21)[[5]](https://www.notion.so/2025-6-3-2b03d5e4375f81b3876ad5fd279e1e50?pvs=21)[[6]](https://www.notion.so/2025-6-4-2b03d5e4375f81cd834cffc2c14df522?pvs=21)
        
- **인프라·비용 최적화 리드**
    - ECS → Vercel 전환 설계, 실제 비용 계산·근거 제시, 장기 비용 절감 효과까지 문서화.[[12]](https://www.notion.so/2025-8-3-2b03d5e4375f81cdb4e5d1c9bcb0e4c4?pvs=21)
    - 방치 서버 정리, 자동 청소·감시 체계 도입 등 운영 관점 개선.[[11]](https://www.notion.so/2025-4-1-2b03d5e4375f814ca328ccf02c69d45a?pvs=21)
- **커뮤니케이션·협업 서포트**
    - QA 팀/모바일 개발자에게 Postman 시나리오 제공, 디버깅 편의성/소통 효율 개선.[[16]](https://www.notion.so/2025-10-3-2b03d5e4375f812e9292fd61444635a7?pvs=21)
    - 주간 회의록 형식으로 항상 “이번 주 진행, 이슈, 다음 주 계획” 정리해서 공유 → 리드/오너십을 보여줌.

---

### 4. 이 내용을 이력서에서 어떻게 쓰면 좋은지

이 2025 페이지만 기준으로도 이런 식의 문장이 나옵니다:

- “헬스케어 백오피스(멀티테넌트, NestJS, MongoDB, Kafka)에서 인증·DB·메시지 파이프라인 장애를 진단하고, 카프카 권한 체계와 DB user 생성 로직을 개선해 프로젝트 생성 이벤트가 안정적으로 전파되도록 개선했습니다.”[[1]](https://www.notion.so/2025-4-2-2b03d5e4375f818abc95f3164e03651e?pvs=21)[[5]](https://www.notion.so/2025-6-3-2b03d5e4375f81b3876ad5fd279e1e50?pvs=21)[[6]](https://www.notion.so/2025-6-4-2b03d5e4375f81cd834cffc2c14df522?pvs=21)
- “기존 ECS 기반 프론트엔드 인프라를 Vercel 서버리스로 전환해 연간 약 450만 원의 인프라 비용 절감 효과를 만들었고, dev/test/release 환경을 분리해 배포 안정성을 높였습니다.”[[12]](https://www.notion.so/2025-8-3-2b03d5e4375f81cdb4e5d1c9bcb0e4c4?pvs=21)
- “인핸드매니저 앱에 로그인 상태 유지 기능과 QA용 서버 전환 기능을 도입하고, iOS 심사 과정에서 발생한 이슈를 분석·수정해 재심사를 통과시켰습니다.”[[8]](https://www.notion.so/2025-2-1-2b03d5e4375f818aae65c700e331e814?pvs=21)[[9]](https://www.notion.so/2025-2-4-2b03d5e4375f81199b7affc127e91307?pvs=21)[[10]](https://www.notion.so/2025-3-5-2b03d5e4375f8139be37ce35aeec0f34?pvs=21)

---

이제 다음 단계로,

- “2025년 경험만 가지고 **이력서 bullet 5~7개 뽑아줘**”
- 또는 “**비용 절감/인프라 관련 bullet만** 따로 정리해줘”

같이 요청해 주시면, 위 내용을 바로 이력서 포맷(한 줄씩 bullet)으로 변환해서 정리해 줄게요.