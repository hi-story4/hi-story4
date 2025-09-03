## 안녕하세요! 비즈니스 중심 개발을 좋아하는 개발자 신준혁입니다. 👋

<!--
**hi-story4/hi-story4** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
## 현재
- 저는 온리유[Onlyou]라는 AI 결혼정보회사를 창업하여 개발/운영하고 있습니다.

## 프로젝트 
## 1. AI 결혼정보회사 온리유 [ Onlyou ]

2024.11 ~ 창업 진행 중

## 설명

### 소개

AI 결혼정보회사 온리유

기존 결혼정보회사 매니저의 역할을 AI로 대체하여 신뢰감 있는 UX 제공과 1/100 가격 혁신

현 인원

기획/마케팅/디자인 1인
기획/개발 1인
FE 개발 1인


<img width="800" height="447" alt="스크린샷 2025-07-13 오후 5 54 18" src="https://github.com/user-attachments/assets/5c3132fc-ad47-4499-bc9e-579274460dbb" />



https://onlyou.co.kr/

### 누적 **유료** 회원 8000+

<aside>
💡
고객의 매니저 만족도를 유지하며 매니저 한명이 1000명을 관리할 수 있는 시스템 구축

</aside>
### 역할

공동 대표 & CTO 

기획, 프로젝트 관리 및 개발 업무 담당

### 성과

6개월만에 매출 500% 성장

업무 시간 기존 대비 70% 효율화

데이터 기반 의사결정 & 시스템 개편 주도 성사율 2.5배 성장

### 개발 & 기획 기여

Blue-Green 방식의 안정된 무중단 CI/CD 파이프라인 구축 (AWS ALB, CodeDeploy, Gihub Actions)

유저 가입 과정 퍼널 UX 개편 

One-hot Encoding 기반 매칭 방식 → Text-Embeddign 방식 + filter 기반 매칭 방식으로의 변경하여 매칭에 소요되는 시간 2시간 → 1분 미만 최적화

유저 고객 데이터 정성&정량 데이터 분석 기반 매칭 알고리즘 개편 성사율 기존 4% → 10% 

- Random Forest Regression 기반 ML 우선
- Vector L2 Distance 유사도 기반

Legacy Code Refactoring

만남 시에만 돈을 받던 비즈니스 모델 개편 , 소개 비용 추가 → 유령회원(잠수) 문제, 수익 극대화 (기존 매출 50% 성장 )

매니저용 관리자 페이지를 통해 고객 관리, 문자 발송 등 편의성 극대화 및 자동화

유저 이탈 원인 분석 “정서적 UX” 개선 

- 일반적인 이탈 : 본인이 거절 후 마음에 드는 이성이 없을 경우 이탈,
- 서비스 정서적인 이탈: 본인이 수락하였지만 상대로부터 거절당한 후 이탈,

서비스 정서적인 이탈의 경우, 매니저의 관리, 메인화면에서의 가이드, 거절을 받을 때 약하게 받는 UX 등으로 해결하여 이탈율 감소 

## 2. 위치기반 동물병원 플랫폼[Pet To You]

---

## 프로젝트 설명

### 소개

위치기반 동물병원 플랫폼 

인원 6명 

마케팅 1인, FE 2인, 디자이너 1인, BE 지원자 포함 2인 팀 프로젝트

핵심 기능

- 카카오톡 / 네이버 소셜 로그인
- 사용자 위치 기반 주변 동물병원 검색 기능
- 위치 반경 / 병원 전문분야 / 영업 시간 / 병원 종류별 검색 가능
- 동물병원 이름 기반 검색
- 반려동물 프로필 관리
- 병원 리뷰 기능

### 기술 스택

**Backend**

- JAVA / Spring Boot
- Spring Data JPA / QueryDsl

**서버**

AWS EC2 / AWS RDS / AWS S3

Docker

![로고.jpg](https://prod-files-secure.s3.us-west-2.amazonaws.com/60af02e3-3960-4ce1-bd3b-784de6473de2/44389fcc-3ec2-4a2e-a697-2b38ae639277/%E1%84%85%E1%85%A9%E1%84%80%E1%85%A9.jpg)

**DB** 

MySQL

Redis

**도구**

QuickDBD, Postman, IntelliJ IDEA

**협업 / 디자인**

Git, GitHub, Notion

UIzard, Figma

## 기여한 점

**역할 요약** : 기획, 로직 설계, 내부 로직 구현,  쿼리 최적화, 배포

`세부 내용`

**설계&구현**

- 전체 서비스 설계
- QueryDsl을 이용한 동적 검색 기능 & 페이징 기능 구현
- ERD 설계 - 종합 예약 플랫폼으로 확장을 고려하여 Store - Hospital 상속 구조 설계
- Store, Hospital뿐만 아니라 관련된 영업시간, 리뷰, 사진 정보 CRUD API 구현
- Hospital 리스트 API의 N+1 문제 해결
- hospital Soft Delete 구현

**최적화**

- **공간 위치 기반**으로 불러오기 위해 Point 객체 타입 활용과 Mysql 의 **ST_BUFFER, ST_Contains를 이용**해 반경 N km 이내의 Hospital 또는 Store를 불러오고 St_Distance_Sphere를 이용해 얼마나 떨어져있는지 계산하는 기능 구현
- 동적 정렬 기능을 포함한 페이징 API 구현 및 최적화
- 공간 인덱스, 페이징, 쿼리 최적화 작업을 통해 응답속도를 300ms → 85ms 개선

## 3. AI View (B2B 영수증 리뷰 서비스)

---

## 프로젝트 설명

### 소개

**개인 프로젝트 (2주)**

AI 기반 OCR 기술을 활용한 영수증 리뷰 API 

스타트업을 위한 B2B API 서비스

**핵심 기능**

- Spring Security 기반 API Key-Secret 기반 인증
- AI OCR 기술 기반 영수증 사진 데이터 가공
- 영수증 검증 로직
- 리뷰 CRUD 기능
- 클라이언트별 API 사용량 측정

**세부 내용**

- 영수증 사진 데이터 → DTO 기반 데이터 가공
- 영수증 승인번호 이용한 중복 검증 & 유효성 검증
- MongoDB에 가공된 영수증 데이터 저장
- Admin & Client 권한별 회원가입 기능
- 클라이언트별 API-KEY 관리 및 사용량 측정
- Redis DB 이용 API 요청 수 캐싱 및 백업
- 외부 AI OCR 엔진 API WebClient 이용하여 요청

4. 2024 해커톤 - 나의 조각집

https://github.com/hi-story4/INTHON_BE_2nd


### 🌙 나의 조각집 – 익명 감정 공유 기반 예술 추천 커뮤니티

나의 조각집은 단순한 익명 커뮤니티를 넘어,
예술을 통해 삶의 의미를 깨닫고, 나를 이해해가는 성찰의 공간입니다.

이곳에서 사용자는 감정이 담긴 조각글을 작성하고,
비슷한 감정을 가진 이의 글에 익명으로 따뜻한 답장을 남깁니다.
또한, 그 글에 어울리는 **예술 작품(시, 음악, 미술 등)**을 추천받아
예술을 통한 위로와 자아 성찰의 경험을 얻게 됩니다.

⸻

🎯 핵심 기능
	•	감정을 담은 익명 조각글 작성
	•	비슷한 고민을 가진 유저 간 따뜻한 답장 교환
	•	GPT 기반 감성 분석 & 작품 추천
	•	감정과 연결된 예술 작품 큐레이션
	•	사용자 맞춤형 예술 기반 상품/커뮤니티 확장 가능성

⸻

🛠️ 기술 스택
	•	Frontend: React, Redux, Vercel
	•	Backend: Spring, MongoDB Atlas, CoolSMS
	•	AI/ML: GPT 4o-mini, Embedding 기반 유사도 분석
	•	Design: Figma
	•	Communication: GitHub, Notion

⸻

💡 우리가 풀고자 한 문제

“감정은 많지만, 어디에도 정리하지 못한 채 흘러가 버리는 말들.”
‘나의 조각집’은 그 감정들을 붙잡아 기록하고,
예술과 타인의 말로부터 스스로에게 필요한 말을 되돌려주는 공간입니다.




### 2025-1 캡스톤 디자인 [Docflow] : AI 대화형 문서화 시스템

DocFlow는 업무 중 발생하는 실시간 대화를 자동으로 분석하고, 문서로 정리해주는 대화형 AI 문서화 플랫폼입니다.
단순한 요약을 넘어, 발화자의 의도 파악 → 대화 흐름 추적 → 문맥 기반 검색 및 생성형 문서화까지
전 과정의 업무 문서 자동화를 지원합니다.



🔍 DocFlow가 해결하는 문제
	•	“대화는 많았지만, 결국 정리할 사람이 따로 필요하다”
	•	회의·상담·업무 협업에서 나온 결정과 맥락이 문서로 남지 않아 누락되거나 반복되는 비효율
	•	기존 RAG 기반 답변 시스템이 문서화까지 연결되지 않는 한계



💡 주요 기능

기능 구분	생성봇	검색봇
목적	대화 내용 자동 문서화	문서 기반 질의 응답
방식	대화 의도 파악 → 문서 생성	질의 → RAG 기반 문서 검색 및 답변 생성
기술	Intent Parsing, Prompt Template, Function Calling	Semantic Search, Reranking

	•	실시간 WebSocket 기반 대화 반영 구조
	•	LLM 기반 문서 요약 + 문단 구조 자동화
	•	Vector + Sparse Hybrid Search 기반 문서 검색
	•	Qdrant 기반 고속 검색 인프라 구축


🛠️ 시스템 구성
	•	프론트엔드: Next.js, Socket 기반 실시간 인터페이스
	•	백엔드: NestJS + Flask AI 서버로 분리된 구조
	•	DB/벡터DB: PostgreSQL, Qdrant
	•	배포: Docker 기반 마이크로서비스 구조


✅ 기대 효과
	•	반복적인 문서 작성 업무 자동화 → 개발 리소스 최소화
	•	검색 + 생성 + 기록이 연결된 새로운 업무 문서 환경 구축
	•	커뮤니케이션 생산성 향상 및 팀 내 정보 투명성 강화




