# lsy860224.github.io

GitHub Pages **user-level root** repo for `https://lsy860224.github.io`.

## ⚠️ Auto-generated content

이 repo의 파일들은 **`gentlelab-web` (Astro 소스 repo)에서 빌드된 결과물**입니다. 직접 편집하지 마세요.

- 소스 repo: https://github.com/lsy860224/gentlelab.github.io (`gentlelab-web` 로컬 폴더)
- 빌드 → 이 repo로 push → GitHub Pages가 root에서 서빙

## 배포 흐름 (현재 — manual)

```bash
cd ~/dev/gentlelab-web
PATH="$HOME/.nvm/versions/node/v22.22.2/bin:$PATH" npm run build
# 결과: dist/

cd ~/dev/lsy860224.github.io
rm -rf _astro en gentledo gentlefast gentlestudy images og privacy *.html *.svg *.xml *.txt
cp -R ~/dev/gentlelab-web/dist/. .
git add -A && git commit -m "deploy: gentlelab-web YYYY-MM-DD HH:mm" && git push
```

## 향후 자동화 (TODO)

`gentlelab-web` repo의 GitHub Actions에 cross-repo push 추가:
- PAT 또는 deploy key를 secret으로 등록
- workflow가 빌드 후 lsy860224.github.io repo에 push
- Pages가 자동 재배포

## 히스토리

- **2026-04-28 17:05** — 구조 전환: gentlelab-web 사이트가 `/gentlelab.github.io/` 서브패스에서 `/` 루트로 이동. 절대 경로 버그 (favicon·nav 깨짐) 해결.
- **2026-04-28 16:42** — 초기 redirect-only 셋업 (현재 폐기, 실제 사이트로 교체)

## 관련

- 본인 프로필: https://github.com/lsy860224
- Astro 소스: https://github.com/lsy860224/gentlelab.github.io
