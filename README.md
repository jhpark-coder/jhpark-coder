# 박준호 | Industrial Automation & AI Full-Stack Developer

> 제조 자동화 도메인에서 C# 데스크톱 클라이언트부터 React·FastAPI 기반 AI/PLC 파이프라인까지 개발합니다.

안녕하세요. 전자회로도(ECAD), PLC, 제조설비 데이터를 다루는 개발자 박준호입니다.
기존 산업용 클라이언트를 현대화하고, 현장 데이터를 AI가 처리할 수 있는 구조로 연결하는 일에 관심이 있습니다.

- 현재: **주식회사 제이엘티 기업부설연구소 팩토리AI팀 연구원**
- 역할: **클라이언트(프론트엔드) 개발자 → AI 풀스택 개발자**
- 주요 분야: **ECAD · PLC · 제조설비 데이터 · 로컬 LLM**
- 근무 지역: **인천**
- Contact: **pjh133765@gmail.com**

## Career

### 주식회사 제이엘티

`2025.11 ~ 현재` · 기업부설연구소 팩토리AI팀 · 연구원/팀원

레이저 비전(LVS), 폐배터리 리사이클링(BR), PLC, ECAD 등 제조설비 관련 소프트웨어를 개발하는 기업입니다.

- 직무: 클라이언트(프론트엔드) 개발, AI 풀스택 개발
- 기업 정보: 매출 94억 원 · 직원 75명

#### C#/.NET ECAD 클라이언트 개발

`2025.11 ~ 2026.07`

**C# · .NET 8 · Avalonia · SQLite · EF Core · MVVM · Git Flow**

- 기존 WinForms 클라이언트 기능을 Avalonia 기반 데스크톱 클라이언트로 마이그레이션
- Application·Domain·Infrastructure·Presentation 경계를 중심으로 클라이언트 구조 개선
- 의존성 주입, MVVM 및 Git Flow 기반 협업·배포 흐름 도입
- SQLite와 EF Core를 활용한 심볼·매크로·설정 데이터 관리
- 전자회로도 편집기, 심볼/매크로, 와이어 라우팅, 프로젝트 저장·복구 기능 개발
- Excel LoadList 변환과 SWE 프로젝트 데이터 가져오기·검증 기능 개발
- 대규모 도면 렌더링 및 편집 반응성 개선, 회귀 테스트와 설치본 검증 자동화

#### AI 기반 PLC 코드 자동 생성 프로젝트

`2026.08 ~ 현재`

**React · TypeScript · Python · FastAPI · Pydantic · Local LLM · PLC ST**

- React·TypeScript 프론트엔드와 Python FastAPI 백엔드 기반 MCC Import 기능 담당
- 제조설비 공정 Excel(`.xlsm`) 파싱 및 공정 스텝 데이터 추출 구조 분석
- 공정 자연어 정형화와 로컬 LLM 기반 PLC 제어 시퀀스 생성 파이프라인 분석
- EM·CM 장비 정보와 MCC 공정 데이터 간 매핑 및 식별자 생성 구조 분석
- 생성된 IEC 61131-3 Structured Text를 PLC Payload와 Flow 데이터로 변환하는 과정 분석
- 프론트엔드·FastAPI·호스트 프로그램 간 연동 인터페이스와 데이터 계약 문서화
- 컨베이어·스토퍼·그리퍼 등 설비 동작 인식 개선을 위한 모델 추가 학습 및 평가 담당

> 회사 프로젝트의 소스 코드는 비공개이며, 위 내용은 담당 업무와 사용 기술을 중심으로 정리했습니다.

## Tech Stack

### Current

![C#](https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![.NET](https://img.shields.io/badge/.NET_8-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![Avalonia](https://img.shields.io/badge/Avalonia-8B44AC?style=flat-square)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

### Previously Used

![Java](https://img.shields.io/badge/Java-007396?style=flat-square)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

## Featured Project

### AI Research Note Writer

[Repository](https://github.com/jhpark-coder/AIResearchNoteWriter) · Windows · C# · .NET 10 · WPF

Codex와 Claude Code의 개발 대화를 프로젝트·날짜별 작업 근거로 정리하고, 실제 Word 연구일지에서 미작성 날짜를 찾는 Windows 프로그램입니다.

- Codex·Claude Code 로컬 세션 수집과 프로젝트/날짜 필터
- 사용자 요청, AI 요약, 빌드·테스트 결과 선별
- 민감 정보 마스킹과 근거 포함·제외 검토
- Word 연구일지 읽기 전용 미작성 날짜 검사
- Windows x64 설치형 EXE와 포터블 ZIP 배포

## Previous Projects

<details>
<summary><strong>FitMate | 실시간 모션 인식 기반 맞춤 운동 추천</strong></summary>

`2025.07 ~ 2025.09` · 개인 프로젝트
[Repository](https://github.com/jhpark-coder/personalproject)

- Spring, React, NestJS, MySQL, Redis, Docker
- MediaPipe 모션 인식과 Google Cloud TTS 기반 운동 지원
- 사용자 상태를 반영한 운동 추천 및 데이터 시각화

</details>

<details>
<summary><strong>Online Portfolio Platform</strong></summary>

`2025.06 ~ 2025.07` · 3인 팀 프로젝트
[Repository](https://github.com/jhpark-coder/SpringBootProject_Group4)

- Spring Boot, React, NestJS, MySQL, Redis, Docker
- 백엔드 API와 데이터베이스 설계
- Tiptap 판매글 CRUD, Socket.IO 알림·채팅 기능

</details>

<details>
<summary><strong>MineSweeper</strong></summary>

`2025.05 ~ 2025.06` · 개인 프로젝트
[Repository](https://github.com/jhpark-coder/MineSweeper-Java)

- Java Swing, MySQL, HikariCP
- BFS 기반 지뢰 탐색과 파일·DB 랭킹 시스템
- MVC 구조와 FlatLaf 다중 테마 적용

</details>

## Education & Certification

### 인하대학교 컴퓨터공학과

`2011.03 ~ 2017.02`

- 주요 과목: 자료구조, 알고리즘, 데이터베이스, 운영체제, 네트워크
- 졸업 프로젝트: 위치 기반 실시간 주유소 추천 앱

### Java 풀스택 개발자 과정

`2025.04 ~ 2025.10`

- Java·Spring, React, 데이터베이스, Docker 기반 프로젝트 수행
- 개인 프로젝트 2회, 팀 프로젝트 1회
- 교육 과정 최우수상

### 자격증

- `2016.01` JLPT N1
- `2019.05` 정보처리기사

## GitHub

<div align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=jhpark-coder&show_icons=true&theme=tokyonight)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=jhpark-coder&layout=compact&theme=tokyonight)

</div>

## Contact

[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:pjh133765@gmail.com)
[![Tistory](https://img.shields.io/badge/Tistory-000000?style=flat-square&logo=tistory&logoColor=white)](https://primotion.tistory.com/)
