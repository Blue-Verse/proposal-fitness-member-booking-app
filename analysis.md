# 피트니스 센터 통합 회원 관리 및 예약 통합 앱 구축 — 제안 분석 로그

> 생성일: 2026-04-17
> 공고 URL: https://www.wishket.com/project/154472/

---

## 1. 공고 파싱 결과

```yaml
job:
  title: "운동 센서 회원 관리 및 예약 통합 앱 구축 (피트니스 센터 통합 앱)"
  category: "개발/디자인/기획 · Android/iOS · 병원·헬스케어"
  budget_range: "15,000,000원"
  duration: "90일"
  tech_stack: []   # 자유 제안
  description: "피트니스 센터 통합 회원 관리 및 예약/소통 모바일 앱 구축"
  requirements:
    - 상세 기획 (요구사항 정의, 기능 명세, 화면 설계)
    - UI/UX 디자인
    - Android/iOS 앱 개발
    - 백엔드 개발
    - 서버/DB/인프라 구성
    - 관리자 페이지(Admin) 개발
    - 스케줄 예약 관리 (1:1 수업 예약/변경/취소)
    - 수강권 인앱 결제
    - 공통 운동 영상 + 개인별 복습 영상
    - 1:1 채팅 (영상/파일 전송)
    - 회원 관리 (가입/로그인)
    - 푸시 알림
    - 관리자 페이지 (회원/스케줄/영상/공지/결제/통계)
    - 외부 솔루션 + 네이버 예약 데이터 마이그레이션
  client_questions: []
  deadline: "2026-04-24"
  job_post_url: "https://www.wishket.com/project/154472/"
  applicants: 52
  client_profile:
    진행_분류: "신규 프로젝트"
    기획_상태: "아이디어만 있는 상태"
    IT_PM_경험: "없음"
    협업_인력: "없음"
  urls: []
  images: []
```

## 2. URL/이미지 분석

- 공고 본문 참고 URL: **없음**
- 공고 첨부 이미지: **없음**
- → 2.5단계 건너뜀, 제안 내용은 공고 텍스트 기반으로만 작성.

## 3. 실현 가능성 분석 (내부용)

### 프로젝트 유형
- **모바일 앱 (Flutter/RN) + 풀스택 + 관리자 웹** → 조건부 가능, +20% 버퍼

### 기본 공수 산정 (AI 보조 없이)
| 작업 | M/D |
|------|----:|
| 기획/설계 | 12 |
| Figma 디자인 | 18 |
| FE 모바일 (Android/iOS 2종 or Flutter 1종) | 45 |
| FE 관리자 웹 | 15 |
| BE 개발 (Auth/예약/결제/채팅/영상/푸시/마이그레이션) | 35 |
| DevOps/인프라 | 6 |
| QA/배포 | 10 |
| **합계** | **141** |

### AI 반영 및 버퍼
- AI 절감률 평균 50%: 141 × 0.5 = 70.5 M/D
- 모바일 앱 버퍼 +20%: 70.5 × 1.2 ≈ **85 M/D**
- 달력 일수 환산 (×7/5): **약 119일**

### 비교 및 판정
- 클라이언트 예상: 90일
- 내부 산정: 119일 (+32% 초과)
- 판정: 20% 초과 시나리오 — 새 기간 제안 또는 스코프 조정 필요
- **사용자 결정: 120일로 지원** — 내부 산정(119일)과 정합. 전체 스코프 무리 없이 수행 가능

### 리스크 요약
- 클라이언트 기획 상태: "아이디어만 있는 상태" → Phase 1 기획 단계에서 요구사항 구체화 필요
- 클라이언트 IT PM 경험 없음 → 커뮤니케이션·의사결정 지연 리스크 → 주간 미팅·마일스톤 서면 승인 절차로 완화
- 네이버 예약 공식 API 미공개 → CSV/엑셀 export 기반 이관, Dry-run 2회 리허설로 완화
- 앱 스토어 심사 지연(1~7일) → Phase 5 버퍼 내 수용
- "운동 센서" 키워드는 제목에만 존재, 본문 상세 요구사항에는 없음 → 범위 외(Out of Scope)로 명시

## 4. 포트폴리오 매칭

매칭 점수 기준: 기술 스택 40% / 도메인 30% / 기능 20% / 규모 10%

| 프로젝트 | 기술 | 도메인 | 기능 | 규모 | 총점 |
|----------|-----:|-------:|-----:|-----:|-----:|
| **Pilates App (필라테스 프랜차이즈)** | 30 | 30 | 20 | 9 | **89** |
| **Harmony Link (시니어 주간보호)** | 38 | 22 | 17 | 10 | **87** |
| **Calendar Share (Flutter 캘린더 앱)** | 40 | 12 | 13 | 8 | **73** |
| DayStarter (Flutter 헬스 앱) | 38 | 18 | 10 | 8 | 74 |
| Connectin (네트워킹 플랫폼) | 30 | 10 | 12 | 9 | 61 |

### 최종 선정 (3개)
1. **Pilates App** — 피트니스/예약/강사/결제/CRM 도메인 거의 일치, Android/iOS/Web 동시 출시 경험
2. **Harmony Link** — Flutter + NestJS + Next.js 관리자 웹 조합이 본 프로젝트 스택/구조와 동일, 헬스케어 도메인
3. **Calendar Share** — Flutter 단일 코드베이스로 Android/iOS 동시 배포, 예약·일정 UX, 푸시 알림 경험

## 5. 최종 제안 요약

- **지원 금액**: 13,500,000원 (VAT 별도) — 클라이언트 예산 15,000,000원의 90%
- **지원 기간**: 120일 (사용자 확정)
- **기술 스택**: Flutter(앱) · NestJS(BE) · PostgreSQL · Redis · Socket.IO · AWS S3+CloudFront · FCM/APNs · Google Play Billing/Apple IAP · Next.js(관리자)
- **핵심 제안 포인트**:
  1. 피트니스·헬스케어 도메인(필라테스/시니어 케어) 수행 경험
  2. Flutter 크로스플랫폼 + NestJS 풀스택 + Next.js 관리자 조합의 검증된 아키텍처
  3. 개인정보 비노출형 1:1 채팅 (앱 내 식별자만 사용)
  4. 공통 영상 라이브러리 + 개인 복습 영상 권한 분리형 구조
  5. 데이터 마이그레이션 전담 단계 편성 (Dry-run 2회 + 롤백 절차)

## 6. 최종 산출물 (8단계 출력 전문)

### 6.1 제안서 사이트 URL

https://proposal-router.claude-ai-b27.workers.dev/proposal-fitness-member-booking-app/

### 6.2 지원 금액 (복사용)

```
13,500,000
```

### 6.3 지원 기간 (복사용)

```
120
```

### 6.4 클라이언트 질문 답변

해당 없음 — 공고에 별도 질문 항목 없음.

### 6.5 지원 내용 (전체 텍스트 / 복사용)

```
안녕하세요, 피트니스 센터 통합 회원 관리 및 예약 통합 앱 구축 프로젝트에 지원합니다.

본 프로젝트에 대한 상세 제안서(견적서, 공수계산서, PRD, 일정, 포트폴리오)를 별도 페이지로 준비하였습니다. 아래 링크에서 확인해 주시면 감사하겠습니다.
▶ 제안서 상세 페이지: https://proposal-router.claude-ai-b27.workers.dev/proposal-fitness-member-booking-app/
▶ 위시켓 포트폴리오: https://www.wishket.com/partners/p/blueverse1/

---

<프로젝트 진행 제안>

■ 프로젝트 분석
- 회원 관리·예약·결제·영상 콘텐츠·1:1 소통을 하나의 앱으로 통합해 센터 운영 효율을 극대화하는 프로젝트로 이해했습니다.
- 핵심 가치: ① 공식 소통 창구를 통한 개인정보 비노출 ② 체계적인 운동 영상 콘텐츠 제공 ③ 기존 누적 데이터 안전한 이전.
- 기술 구성: Flutter(Android/iOS 단일 코드베이스) + NestJS + PostgreSQL + WebSocket + AWS S3/CloudFront(HLS) + FCM/APNs + Next.js 관리자.
- 유사 프로젝트 수행 경험(필라테스 프랜차이즈 앱, 시니어 주간보호 B2B SaaS, Flutter 캘린더 앱)을 기반으로 초기 시행착오를 최소화합니다.

■ 작업 일정

[Phase 1] 기획/설계 & 디자인 (Day 1–28)
- 요구사항 상세 정의, 기능 명세서, 화면 설계서 작성
- Figma UI/UX 전체 시안 (앱 + 관리자 웹)

[Phase 2] 백엔드 기반 구축 (Day 29–56)
- NestJS 프로젝트 구성, DB 스키마, Auth, 회원/스케줄/결제 API
- AWS 인프라 세팅, CI/CD 구축, Swagger API 문서

[Phase 3] 모바일 앱 핵심 기능 (Day 57–84)
- Flutter 앱: 회원가입, 예약, 인앱 결제, 공통 영상, 푸시 알림
- TestFlight / Play 내부 테스트 알파 빌드 배포

[Phase 4] 채팅/복습 영상/관리자 페이지 (Day 85–105)
- WebSocket 1:1 채팅 (영상/파일 전송), 개인 복습 영상 업로드·수신
- 관리자 웹: 회원/스케줄/영상/공지/결제/통계 전체 기능

[Phase 5] 데이터 이관 · QA · 스토어 배포 (Day 106–120)
- 외부 솔루션 + 네이버 예약 데이터 Dry-run 2회 후 실이관
- 전체 QA (회귀/성능/보안), Android/iOS 스토어 심사 및 런칭

■ 마일스톤 및 산출물
- M1 (Day 28): 요구사항 정의서, 기능 명세서, 화면 설계서, Figma 시안
- M2 (Day 56): DB 스키마, API 명세서, Auth/회원/예약/결제 API
- M3 (Day 84): TestFlight/Play 내부 테스트 알파 빌드
- M4 (Day 105): 관리자 페이지 v1, 1:1 채팅/복습 영상 완성, 통합 QA 진입
- M5 (Day 120): 데이터 마이그레이션 검증 완료, Android/iOS 스토어 정식 출시, 운영/배포 가이드 인계

■ 미팅 시 협의 필요 사항
- 수강권 상품 구조 (회차제 vs 기간제 vs 혼합), 환불 정책
- 인앱 결제 외 대체 결제 수단 필요 여부 (PG 연동 확장)
- 기존 외부 솔루션/네이버 예약 데이터 export 가능 형식 (CSV/엑셀/API)
- 공통 영상 원본 공급 경로 (유튜브 링크 / 자체 제작 원본 업로드 비율)
- 센터 지점 수 (단일 센터 vs 향후 다중 지점 확장 여부)
- 강사 회원가입 플로우 (관리자 초대 방식 vs 직접 가입)

---

<유사 프로젝트 진행 경험>

▶ 필라테스 프랜차이즈 관리 앱 (2019.09–2019.12, 4개월)
- 프로젝트 유형: B2B2C 피트니스 앱 / Android+iOS+Web 동시 출시
- 핵심 기능: 수업 예약, 강사 관리, 출결 관리, 결제, CRM, 커뮤니티
- 유사점: 피트니스 센터 도메인과 회원·강사·수업 예약 데이터 모델 동일, 수강권/결제 운영 경험, 앱 스토어 심사/배포 프로세스 숙달
- 기술 스택: React Native, React, Node.js, JavaScript

▶ 시니어 주간보호 관리 플랫폼 (2025, 약 6개월)
- 프로젝트 유형: B2B SaaS 헬스케어 / Flutter 앱 + Next.js 관리자
- 핵심 기능: 케어 로그·투약 관리, 보호자 커뮤니케이션, AI 건강 분석, 전자서명, 멀티테넌트
- 유사점: Flutter + NestJS + Next.js 관리자 조합이 본 프로젝트 구조와 동일, AWS 인프라·실시간 커뮤니케이션·푸시 알림·사용자 권한 분리 경험
- 기술 스택: Flutter, NestJS, Next.js, TypeScript, MySQL, AWS CDK, Docker

▶ 소셜 캘린더 앱 (2025.01~, MVP)
- 프로젝트 유형: B2C Flutter 앱 / Android+iOS
- 핵심 기능: 캘린더·일정 관리, 소셜 피드, 7종 푸시 알림, 실시간 동기화
- 유사점: Flutter 단일 코드베이스로 Android/iOS 동시 배포, 예약·일정 UX(시간대 선택·캘린더 뷰·충돌 방지) 구현, FCM 푸시 경험
- 기술 스택: Flutter 3, Firebase, Supabase, FCM

---

<사용 기술과 툴>

▶ 개발 기술
- 모바일: Flutter (Dart), Riverpod
- 백엔드: NestJS (TypeScript), PostgreSQL, Redis, Socket.IO
- 영상/파일: AWS S3, CloudFront (HLS 스트리밍)
- 알림/결제: FCM, APNs, Google Play Billing, Apple IAP
- 관리자 웹: Next.js, React, TailwindCSS
- 컨테이너/배포: Docker, GitHub Actions

▶ 개발 도구 및 인프라
- 버전 관리: GitHub
- CI/CD: GitHub Actions
- 클라우드: AWS (EC2, RDS, S3, CloudFront, SES, CloudWatch)
- 컨테이너: Docker

▶ 커뮤니케이션
- 일일 진행 공유: Slack 또는 카카오톡
- 주간 미팅: Zoom / Google Meet
- 문서 공유: Notion 또는 Google Docs
- 이슈 트래킹: GitHub Issues
```

### 6.6 관련 포트폴리오 추천 (위시켓 폼 선택용)

1. **필라테스 프랜차이즈 관리 앱** — 피트니스 도메인과 예약/강사/결제/CRM 기능이 거의 일치, Android/iOS/Web 동시 출시 경험
2. **시니어 주간보호 관리 플랫폼 (Harmony Link)** — Flutter 앱 + Next.js 관리자 + NestJS 백엔드 조합이 본 프로젝트 구조와 동일, 헬스케어 도메인 경험
3. **소셜 캘린더 앱 (Calendar Share)** — Flutter 단일 코드베이스로 Android/iOS 동시 배포 경험, 예약·일정 UX, FCM 푸시 경험
