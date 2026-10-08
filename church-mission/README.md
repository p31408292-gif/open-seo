# 인천제2교회 세계선교 페이지

빌드 없이 동작하는 정적 페이지입니다. `index.html`을 브라우저로 열거나, 폴더 전체를 아무 정적 호스팅(GitHub Pages, Netlify, Cloudflare Pages, 교회 서버)에 올리면 됩니다.

- 선교사 추가/변경: `index.html`의 `FIELDS`(선교지 좌표)와 `MISSIONARIES`(선교사 목록)만 수정합니다.
- 보안 지역(C국·H국 등)은 지도에 표시하지 않고 `secure: true`로 표기합니다. 이름 가림은 `MASK_SECURE_NAMES`로 끄고 켭니다.
- `vendor/`에는 d3 7.9.0, topojson-client 3.1.0, world-atlas 2.0.2(110m)가 포함되어 있어 외부 CDN 없이 동작합니다. 웹폰트만 Google Fonts에서 불러옵니다.
