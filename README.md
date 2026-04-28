# lsy860224.github.io

GitHub Pages **user-level root** repo for `https://lsy860224.github.io`.

## 목적

이 저장소는 단 하나의 역할만 합니다 — **루트 도메인(`lsy860224.github.io`) 접속 시 GentleLab 시리즈 랜딩으로 자동 리다이렉트**.

GitHub Pages 사양상 `<username>.github.io/` 루트에서 페이지를 서비스하려면 같은 이름의 repo가 필요합니다. 이 repo가 없으면 루트는 404가 떠요. 외부 공유·SNS 프로필 링크 등에서 root URL을 자연스럽게 처리하기 위해 만들었습니다.

## 동작

- `index.html` — `<meta refresh>` + JS 양쪽으로 즉시 `/gentlelab.github.io/`로 이동
- `404.html` — 존재하지 않는 sub-path도 모두 GentleLab 메인으로 이동
- `<canonical>` 태그로 SEO는 GentleLab을 가리키고, `noindex,follow`로 검색 결과에 redirect 페이지 자체는 숨김

## 변경

GentleLab 도메인이 커스텀 도메인(예: `gentlelab.com`)으로 전환되면 `/gentlelab.github.io/`를 새 도메인으로 일괄 치환.

## 관련

- GentleLab 시리즈: https://lsy860224.github.io/gentlelab.github.io/
- 본인 프로필: https://github.com/lsy860224
