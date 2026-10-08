# Chidera Ikenna-Obi: portfolio

A single-page portfolio presenting Chidera Ikenna-Obi as a project lead / product owner for digital products. It's aimed at UK PMO Analyst, Project Analyst, IT/Digital Project Coordinator, Graduate PM and Business Analyst roles.

- Plain semantic HTML and CSS. No JavaScript, no build step, no frameworks.
- No cookies, analytics, tracking or external requests (system fonts only; all images are local).
- Responsive (tested at 1440 px and 390 px) and accessible (axe-core: 0 WCAG 2.1 AA violations at both widths).

## Structure

```
index.html                        the whole site
assets/css/styles.css             styles
assets/img/*.webp                 screenshots of the live apps (taken 8 Oct 2026)
assets/Chidera_Ikenna-Obi_CV.pdf  downloadable CV (web copy of the master CV: no phone number or postcode)
assets/favicon.svg
```

Case-study statements that are inferences rather than verified facts are marked with HTML comments (`<!-- C01 -->` … `<!-- C23 -->`). They're explained in `../CLAIMS_TO_CONFIRM.md`.

## Run locally

Any static file server works. For example:

```bash
cd chideraportfolio
python3 -m http.server 4321
# open http://localhost:4321
```

or `npx serve .`

## Deploy (when ready)

The site is static and works on Vercel with zero configuration: import the folder or repo, set Framework Preset to **Other**, and leave the build command empty. The output directory is the project root. Netlify or GitHub Pages also work.

> Live at https://chideraikennaobi.vercel.app (Vercel auto-deploys from main).

## Updating

- **CV:** replace `assets/Chidera_Ikenna-Obi_CV.pdf` (keep the file name, or update both links in `index.html`). Use a web copy with the phone number and postcode removed. The public contact details are email and "Hartlepool" only.
- **App screenshots:** replace the matching file in `assets/img/` (960×600 WebP).
- **Case studies:** each one is an `<article class="case">` in `index.html` with eight `<section class="case-sec">` blocks.
