# 전혜영 · 챗GPT·생성형 AI 교육 전문가 소개 사이트

강사 브랜딩용 원페이지 웹사이트입니다. 빌드 도구 없이 HTML/CSS/JS만으로 동작합니다.

**배포 주소:** https://nanicca.github.io

## 파일 구조

```
index.html        전체 페이지 (구조·스타일·스크립트 포함)
assets/data.js    출강 이력 데이터 (73건)
assets/profile.jpg 프로필 사진
.nojekyll         GitHub Pages가 Jekyll 처리를 건너뛰도록 하는 표시 파일
```

## 내용 수정 방법

- **출강 이력 추가** → `assets/data.js` 의 배열에 항목을 하나 추가합니다.
  ```js
  {"p":"2026.10","y":"2026","o":"기관명","t":"과정명","a":"교육대상","s":false,"c":"public"}
  ```
  - `p` 기간 · `y` 연도 · `o` 기관 · `t` 주제 · `a` 대상 · `s` 교육지원 여부
  - `c` 분류: `public`(공공·행정) / `corp`(기업) / `edu`(대학·학교) / `org`(협회·센터)
  - 상단 통계 숫자(73회·69곳)는 `index.html` 의 `.stats` 영역에서 직접 수정합니다.

- **경력·자격·문의처 수정** → `index.html` 안의 해당 섹션을 수정합니다.

## 로컬에서 확인

```
python -m http.server 8777
```
브라우저에서 http://127.0.0.1:8777 접속.

## 수정 사항 반영 (배포)

```
git add .
git commit -m "내용 수정"
git push
```
푸시 후 1~2분 내 https://nanicca.github.io 에 반영됩니다.
