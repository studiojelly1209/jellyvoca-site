# 젤리 영단어 — GitHub Pages

앱 소개 사이트 · 개인정보처리방침 · 사용자 메뉴얼

## 파일 구조

```
github-pages/
├── index.html    ← 메인 (앱 소개)
├── privacy.html  ← 개인정보처리방침
├── manual.html   ← 사용자 메뉴얼
├── style.css     ← 공통 스타일
└── README.md
```

## 배포 방법 (GitHub Pages)

1. 이 `github-pages/` 폴더 안의 파일들을 별도 저장소(예: `jellyvoca-site`)의 루트에 복사
2. GitHub → Settings → Pages → Source: `main` 브랜치 선택 → Save
3. 도메인 연결 시: Settings → Pages → Custom domain 입력 후 DNS CNAME 설정

## 수정이 필요한 항목

- `index.html`: Google Play 스토어 링크 (`https://play.google.com/store` → 실제 URL)
- `privacy.html`: 이메일 주소 (`support@jellyvoca.app` → 실제 이메일)
- `manual.html`: 이메일 주소 동일
- AdSense 적용 시: 각 HTML `<head>`에 AdSense 스크립트 추가

## AdSense 스크립트 추가 위치 (승인 후)

```html
<head>
  ...
  <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-XXXXXXXXXXXXXXXX"
     crossorigin="anonymous"></script>
</head>
```
