# 인천제2교회 세계선교 페이지

빌드 없이 동작하는 정적 페이지입니다. `index.html`을 브라우저로 열거나, 폴더 전체를 아무 정적 호스팅(GitHub Pages, Netlify, Cloudflare Pages, 교회 서버)에 올리면 됩니다.

- 선교사 추가/변경: `index.html`의 `FIELDS`(선교지 좌표)와 `MISSIONARIES`(선교사 목록)만 수정합니다.
- 보안 지역(C국·H국 등)은 지도에 표시하지 않고 `secure: true`로 표기합니다. 이름 가림은 `MASK_SECURE_NAMES`로 끄고 켭니다.
- `vendor/`에는 d3 7.9.0, topojson-client 3.1.0, world-atlas 2.0.2(110m)가 포함되어 있어 외부 CDN 없이 동작합니다. 웹폰트만 Google Fonts에서 불러옵니다.

## 선교 편지 올리기

`letters.js`에 편지를 한 통씩 추가합니다. 파일 맨 위 주석에 적는 방법이 있습니다.

- `missionary`는 `index.html`의 선교사 이름과 똑같이 적어야 선교지·파송/협력 구분이 자동으로 붙습니다.
- 사진은 `letters/photos/`, 원본 PDF는 `letters/` 폴더에 넣고 경로를 적습니다.
- 보안 지역 선교사님 편지는 본문·사진에 실명, 도시, 현지인, 단체명이 드러나지 않는지 확인한 뒤 올립니다. 이름 가림은 자동이지만 본문은 그대로 공개됩니다.
- `sample: true`가 붙은 두 통은 예시이므로 실제 편지를 넣으면 지웁니다.
- 특정 편지로 바로 가는 주소: `index.html#letter-2026-09-20-1` (날짜-그날의 순번)
