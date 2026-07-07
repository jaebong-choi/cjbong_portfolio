# 최재봉 포트폴리오 — 유학 컨설팅 × AI 콘텐츠

유학 상담 17년 경력의 상담가가 만드는 AI 콘텐츠 포트폴리오 사이트입니다.
랜딩페이지 · 영상(숏폼/롱폼) · 카드뉴스 · AI 상담 툴 제작 사례를 한 페이지에 정리했습니다.

Claude Design에서 만든 프로토타입(`Portfolio.dc.html`)을 자체 완결형 정적 사이트로 재구성한 것입니다.

## 구성

- `index.html` — 사이트 전체 (HTML/CSS/JS 단일 파일, 빌드 불필요)
- `assets/` — 프로필/로고 이미지, 작업 썸네일(`assets/slots/`)

정적 사이트라 별도 빌드 과정이 없습니다. 어떤 정적 호스팅(Vercel, Netlify, GitHub Pages)에도 그대로 올라갑니다.

## 로컬 미리보기

```powershell
powershell -ExecutionPolicy Bypass -File serve-static.ps1 -Port 4321
# http://localhost:4321 접속
```

## 배포 (Vercel)

Vercel 대시보드에서 이 GitHub 저장소를 Import 하면 됩니다.
빌드 설정 없이 "Other / static" 그대로 배포되며, 이후 `main` 브랜치에 push할 때마다 자동 재배포됩니다.
