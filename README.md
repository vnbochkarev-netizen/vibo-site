# vibo-site

Production build of the ViBo website, served by GitHub Pages at https://wwwvibo.com.

Source lives in `vibo-web` (React 19 + Vite). This repository holds only the
compiled output: what is committed here is what is deployed.

## Pages

- `/` — platform and skills
- `/product` — agent-skill architecture
- `/benchmarks` — measured efficiency
- `/security` — private execution
- `/pricing` — plans and access

`404.html` is a copy of `index.html` so client-side routes resolve on a static host.

## Updating

```bash
# in vibo-web
pnpm --filter client build
rsync -a --delete apps/client/dist/ ../vibo-site/   # keep CNAME
cp ../vibo-site/index.html ../vibo-site/404.html
```

Then commit and push — Pages picks it up on the next build.
