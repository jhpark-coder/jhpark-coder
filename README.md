# 박준호 | 웹 풀스택 개발자

> 화면부터 서버, 배포까지 혼자 완성해 온 풀스택 개발자입니다.

React·TypeScript 화면과 Python FastAPI 서버로 사내에서 실제로 쓰는 앱을 만들고 있습니다.
사용자 조작이 많은 화면을 만드는 일과, 자동 테스트로 바뀐 코드가 기존 기능을 깨지 않는지 확인하는 일을 중요하게 여깁니다.

- 현재: **주식회사 제이엘티 기업부설연구소 연구원** · 풀스택 개발 (2025.11 ~ 현재)
- 실무에서 쓰는 기술: **React · TypeScript · Python FastAPI · SQLite · Electron · C#**
- 프로젝트에서 쓴 기술: Java Spring Boot · NestJS · MySQL · Docker · AWS
- Contact: **pjh133765@gmail.com** · [Blog](https://primotion.tistory.com/)

## Career

### 주식회사 제이엘티 · 기업부설연구소

`2025.11 ~ 현재` · 연구원 · 풀스택 개발

#### 사내 업무 자동화 데스크톱 앱

`React 19` `TypeScript` `Electron` `Python FastAPI` `SQLAlchemy` `SQLite` `C#/.NET`

엑셀로 주고받던 설계 데이터를 불러와 계산하고, 결과를 편집기에서 다듬어 문서와 PDF로 자동 생성하는 사내 앱입니다. 입사 첫 달 이후 설계부터 구현, 테스트, 배포까지 혼자 맡고 있습니다.

- **아키텍처**: React 화면, 로컬 FastAPI 서버, SQLite를 Electron 하나로 묶는 구조 설계. PyInstaller·NSIS로 패키징해 사용자 PC에 Python·Node 없이 설치
- **구조 전환**: 기존 C# WinForms 앱을 Avalonia로 옮기며 Clean Architecture를 적용했고, 이후 React·Electron 구조로 다시 전환
- **그래프 편집기**: JointJS 기반 노드·연결선 편집기, 직교 경로 자동 계산, Undo/Redo. 노드가 많아질수록 느려지던 편집 속도를 경로 탐색 범위 축소와 렌더링 분리로 개선
- **엑셀식 데이터 표**: 6개 화면이 각자 구현하던 표를 공통 컴포넌트 하나로 통일 (범위 선택, Excel 복사·붙여넣기, 채우기, 정렬·필터, 실행 취소)
- **데이터 처리**: 엑셀을 불러와 항목을 매핑하고 규칙대로 계산·매칭, 계산 근거 보존. 규칙 문서가 없어 실제 결과물을 거꾸로 분석해 규칙을 찾아냄
- **안정성**: 편집 중인 문서를 IndexedDB에 자동 백업, 저장 요청을 프로젝트별 큐로 순서대로 처리
- **품질**: 자동 테스트 약 4,000건(pytest 2,976건, 프런트 1,200여 건), 실제 결과물을 정답으로 삼는 회귀 테스트
- **배포**: `develop` · `release/` · `hotfix/` 브랜치 전략과 배포 절차 정리

#### 그 외 업무

- **사내규정 RAG 챗봇** (`2026.09` · 단독): PDF 조항·병합 표 파싱, 벡터 검색, 로컬 LLM 답변과 근거 검증, 관리자 화면까지 혼자 개발
- **사내 견적 관리 시스템** (`2025.12 ~ 2026.01` · 2명): 프론트엔드를 맡아 백엔드 개발자와 API를 맞추며 화면 구현
- **PLC 코드 생성 AI · 엑셀 변환 모듈** (`2026.07 ~ 2026.09` · 3명): 설비 제어 엑셀 파싱·변환 담당, 데이터 형식을 먼저 정하고 검증한 뒤 병합
- **설비 측정 PC 로거** (`2026.06 ~ 2026.07` · 단독): C# WPF로 PLC 통신, 측정값 판정, CSV 저장 구현, 고객사 현장 시연

> 회사 프로젝트의 소스 코드와 화면은 비공개라 링크를 넣지 않았습니다.

## Tech Stack

**Frontend**

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Zustand](https://img.shields.io/badge/Zustand-443E38?style=flat-square)
![Three.js](https://img.shields.io/badge/Three.js-000000?style=flat-square&logo=threedotjs&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)

**Backend**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Java](https://img.shields.io/badge/Java-007396?style=flat-square)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white)

**Database · Infra**

![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

**Desktop · Test · AI**

![Electron](https://img.shields.io/badge/Electron-47848F?style=flat-square&logo=electron&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)
![Vitest](https://img.shields.io/badge/Vitest-6E9F18?style=flat-square&logo=vitest&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)

## Featured Projects

### Interior Simulator

`2026.02 ~ 2026.10` · 개인 프로젝트 · [Repository](https://github.com/jhpark-coder/Interior-Simulator)

`React 19` `TypeScript` `Konva` `React Three Fiber` `Zustand` `Zod` `Vitest`

방 구조와 가구를 2D에서 편집하고, 같은 데이터를 3D 공간에서 바로 확인하는 인테리어 배치 웹앱입니다.

- React Konva 기반 2D 편집기와 React Three Fiber 기반 3D 장면을 **하나의 Zustand 상태로 동기화**
- 가구·문·창문 배치, 그리드 스냅, 벽 경계·가구 간 충돌 검사
- 문·창문 개폐, 수납장·서랍·모니터암 등 상호작용 가능한 3D 모델
- Undo/Redo, Zod 스키마 검증을 거치는 JSON 저장·불러오기와 자동 저장
- Vitest로 좌표 변환·스냅·히스토리·스키마 단위 테스트

### DevMate

`2025.10 ~` · 개인 프로젝트 · [Repository](https://github.com/jhpark-coder/devmate)

`Python` `LangChain` `FAISS` `Ollama` `Streamlit` `pytest`

22개 기술의 공식 문서를 한국어로 질문하면 근거 문서와 함께 답하는 RAG 챗봇입니다. API 키 없이 로컬에서만 동작합니다.

- 140개 문서를 나눠 다국어 임베딩(bge-m3)으로 FAISS에 색인, **한국어 질문으로 영어 원문 검색**
- 답변마다 유사도와 원문 미리보기로 출처 표시
- LLM과 임베딩을 인터페이스로 감싸, OpenAI에서 로컬 Ollama로 바꿀 때 해당 계층만 수정
- Domain·Application·Infrastructure 계층 분리, 단위·통합·E2E 테스트

### AUTOMATA — 3D 인터랙티브 웹 매뉴얼

`2026.07 ~ 2026.08` · 개인 프로젝트 · [Repository](https://github.com/jhpark-coder/automata-plc-manual)

`Next.js 16` `React 19` `Three.js` `Cloudflare`

산업 장비 41종의 생김새와 동작을 3D로 돌려 보며 배우는 한국어 인터랙티브 학습 사이트입니다.

- 회전·확대할 수 있는 WebGL 3D 모델과 가동부 애니메이션
- 동작 순서에 따라 바뀌는 상태 패널과 제어 명령 표시
- 동작 버튼 98개의 타이밍·상태·복귀 자세를 Playwright로 자동 검증하는 스크립트
- Next.js로 빌드해 OpenNext로 Cloudflare Workers에 배포

## Previous Projects

<details>
<summary><strong>Nexus | 온라인 포트폴리오 판매 플랫폼</strong> · 2025.06 ~ 2025.07 · 3인 팀 (팀장 · 백엔드)</summary>

[Repository](https://github.com/jhpark-coder/SpringBootProject_Group4)

- Spring Boot, Spring Security, React, NestJS, MySQL(MariaDB), Redis, Docker, AWS EC2·RDS
- 백엔드 API와 데이터베이스 설계, 시스템 아키텍처
- NestJS·Socket.IO 기반 실시간 채팅·알림 서버
- Tiptap 에디터 연동, 결제한 사용자만 보는 유료 콘텐츠 영역
- Docker·Git 환경 구축, AWS EC2 배포

</details>

<details>
<summary><strong>FitMate | 실시간 모션 인식 기반 맞춤 운동 추천</strong> · 2025.07 ~ 2025.09 · 개인</summary>

[Repository](https://github.com/jhpark-coder/personalproject)

- Spring Boot, React, NestJS, MySQL, MongoDB, Redis, Docker
- MediaPipe 포즈 인식으로 운동 자세를 분석하고, 브라우저 음성 합성(Web Speech API)으로 실시간 코칭
- OAuth 2.0 소셜 로그인, NestJS 통신 서버로 실시간 알림과 Twilio SMS 발송
- 사용자 상태를 반영한 운동 추천과 Recharts 데이터 시각화

</details>

<details>
<summary><strong>MineSweeper</strong> · 2025.05 ~ 2025.06 · 개인</summary>

[Repository](https://github.com/jhpark-coder/MineSweeper-Java)

- Java Swing, MySQL, HikariCP
- BFS 기반 지뢰 탐색과 파일·DB 랭킹 시스템
- MVC 구조와 FlatLaf 다중 테마 적용

</details>

## Education & Certification

### AI활용 풀스택 부트캠프 (프론트엔드·백엔드)

`2025.04 ~ 2025.10` · 인천더조은컴퓨터아트학원 · 6개월

- Java·Spring, Python, React, Flutter, 데이터베이스, Docker 기반 프로젝트 수행
- 개인 프로젝트 2회, 팀 프로젝트 1회 (팀장)
- **최우수상** 수상 (전 항목 평가 최우수 성적)

### 인하대학교 컴퓨터정보공학과

`2011.03 ~ 2017.02`

- 주요 과목: 자료구조, 알고리즘, 데이터베이스, 운영체제, 네트워크
- 졸업 프로젝트: 위치 기반 실시간 주유소 추천 앱

### 자격증

- `2019.05` 정보처리기사
- `2016.01` JLPT N1
