# 💥 오류
refusing to merge unrelated histories

# 🔎 테스트
1. push-test Repository 생성할 때, README 파일을 추가하지 않고 생성
2. IntelliJ 프로젝트 commit 및 push
3. README 파일 commit
4. IntelliJ에서 Main 클래스 수정 후 commit 및 push

# ❓ 원인
연동한 GitHub Repository의 README.md 파일을 커밋한 이력이 로컬 저장소의 커밋 이력에는 없어서 생긴 오류이다

# ⭕ 해결

### ✔ 방법 1
README 파일을 추가하지 않고 GitHub Repository 생성

### ✔ 방법 2
IntelliJ 터미널에서 아래 명령어 실행
- git pull --allow-unrelated-histories REMOTE BRANCH
- git pull --allow-unrelated-histories origin main
