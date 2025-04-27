# 북엔드 바탕

[배포처 바로가기](https://www.bookend.tech/font)

&nbsp;

## 웹 폰트

사용하는 `font-family`의 이름은 `Bookend Batang`입니다.

### HTML

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/fonts-archive/BookendBatang/BookendBatang.css" type="text/css"/>
```

### CSS `@Import`

```css
@import url('https://cdn.jsdelivr.net/gh/fonts-archive/BookendBatang/BookendBatang.css');
```

### CSS `@font-face`

```css
@font-face {
  font-family: 'Bookend Batang';
  font-weight: 400;
  font-style: normal;
  font-display: swap;
  src: url('https://cdn.jsdelivr.net/gh/fonts-archive/BookendBatang/BookendBatang-Regular.woff2') format('woff2'),
      url('https://cdn.jsdelivr.net/gh/fonts-archive/BookendBatang/BookendBatang-Regular.woff') format('woff'),
      url('https://cdn.jsdelivr.net/gh/fonts-archive/BookendBatang/BookendBatang-Regular.otf') format('opentype'),
      url('https://cdn.jsdelivr.net/gh/fonts-archive/BookendBatang/BookendBatang-Regular.ttf') format('truetype');
}
@font-face {
  font-family: 'Bookend Batang';
  font-weight: 600;
  font-style: normal;
  font-display: swap;
  src: url('https://cdn.jsdelivr.net/gh/fonts-archive/BookendBatang/BookendBatang-SemiBold.woff2') format('woff2'),
      url('https://cdn.jsdelivr.net/gh/fonts-archive/BookendBatang/BookendBatang-SemiBold.woff') format('woff'),
      url('https://cdn.jsdelivr.net/gh/fonts-archive/BookendBatang/BookendBatang-SemiBold.otf') format('opentype'),
      url('https://cdn.jsdelivr.net/gh/fonts-archive/BookendBatang/BookendBatang-SemiBold.ttf') format('truetype');
}
```

&nbsp;

## 다이나믹 서브셋

웹폰트의 최적화를 위해 모던 브라우저에서는 글리프를 여러개로 나누어 필요한 부분만 동적으로 파싱하는 다이나믹 서브셋을 제공합니다. 폰트의 용량이 부담된다면 아래 코드를 사용하는 걸 추천합니다.

### HTML

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/fonts-archive/BookendBatang/subsets/BookendBatang-dynamic-subset.css" type="text/css"/>
```

### CSS

```css
@import url("https://cdn.jsdelivr.net/gh/fonts-archive/BookendBatang/subsets/BookendBatang-dynamic-subset.css");
```

&nbsp;

## font-family

어느 브라우저나 시스템 환경에서도 동일한 폰트가 적용되어야 한다면 아래와 같이 구성하는 걸 추천합니다. `-apple-system`과 `BlinkMacSystemFont`는 맥, `Segoe UI`는 윈도우, `Roboto`는 안드로이드의 기본 폰트입니다.

```css
font-family: "Bookend Batang", -apple-system, BlinkMacSystemFont, "Segoe UI",Roboto, Oxygen, Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
```

&nbsp;

## 라이선스

라이선스는 언제든지 변경될 수 있습니다. 변경사항을 확인하려면 배포처를 방문해 주세요.

```
SIL 오픈 폰트 라이선스

북엔드 바탕 서체의 지적 재산권은 (주)북엔드에 있습니다. 북엔드 바탕 서체는 개인 및 기업 사용자를 포함한 모든 사용자에게 무료로 제공되며 자유롭게 사용할 수 있고 상업적 이용이 가능합니다.

ⓘ 주의 : 본 서체는 글꼴 자체를 유료로 판매하거나 왜곡 변형할 수 없습니다

사용 가능 범위
인쇄 브로슈어, 포스터, 책, 잡지 및 출판용 인쇄물 등
웹사이트 웹페이지, 광고 배너, 메일, E-브로슈어 등
영상 영상물 자막, 영화 오프닝/엔딩 크레딧, UCC 등
포장지 판매용 상품의 패키지
임베딩 웹사이트 및 프로그램 서버 내 폰트 탑재, E-book 제작
BI/CI 회사명, 브랜드명, 상품명, 로고, 마크, 슬로건, 캐치프레이즈
OFL 폰트 파일의 수정/ 복제/ 배포 가능. 단, 폰트 파일의 유료 판매는 금지
```
