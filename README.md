# 박준호 | 제조 자동화 소프트웨어 풀스택 개발자

> 전기 설계 엑셀 자료를 도면으로 바꾸는 Windows 데스크톱 앱을 설계부터 설치본 배포까지 혼자 만들고 있습니다.

제조설비의 전기 설계(ECAD)와 PLC 데이터를 다루는 풀스택 개발자입니다.
설계자가 엑셀과 CAD를 오가며 손으로 하던 작업을 규칙으로 옮기고, 그 결과를 실제 도면과 대조해 검증하는 일을 합니다.

- 현재: **주식회사 제이엘티 기업부설연구소 팩토리AI팀 연구원** (2025.11 ~ 현재)
- 주요 분야: **전기 설계 자동화(ECAD) · PLC 구성 · 데스크톱 앱**
- 주로 쓰는 기술: **React · TypeScript · Electron · Python FastAPI · C#/.NET · SQLite**
- Contact: **pjh133765@gmail.com**

## Career

### 주식회사 제이엘티 · 기업부설연구소 팩토리AI팀

`2025.11 ~ 현재` · 연구원 · 풀스택 개발

레이저 비전(LVS), 폐배터리 리사이클링(BR), PLC, ECAD 등 제조설비 소프트웨어를 개발하는 기업입니다.

#### 전기 설계 자동화 데스크톱 앱 (사내 ECAD)

`Electron` `React 19` `TypeScript` `JointJS` `Python FastAPI` `SQLAlchemy` `SQLite` `C#/.NET` `SOLIDWORKS Electrical API`

제어반 설계자는 부품 목록(BOM)과 부하 계산표(LoadList)를 엑셀로 받아 단선도를 손으로 그리고, SOLIDWORKS Electrical에서 같은 도면을 다시 그립니다.
이 흐름을 **BOM 반입 → 부하 전기 계산 → 단선도 자동 구성 → SOLIDWORKS Electrical 도면·PDF 자동 생성**으로 잇는 Windows 데스크톱 앱입니다.

- 설계·구현·테스트·설치본 배포를 혼자 맡아 1년간 개발 진행
- Git Flow(`develop` 통합 검증 · `release/` 배포 · `hotfix/` 긴급 수정) 기반 브랜치·배포 절차 도입

**구조**

- Electron 셸이 로컬 FastAPI 백엔드를 띄우고, React 편집기와 SQLite 저장소를 연결하는 구조 설계
- C# 생성기가 SOLIDWORKS Electrical COM API로 심볼·매크로·와이어를 배치하고 PDF·프로젝트 아카이브 출력
- SWE 생성 시 템플릿·심볼 형상을 재사용하고 COM 중복 조회 제거
- PyInstaller·NSIS로 패키징해 사용자 PC에 Python·Node·Docker 없이 설치·실행
- 편집 중 문서는 IndexedDB에 자동 백업하고, 저장·반입·생성 요청은 프로젝트별 쓰기 큐로 순서 보장

**단선도 편집기**

- JointJS 기반 심볼 배치, 직교 와이어 경로와 이동 중 경로 미리보기, 구조상자, Undo/Redo
- 와이어 자동 우회 경로·심볼 배치 탐색 범위를 줄이고 선택 표시와 미니맵 갱신을 분리해 편집 반응성 개선

**엑셀 데이터 처리와 전기 계산**

- 부품 DB·BOM·부하 계산 등 6개 화면이 함께 쓰는 엑셀식 공통 표: 범위 선택, Excel과 복사·붙여넣기, 채우기, 정렬·필터, 실행 취소
- 시트·열·단위를 지정하는 LoadList 반입, 정격 전류·부하율·동시율 계산, 상분배, 차단기 용량 후보 선정과 근거 보존
- 제조사별 모델명 해석 규칙(LS·OMRON·미쓰비시·삼원ACT)으로 정격 사양을 추출하고 BOM 행을 부품 DB에 자동 매칭
- 판넬별 부하 역할과 보호 협조 규칙으로 단선도 회로 계층을 자동 구성
- 미쓰비시 PLC 베이스·슬롯 구성과 점별 IO를 단선도 장치와 연결

**검증**

- 자동 테스트 약 4,000건(백엔드 pytest 2,976건, 프런트 1,200여 건)과 백엔드 병렬 실행 도구
- 실제 설계 도면을 정답지로 삼아 자동 생성한 단선도를 계통 단위로 대조하는 회귀 테스트
- 생성 도면 검사 스크립트: 대각선 와이어, 접속점에 닿지 않는 끝, 의도하지 않은 T자 분기, 없는 심볼을 가리키는 와이어를 각각 0건으로 확인
- 배포본을 빈 사용자 프로필로 실행해 저장·재열기·생성 흐름 확인

> 회사 프로젝트의 소스 코드와 화면은 비공개라 링크를 넣지 않았습니다. 담당 업무와 기술 위주로 정리했습니다.

## Tech Stack

### Current

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Electron](https://img.shields.io/badge/Electron-47848F?style=flat-square&logo=electron&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![C#](https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

### Previously Used

![Java](https://img.shields.io/badge/Java-007396?style=flat-square)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

## Featured Projects

### AUTOMATA — PLC 현장 자동화 매뉴얼

[Repository](https://github.com/jhpark-coder/automata-plc-manual) · Next.js 16 · React 19 · Three.js

제조설비의 생김새, 역할, 태그, 동작 상태와 PLC 명령을 하나의 흐름으로 학습할 수 있는 한국어 인터랙티브 웹 매뉴얼입니다.

- 컨베이어, 실린더, 그리퍼, 센서, 산업용 로봇 등 장비 24종 수록
- 회전·확대 가능한 WebGL 3D 형상과 가동부 동작 시연
- 동작 순서에 따라 바뀌는 `LIVE STATE`와 PLC 명령 표시
- 동작 버튼 64개의 타이밍·상태·복귀 자세를 자동 검증하는 스크립트 구축
- Next.js 빌드와 Cloudflare 배포 패키징 지원

### Interior Simulator

[Repository](https://github.com/jhpark-coder/Interior-Simulator) · React 19 · TypeScript · Konva · React Three Fiber

방 구조와 가구를 2D에서 편집하고 같은 데이터를 3D 공간에서 확인하는 인테리어 배치 시뮬레이터입니다.

- React Konva 기반 2D 편집기와 React Three Fiber 기반 3D 장면 구현
- 가구·문·창문 배치, 그리드 스냅, 경계 및 가구 충돌 검사
- 문·창문 개폐와 수납장·서랍·모니터암 등 상호작용 가능한 3D 메시
- Zustand 단일 상태를 통한 2D·3D 동기화 및 Undo/Redo
- Zod 기반 JSON 저장·불러오기 검증과 자동 저장
- Vitest 기반 좌표·스냅·히스토리·스키마 단위 테스트

### DevMate

[Repository](https://github.com/jhpark-coder/devmate) · Python · Streamlit · LangChain · FAISS · Ollama

방대한 기술 문서를 한국어 질의응답으로 탐색하는 RAG 기반 공식 문서 도우미입니다. API 키 없이 로컬에서만 동작합니다.

- 22개 기술·140개 문서를 청킹해 로컬 다국어 임베딩(bge-m3)으로 FAISS 벡터 인덱싱
- 한국어 질문으로 영어 원문을 검색하고, 유사도·원문 미리보기를 포함한 출처 표시
- LLM과 임베딩을 모두 로컬 Ollama로 실행하는 LLM 추상화 (설치된 모델을 UI에서 선택)
- Domain·Application·Infrastructure 계층으로 문서 처리와 검색 책임 분리
- Streamlit 기반 대화형 검색 UI와 단위·통합·E2E 테스트 구성

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

### AI활용 풀스택 부트캠프 (프론트엔드·백엔드)

`2025.04 ~ 2025.10` · 인천더조은컴퓨터아트학원 · 6개월

- Java·Spring, Python, React, Flutter, 데이터베이스, Docker 기반 프로젝트 수행
- 개인 프로젝트 2회, 팀 프로젝트 1회
- **최우수상** 수상 (전 항목 평가 최우수 성적)

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
