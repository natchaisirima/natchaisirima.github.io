# Portfolio — natchaisirima.github.io

Personal portfolio / CV site for Natchai Sirima (Environmental Manager · Environmental Engineer), published via **GitHub Pages** at https://natchaisirima.github.io.

## Structure

Plain static site — no build step, no dependencies:

- `index.html` — single-page CV: profile header, skills, project experience (NSCR-EX, Nam Theun 1, Bangkok–Nong Khai HSR, Yangon PPP, Turkey biogas), **AI & Digital Engineering** (AI-assisted development work), education, photo galleries with a lightbox
- `style.css` — all styling, including print and mobile breakpoints
- `img/` — photos; `avatar-web.jpg` is the downsized (256 px) copy served on the page, `avatar.jpg` is the full-resolution original
- `Natchai_Sirima_CV.pdf` — the short 1-page CV ("Download CV" button)
- `Natchai_Sirima_ITD_CV_ENG.pdf` / `Natchai_Sirima_ITD_CV_TH.pdf` — the full ITD-format CVs, English and Thai ("ITD CV (ENG)" / "ITD CV (TH)" buttons)

## Publish

Push to `main`; GitHub Pages serves the repo root:

```bash
git add -A && git commit -m "Update portfolio" && git push
```

## CV files — public vs private

The two ITD CVs served here are **public variants**: the personal-information block is
reduced to work email, mobile numbers, nationality, location and this site. The full ITD
CVs are kept outside this repo and are never published.

When a CV changes, edit the source document, export to PDF, and copy only the two
`ITD_CV_*` PDFs into this repo.

## Notes

- Gallery images use `loading="lazy"`; keep new photos web-sized (< ~250 KB) before adding.
- If you replace the avatar, regenerate the web copy: `sips -Z 256 -s formatOptions 85 img/avatar.jpg --out img/avatar-web.jpg`
