# 영상 기획안 제작 시스템

영화/애니메이션 제작을 위한 체계적인 기획안 작성 도구입니다.

## 주요 기능

### 🎬 Module 1 — 스토리
- **1단계**: 제작 형식 선택 (영화/애니메이션/드라마 등)
- **2단계**: 줄거리 및 세계관 작성 (AI 자동 생성 지원)

### 👥 Module 2 — 캐릭터
- **3단계**: 캐릭터 설정 (메인/서브 캐릭터, AI 자동 생성)

### 📝 Module 3 — 시나리오
- **4단계**: 5막 구조 시나리오 작성 (AI 지원)
- **5단계**: 톤 & 무드 설정
- **6단계**: 장면별 상세 기획

### 🎨 Module 4 — 제작
- **7단계**: 배경 설정
- **8단계**: 장면별 톤 매칭
- **9단계**: 최종 기획 문서 작성 (AI 통합 생성)

## 🤖 AI 기능 (Gemini API)

### 지원되는 생성 기능
- 줄거리 자동 생성
- 세계관 구축
- 캐릭터 자동 생성 (외모, 성격, 배경 등)
- 5막 구조 시나리오 작성
- 종합 기획 문서 생성

### API 설정
1. [Google AI Studio](https://aistudio.google.com/app/apikey)에서 API 키 발급
2. 좌측 사이드바에 API 키 입력
3. "API 키 테스트" 버튼으로 연결 확인

### 사용 모델
- **gemini-1.5-flash** (1순위): 빠르고 안정적
- **gemini-1.5-pro** (2순위): 고성능
- **gemini-pro** (3순위): 기본 모델

자동 폴백 시스템으로 사용 가능한 모델을 자동 선택합니다.

## 📁 파일 구조

### 최신 버전
- **video-planning-v2.html**: Gemini API 통합 최신 버전 (v1 API, 자동 모델 선택)

### 이전 버전
- `video-planning-complete-pro.html`: PRO 버전
- `video-planning-workflow-complete.html`: 워크플로우 완성 버전
- `video-planning-workflow-module4.html`: Module 4까지 구현
- `video-planning-workflow-module3.html`: Module 3까지 구현
- `video-planning-workflow-v2.html`: 초기 워크플로우
- `video-planning-workflow.html`: 최초 버전

## 🚀 사용 방법

1. `video-planning-v2.html` 파일을 브라우저에서 열기
2. Gemini API 키 입력 (선택사항, AI 기능 사용 시 필요)
3. 좌측 사이드바에서 단계별로 진행
4. 각 단계에서 AI 자동 생성 버튼 활용
5. 모든 단계 완료 후 9단계에서 최종 기획안 생성

## 💾 데이터 저장

- 모든 입력 데이터는 브라우저의 `localStorage`에 자동 저장
- API 키도 로컬에만 저장 (서버 전송 없음)
- 진행 상황 자동 저장 및 복원

## 🔧 기술 스택

- Pure HTML/CSS/JavaScript
- Google Gemini API (v1)
- LocalStorage API
- Fetch API

## 📝 라이선스

개인 및 상업적 사용 가능

---

**마지막 업데이트**: 2025-11-26
**API 버전**: v1 (안정 버전)
