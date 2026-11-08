# Saisumanth Orupula – Portfolio

Personal portfolio website of **Saisumanth Orupula**, DevOps & Playwright Automation Engineer.

**Live site:** https://saisumanthorupula.github.io/portfolio/

## Sections

| Section | What it shows |
|---|---|
| Home | Auto-scrolling hero slider (photo + Accenture) with dot indicators |
| About me | Short introduction and career focus |
| Skills | Playwright, TypeScript, Cucumber, Azure DevOps, GitHub Actions, Docker |
| Experience | Automation Engineer at Accenture (May 2024 – Present) |
| Contact | Google Form plus Email, LinkedIn, GitHub, Facebook and Instagram links |

## Tech

Plain **HTML, CSS and a little JavaScript**. There is no build step, framework or package manager.
Icons come from Font Awesome 4.7 (CDN). It is hosted on **GitHub Pages**.

## Project structure

```
Portfolio/
├── index.html      # page content and slider/menu scripts
├── style.css       # all styling (responsive, mobile-first breakpoints)
├── images/         # photos and logos used by the site
├── .gitignore      # keeps private images out of the repo
└── README.md
```

## Run locally

Open `index.html` in a browser, or use the VS Code **Live Server** extension.
The Google contact form only loads fully when the page is served over the web.

## What changed in Version-2 (compared to Version-1)

### Fixed
- **Skills section:** removed the stray `6` and made every label match its bar (Playwright 95%, TypeScript 80%, Cucumber 85%, Azure DevOps 90%, GitHub Actions 90%, Docker 60%). Docker previously showed 90% on a 60% bar.
- **Broken or outdated items:** removed the "Corona Virus 2020" footer link, the broken `javascript:vo id(0)` link and the dead "Works" nav link, and fixed typos (`w3-conatainer`, "Iam", "compluted").
- **Markup:** `<meta charset>` is now inside `<head>`, and the page uses semantic tags (`<main>`, `<section>`, `<footer>`).
- **Cleanup:** removed large blocks of commented-out code.

### Responsive design
- Rebuilt the layout with plain CSS, so the page works on phones, tablets and desktop.
- Replaced the old nav with a hamburger menu on small screens that closes after you tap a link.
- Sections stack into one column below 768px, with no horizontal scrolling.

### New features
- **Experience section** with the Accenture role, dates, 400+ automated test cases and a logo badge.
- **Hero slider:** the photo and an Accenture image crossfade automatically in a loop. Dot indicators below the images are clickable, and you can swipe on touch screens. It pauses on hover and when the tab is hidden.
- **Hero animation:** gentle fade-in and slow zoom on the images.
- **Visitor counter** badge, centred in the footer.
- **Right-click message:** shows "Right click was disabled by Sumanth." (This does not truly protect images.)
- **About me:** now text only, with a centred role line and a readable single column. The old photo was removed.

### Performance, SEO and housekeeping
- Dropped Bootstrap 3, W3.CSS, jQuery and Material Icons. Only Font Awesome is still loaded.
- Removed 4 unused image files (`ffb.jfif`, `in.jfif`, `github.png`, `linkedin.png`) and moved the rest into `images/`.
- Added page title, meta description, Open Graph tags, image `alt` text and `loading="lazy"` on lower images.
- Added `rel="noopener noreferrer"` to external links.
- Removed the phone number from the page for privacy.
- Added a `.gitignore` (private image `about.jpeg`, `originals/`, OS and editor files).
- Added this README.
- Respects the "reduce motion" setting: animations and auto-scroll are turned off for those visitors.

### At a glance

| | Version-1 | Version-2 |
|---|---|---|
| Layout | W3.CSS + Bootstrap 3, partly responsive | Plain CSS, fully responsive |
| Libraries | W3.CSS, Bootstrap, jQuery, Font Awesome, Material Icons | Font Awesome only |
| Hero | Single static photo | Auto-scrolling slider with indicators |
| Experience | None | Accenture timeline card |
| Images | Loose files in the root | Organised in `images/` |
| Visitor counter | Third-party script and Corona link | Simple footer badge |
| Skills bars | Mismatched labels and a stray `6` | Accurate and consistent |

## Contact

- Email: saisumanthorupula@gmail.com
- LinkedIn: https://www.linkedin.com/in/saisumanthorupula/
- GitHub: https://github.com/sumanth83
