# MYK Korea Tours — Website

MYK 관광 가이드(가이드: Marcos Lee) 홈페이지입니다. 외국인 여행자를 위한 영어 홈페이지이며,
GetYourGuide · Klook · Viator에 등록된 실제 투어 상품으로 연결됩니다.

This is the homepage for **MYK Korea Tours**, a private English-speaking tour guide
service in Korea run by licensed local guide **Marcos Lee**. It links to real,
bookable tours on GetYourGuide, Klook, and Viator.

## 파일 구성 / Files

- `index.html` — 홈페이지 전체 (HTML + CSS + JavaScript가 한 파일에 다 들어 있어요)
  The entire website — a single self-contained file. All styles, scripts, and
  content live here, so editing this one file changes the whole site.

## 어떻게 수정하나요 / How to edit

이 사이트는 파일 하나로 되어 있어서, `index.html`만 고치면 됩니다. Cursor에서 열고
자연어로 요청하면 돼요. 예: "히어로 제목을 ○○로 바꿔줘", "투어 카드 하나 추가해줘".

Everything is in `index.html`. Open it in Cursor and ask in plain language, e.g.
"change the hero headline to X" or "add a new tour card for Y".

## 게시 / Deployment

정적 사이트라 빌드가 필요 없습니다. 두 가지 방법 중 하나로 게시하세요.
Static site — no build step. Deploy either way:

### GitHub Pages (GitHub만으로)
1. 저장소를 GitHub에 올립니다 (Cursor의 "Publish to GitHub").
2. GitHub 저장소 → **Settings → Pages** → Source: *Deploy from a branch* →
   Branch: `main`, folder: `/ (root)` → **Save**.
3. 1분쯤 뒤 `https://<username>.github.io/<repo-name>/` 에서 열립니다.
   무료 GitHub Pages는 저장소가 **Public**이어야 합니다.
   (`.nojekyll` 파일이 포함되어 있어 Jekyll 처리 없이 그대로 서빙됩니다.)

### Netlify (대안)
- GitHub 저장소를 연결. Build command: (none), Publish directory: `.`

## 게시 후 할 일 / After going live

`index.html` 안의 임시 주소 `https://www.myktour.com/` 를 실제 게시 주소로 바꿔주세요.
검색엔진(SEO)과 소셜 공유 미리보기가 올바르게 동작하려면 필요합니다. 위치:
`<link rel="canonical">`, Open Graph `og:url` / `og:image`, Twitter 태그,
그리고 하단의 JSON-LD 구조화 데이터.

Replace the placeholder domain `https://www.myktour.com/` in `index.html` with your
real published URL (canonical link, Open Graph tags, Twitter tags, and the JSON-LD
structured data block).

## 아직 채워야 할 항목 / Still to fill in

- 가이드 프로필 사진 & 투어 사진 (현재 자리표시자) / guide photo & tour photos
- 연락처: 이메일, 카카오톡/왓츠앱, 인스타그램 / contact details
- 소개 문구의 경력 연차 `[X]` / years of experience in the About section
- 소셜 공유용 대표 이미지 `og-image.jpg` / social preview image
