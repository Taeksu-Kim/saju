# 사주 분석 웹 서비스

paperclip을 이용한 사주 분석 웹 사이트 생성 프로젝트

## 기술 스택

- **Backend**: FastAPI (Python 3.11+)
- **Frontend**: React 18 + TypeScript (Vite)
- **Database**: PostgreSQL
- **AI**: Claude API (Anthropic)

## 로컬 개발 환경

### 백엔드

```bash
# 가상환경 생성 (WSL2 네이티브 경로 권장 — /mnt/d/ 보다 7배 빠름)
python3 -m venv ~/.cache/saju/venv
ln -s ~/.cache/saju/venv backend/.venv

# 패키지 설치
backend/.venv/bin/pip install -r backend/requirements.txt

# 서버 실행
backend/.venv/bin/uvicorn app.main:app --app-dir backend --reload --port 8000
```

### 프론트엔드

```bash
cd frontend
npm install
npm run dev   # http://localhost:5173
```

### API 문서

서버 실행 후 → http://localhost:8000/docs
