# Portfolio — natchaisirima.github.io

Personal portfolio / CV site for Natchai Sirima (Environmental Manager · Environmental Engineer), published via **GitHub Pages** at https://natchaisirima.github.io.

## Structure

Plain static site — no build step, no dependencies:

- `index.html` — single-page CV: profile header, skills, project experience (NSCR-EX, Nam Theun 1, Bangkok–Nong Khai HSR, Yangon PPP, Turkey biogas), education, photo galleries with a lightbox
- `style.css` — all styling, including print and mobile breakpoints
- `img/` — photos; `avatar-web.jpg` is the downsized (256 px) copy served on the page, `avatar.jpg` is the full-resolution original
- `Natchai_Sirima_CV.pdf` — downloadable CV linked from the header

## Publish

Push to `main`; GitHub Pages serves the repo root:

```bash
git add -A && git commit -m "Update portfolio" && git push
```

## Notes

- Gallery images use `loading="lazy"`; keep new photos web-sized (< ~250 KB) before adding.
- If you replace the avatar, regenerate the web copy: `sips -Z 256 -s formatOptions 85 img/avatar.jpg --out img/avatar-web.jpg`
