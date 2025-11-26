# GitHub 연결 가이드

## ⚡️ 빠른 설정 (3단계)

### 1단계: GitHub에서 새 저장소 생성
1. https://github.com/new 접속
2. Repository name: `video-planning-system` 입력
3. **"Add a README file" 체크 해제** (중요!)
4. "Create repository" 클릭

### 2단계: 아래 명령어 실행

GitHub 저장소를 생성한 후, **YOUR_USERNAME을 본인의 GitHub 아이디로 변경**하고 실행:

```bash
cd /Users/mac/Documents/coding
git remote add origin https://github.com/YOUR_USERNAME/video-planning-system.git
git branch -M main
git push -u origin main
```

### 3단계: 확인

브라우저에서 `https://github.com/YOUR_USERNAME/video-planning-system` 접속하여 확인!

---

## 🔐 인증 방법

### Personal Access Token 사용 (추천)

GitHub는 이제 비밀번호 대신 Token을 사용합니다.

1. **Token 생성**
   - https://github.com/settings/tokens 접속
   - "Generate new token" → "Generate new token (classic)" 클릭
   - Note: `video-planning-push`
   - Expiration: `90 days` (또는 원하는 기간)
   - Scopes: ✅ **repo** 체크
   - "Generate token" 클릭
   - ⚠️ **토큰을 복사해서 안전한 곳에 저장** (다시 볼 수 없음!)

2. **Push 시 인증**
   ```bash
   git push -u origin main
   ```
   - Username: `YOUR_GITHUB_USERNAME`
   - Password: `복사한_Token_붙여넣기`

---

## 📝 이후 업데이트 방법

파일 수정 후 GitHub에 푸시:

```bash
cd /Users/mac/Documents/coding

# 변경 사항 확인
git status

# 변경된 파일 추가
git add video-planning-v2.html

# 커밋
git commit -m "Update: AI generation improvements"

# 푸시
git push
```

---

## 🌐 저장소 URL 예시

생성 후 접속할 URL:
```
https://github.com/YOUR_USERNAME/video-planning-system
```

README 파일이 자동으로 표시되어 프로젝트 설명을 볼 수 있습니다.

---

## ⚠️ 주의사항

1. **API 키 보안**
   - `.gitignore`에 API 키 파일이 포함되어 있는지 확인
   - HTML 파일에 API 키가 하드코딩되지 않았는지 확인
   - 사용자가 직접 입력하도록 설계되어 있어 안전함

2. **브랜치**
   - 메인 브랜치명: `main`

3. **이미 커밋된 파일들**
   - video-planning-v2.html (최신)
   - video-planning-complete-pro.html
   - 워크플로우 이전 버전들
   - README.md (프로젝트 문서)
   - .gitignore (불필요한 파일 제외)

---

**다음 단계**: 위의 명령어를 실행하여 GitHub에 푸시하세요! 🚀
