<style>
@import url('https://cdn.jsdelivr.net/gh/orioncactus/pretendard/dist/web/static/pretendard.css');

* {
  font-family: 'Pretendard', -apple-system, BlinkMacSystemFont, system-ui, sans-serif;
}

body {
  font-size: 14px;
  line-height: 1.6;
  color: #1a1a1a;
}

h1 {
  font-size: 28px;
  font-weight: 700;
  color: #1a1a1a;
  margin-bottom: 10px;
}

h2 {
  font-size: 20px;
  font-weight: 600;
  color: #333;
  border-bottom: 2px solid #333;
  padding-bottom: 8px;
  margin-top: 30px;
}

h3 {
  font-size: 16px;
  font-weight: 600;
  color: #1a1a1a;
}

a {
  color: #0066cc;
  text-decoration: none;
}

a:hover {
  color: #004499;
  text-decoration: underline;
}

ul {
  padding-left: 20px;
}

li {
  margin-bottom: 4px;
}

strong {
  font-weight: 600;
}

hr {
  border: none;
  border-top: 1px solid #e0e0e0;
  margin: 25px 0;
}

table {
  border: none !important;
  border-collapse: collapse;
  margin-bottom: 20px;
}

table td {
  border: none !important;
}

code {
  background-color: #f4f4f4;
  padding: 2px 6px;
  border-radius: 4px;
  font-size: 13px;
}
</style>

<table width="100%" style="border: none; border-collapse: collapse;">
<tr>
<td style="border: none; vertical-align: top; padding-right: 25px;">
<img src="../../img/박시완 사진2.jpg" alt="박시완" width="130" style="border-radius: 8px;" />
</td>
<td style="border: none; vertical-align: top;">
<h1 style="margin: 0 0 10px 0; font-size: 28px;">박시완 | Frontend Developer</h1>
<p style="margin: 5px 0;"><strong>Phone</strong>: 01026559167</p>
<p style="margin: 5px 0;"><strong>Email</strong>: siwandevelop@gmail.com</p>
<p style="margin: 5px 0;"><strong>GitHub</strong>: <a href="https://github.com/park-siwan">github.com/park-siwan</a></p>
<p style="margin: 5px 0;"><strong>Location</strong>: 서울</p>
</td>
</tr>
</table>

---

## 소개

**React, Next.js, TypeScript 기반 프론트엔드 개발자 (4.5년)**

React·Next.js·TypeScript 기반으로 서비스 성능 78.75% 개선, 인프라 비용 연 450만원 절감, 디자인 시스템 구축 등 실질적 비즈니스 성과를 만들어온 프론트엔드 개발자입니다. 기획자·디자이너·QA와의 협업 워크플로를 직접 설계하고, 팀 내 기술적 병목을 선제적으로 발견·해결해온 경험이 있습니다.

**기술 스택:** JavaScript, TypeScript, React, Next.js, HTML, CSS, Tailwind CSS, Jotai, TanStack Query, react-hook-form, Chart.js, Cypress, Vercel, GitHub Actions

**AI 활용:** ChatGPT (2023~2024), Codex, Cursor, Windsurf, Claude Code, Gemini

---

## 경력

### 인핸드플러스주식회사 | 프론트엔드 개발자 (2022.06 ~ 2025.11, 3년 6개월)

_헬스케어 SaaS — B2C 투약 순응도 모니터링 서비스_

기술: React, Next.js 13~15, TypeScript, Tailwind CSS, Recoil, TanStack Query, Chart.js, Cypress

초기 주요 과제: Next.js 무경험으로 인해 빠른 학습 요구, 유지보수 불가능해진 사내 백오피스 재개발, 투자 유치를 위한 사외 의료진·복지사 전용 복약관리 백오피스 프론트 신규 기능 개발

#### 페이지 로딩 78.75% 개선
2025.02 ~ 2025.03

- **상황**: 차트 페이지 로딩에 8초 소요
- **과제**: 성능 병목을 정의하고 단계적으로 해결
- **행동**: React 번들 분석 후 코드 스플리팅·트리 셰이킹 적용 → Vercel Edge Network 서울 리전 전환
- **결과**: 8초 → 3초(62.5%) → 1.7초(43.3%), 총 78.75% 개선

#### Next.js 메모리 사용량 40% 감소 — 502 장애 해결
2024.01 ~ 2024.02

- **상황**: 운영 중 간헐적 502 Bad Gateway 발생, 원인 불명
- **과제**: 장애 근본 원인 분석 및 해결
- **행동**: 서버 로그·메모리 프로파일링으로 axios 인터셉터 중복 등록에 의한 메모리 누수 파악, HTTP/2 통신 개선
- **결과**: 메모리 사용량 40% 감소, 502 장애 완전 해소

#### ECS → Vercel 전환 제안·주도 — 연 450만원 절감
2025.05 ~ 2025.06

- **상황**: AWS ECS 운영 비용 대비 효율이 낮음
- **과제**: 인프라 비용 최적화
- **행동**: Vercel 전환을 팀에 제안하고, 전환 작업을 직접 진행·주도
- **결과**: 연간 약 450만원 인프라 비용 절감

#### 반응형 웹 설계 — 3환경 동시 서비스
2022.09 ~ 2022.12

- **상황**: 데스크톱 전용 서비스, 모바일·앱 대응 불가
- **과제**: 하나의 코드베이스로 모바일 웹·데스크톱·네이티브 앱 동시 서비스
- **행동**: Next.js + CSS 미디어쿼리 기반 반응형 전면 리뉴얼(입사 6개월 만에 단독 주도), 2025년에 Android(Kotlin)/iOS(Swift) WebView 탑재 및 네이티브 앱 빌드·배포 추가 담당
- **결과**: 하나의 React 코드베이스로 모바일 웹·데스크톱·네이티브 앱(WebView) 3환경 동시 서비스

#### React 컴포넌트 기반 디자인 시스템 구축
2022.09 ~ 2025.11

- **상황**: UI 컴포넌트 파편화, 디자이너-개발자 간 스펙 불일치 빈번
- **과제**: 디자인 스펙이 코드에 일관되게 반영되는 시스템 구축
- **행동**: Figma Dev Mode 스펙을 React + TypeScript 컴포넌트로 구현, Typography props 설계, TypeScript 타입으로 잘못된 스타일 조합 빌드 타임 차단, CSS 트랜지션 값 중앙 정의
- **결과**: 서비스 전체 인터랙션 일관성 확보, 디자인-개발 스타일 불일치 감소

#### 아키텍처 트레이드오프 판단
2025.01 ~ 2025.02

- **상황**: 프로젝트 규모 증가로 컴포넌트 간 의존성 복잡화
- **과제**: 적합한 아키텍처 선택
- **행동**: Feature-Sliced Design 학습·도입 후 운영, 생산성 저하 확인 → 트레이드오프 분석
- **결과**: React 컴포넌트 재사용 극대화를 위해 Atomic Design으로 전환 결정

#### 4개 국어 국제화 시스템
2022.09 ~ 2025.03

- **상황**: 글로벌 서비스 확장 필요, 번역 관리가 수동적
- **과제**: 다국어 지원 및 번역 협업 자동화
- **행동**: next-i18next 기반 SSR/SSG 국제화 설계, JavaScript로 Accept-Language 자동 언어 감지 구현, 노션 DB-번역 JSON 자동 동기화 시스템 개발
- **결과**: 한/중/일/영 4개 국어 지원, 기획자·QA·개발자 간 번역 협업 워크플로 구축으로 부서 간 커뮤니케이션 비용 절감

#### 데이터 시각화
2023.03 ~ 2023.06

- **상황**: 투약 순응도 차트 60개+ 데이터 포인트 시 가독성 저하 / 백오피스 정보 탐색 비효율
- **과제**: 스크롤 없는 대시보드 완성 / 관리자 UX 개선
- **행동**: Chart.js 기반 자동 생략 처리 알고리즘 JavaScript로 구현 / React 기반 실시간 검색·멀티 필터링·퀵서치 구현
- **결과**: 의료진용 직관적 대시보드 완성 / 관리자 정보 탐색 효율 개선

#### 사내 직원용 백오피스 UI 개발
2022.06 ~ 2025.11

- **상황**: 대학병원 및 제약회사별 복약관리 프로젝트 관리를 위해 필요한 복잡한 정보처리를 스프레드 시트에서 하던 방식이 여러 직원의 업무 부담이 가중됨
- **과제**: 스마트워치 등록 및 입출고 관리, 프로젝트 관리, AI 영상 분석 설정, 고객 채팅 기능, 동글 재고 관리, 기관·그룹 관리
- **행동**: MUI 활용해 빠르게 구현
- **결과**: 기본 업무 수행하며 제한 시간 내 추가 업무 구현 성공, 사내 직원의 업무 부담이 줄었으며 반복되는 휴먼에러 감소, 체계적인 프로젝트 고객관리

#### Figma Plugin 개발
2025.04 ~ 2025.05

- **상황**: 디자인 규격서 변경 시 개발자가 수동 추적 / 프론트엔드 품질 검증 체계 부재
- **과제**: 협업 병목 해소 / 자동화된 품질 검증
- **행동**: Figma Plugin API(JavaScript)로 규격서 자동 추적 도구 개발·팀 제안 / Cypress 기반 E2E 테스팅 환경 구축·시연
- **결과**: 디자이너-개발자 협업 병목 개선 제안 / 품질 검증 방식 제안

---

### 주식회사 트리피누 | 프론트엔드 개발자 (2021.05 ~ 2022.03, 11개월)

_B2C 여행 플랫폼 스타트업 — 시드 투자 유치 및 수상_

기술: React, JavaScript, Material-UI, Sass/SCSS, react-i18next

- **과제**: React 무경험으로 인해 빠른 학습 요구, 초기 스타트업에서 빠른 기능 개발과 UI 일관성 동시 달성
- **행동**: React + Atomic Design 기반 컴포넌트 라이브러리 설계, HTML/CSS 4-point grid system 적용, QA 검증으로 정합성 확인. react-leaflet(JavaScript) 220개국 여행 경로 시각화, React로 예약 시스템(회원/비회원, 계약금/잔금/환불, 다중 화폐 KRW/USD) 개발
- **결과**: 디자이너 스펙-코드 정합성 확보, 시드 투자 유치 및 수상에 기여

---

## 사이드 프로젝트

### 퀀트트레이딩 대시보드 / 자동 매매 | 2025.11 ~ 현재

_풀스택_ — React 19, Next.js 16, TypeScript, WebSocket, TradingView Lightweight Charts, Hono, CCXT, Winston, Vitest

- **상황**: 시장의 비효율성을 발견하려면 대량의 실시간 데이터를 빠르게 판단해야 하는데, 기존 도구로는 한계가 있었음
- **과제**: 데이터 기반 의사결정 → 자동화 → 수익화까지 단계적으로 해결
- **행동**: 1단계) React + WebSocket으로 10개+ 기술적 지표를 실시간 시각화하는 대시보드 구축 → 2단계) 대시보드의 판단 과정을 자동화하기 위해 Pine Script 전략 설계·백테스팅 후 TypeScript 자동매매 봇 개발 → 3단계) 봇 배포·유지보수의 진입장벽을 낮추기 위해 Bybit 카피트레이딩으로 전환하여 사용자가 별도 설정 없이 전략을 따라갈 수 있는 구조로 설계
- **결과**: Bybit 카피트레이딩 심사 통과/특별면제, 2025.12 최고의 마스터트레이더 선정. 기획부터 수익화까지 1인 완결

---

## 학력

**울산대학교 | 디지털콘텐츠디자인 전공**
2014.03 ~ 2021.02

- HTML, CSS, JavaScript, jQuery, canvas API 등의 프로그래밍 원리를 학습

**한국조형예술고등학교 | 그래픽디자인과**
2011.03 ~ 2013.03

- 포토샵, 일러스트 등을 활용한 디자인 작업

---

## 링크

- **이력서 상세 증빙**: [github.com/park-siwan/resume](https://github.com/park-siwan/resume)
- **GitHub**: [github.com/park-siwan](https://github.com/park-siwan)
