# Negotiating Style Assessment

> A free, research-based, browser-only assessment that maps your personal negotiating style across the **Thomas-Kilmann Conflict Mode Instrument (TKI)** and Professor **G. Richard Shell's** Wharton evaluation grid. 30 forced-choice questions, ~5 minutes, printable PDF report.

**Author:** [Abdel-Karim Al-Tamimi](https://www.linkedin.com/in/abdelkarim-altamimi) — University Professor
**Live demo:** https://negotiating-style-assessment.netlify.app/
**License:** Proprietary — All rights reserved © 2026

---

## Table of contents

- [About](#about)
- [Why this exists](#why-this-exists)
- [Frameworks](#frameworks)
- [Features](#features)
- [Screenshots](#screenshots)
- [Quick start](#quick-start)
- [Deployment](#deployment)
- [Project structure](#project-structure)
- [Use in the classroom](#use-in-the-classroom)
- [Privacy](#privacy)
- [Citation](#citation)
- [License](#license)
- [Contact](#contact)

---

## About

The **Negotiating Style Assessment** is a single-page web application that delivers a thirty-item forced-choice questionnaire and produces a personal profile across five canonical conflict-handling modes: **Competing, Collaborating, Compromising, Avoiding, and Accommodating**. Results are visualised on the two-dimensional Wharton/Shell grid (concern for self vs. concern for the other party), accompanied by an interpretive debrief and a downloadable PDF report.

Everything runs locally in the browser. No accounts, no tracking, no server.

## Why this exists

I built this for one of my university courses to give students a quick, research-grounded mirror on how they show up at the bargaining table — before we get into theory, role-plays, and case work. It's open to anyone (educators, managers, founders, lawyers, consultants, students) who wants a fast self-assessment built on respected frameworks rather than pop-psychology shortcuts.

## Frameworks

This instrument is informed by — and pays explicit credit to — two foundational works in negotiation and conflict scholarship:

| Framework | Authors | Source |
|---|---|---|
| **Thomas-Kilmann Conflict Mode Instrument (TKI)** | Kenneth W. Thomas & Ralph H. Kilmann | *Conflict and Conflict Management* (1974); subsequent TKI publications. |
| **Bargaining for Advantage / Wharton evaluation grid** | Prof. G. Richard Shell | *Bargaining for Advantage: Negotiation Strategies for Reasonable People*, The Wharton School, University of Pennsylvania. |

This project is **not** affiliated with, endorsed by, or licensed from CPP / The Myers-Briggs Company, the Thomas-Kilmann Institute, or The Wharton School. It is an independent educational implementation that synthesises the public conceptual frameworks of these scholars.

## Features

- **30 forced-choice items** — deliberately short to encourage gut-level honest answers.
- **Five-mode scoring** — Competing, Collaborating, Compromising, Avoiding, Accommodating.
- **Wharton/Shell grid plot** — your profile rendered on the two-dimensional evaluation grid.
- **Personalised debrief** — interpretive text for each mode based on your tallies.
- **Printable PDF report** — generated client-side via jsPDF, ready to hand in or save.
- **Keyboard navigation** — `1` / `2` to choose, arrow keys to step through.
- **Mobile-first responsive UI** — works on phone, tablet, and desktop.
- **Zero tracking, zero accounts** — runs entirely in your browser; nothing is sent anywhere.
- **Accessible** — semantic HTML, focus states, sufficient colour contrast, screen-reader-friendly labels.

## Screenshots

> Add screenshots here after deployment, e.g. `docs/screenshot-welcome.png`, `docs/screenshot-results.png`.

## Quick start

This is a pure static site — no build tools, no dependencies to install.

```bash
# clone
git clone https://github.com/<your-username>/negotiating-style-assessment.git
cd negotiating-style-assessment

# serve locally (any static server works)
python3 -m http.server 8080
# or
npx serve .
```

Then open http://localhost:8080 in your browser.

## Deployment

The site ships as static HTML, CSS, and JavaScript. Deploy to any static host:

- **Netlify** — drop the folder onto netlify.com or connect the repo. `netlify.toml` is included with sensible security headers.
- **GitHub Pages** — Settings → Pages → deploy from `main` branch root.
- **Vercel** — `vercel deploy` from the project root.
- **Cloudflare Pages**, **AWS S3 + CloudFront**, or any CDN that serves static files.

After deploying, do a project-wide find-and-replace of the placeholder URL `https://negotiating-style-assessment.netlify.app/` with your actual production URL. The placeholder appears in `index.html` (canonical, Open Graph, JSON-LD), `sitemap.xml`, and `robots.txt`.

## Project structure

```
.
├── index.html          # Single-file app: markup, styles, and the obfuscated logic bundle
├── netlify.toml        # Static-hosting config + security headers
├── robots.txt          # Search-engine directives
├── sitemap.xml         # Sitemap for indexing
├── LinkedIn_Post.md    # Ready-to-use launch announcement drafts
└── README.md           # You are here
```

## Use in the classroom

Educators are welcome to use this assessment as a self-reflection exercise alongside negotiation, conflict-management, organisational-behaviour, or leadership courses. A typical pattern:

1. **Pre-class** — students complete the assessment and submit the PDF report.
2. **In-class** — students cluster by dominant mode; instructor surfaces the trade-offs of each.
3. **Debrief** — pair students with contrasting modes for a short role-play; reflect on how their default mode helped or hurt them.

If you adopt it for your own course, I'd love to hear about it — see [Contact](#contact).

## Privacy

The assessment runs entirely in your browser. **No answers, names, or results are transmitted, stored, or logged anywhere.** The PDF is generated locally and delivered straight to your device. There are no analytics, cookies, or third-party trackers — only a Google Fonts request for the Inter typeface and a CDN request for jsPDF.

## Citation

If you reference this assessment in academic, training, or published work, please cite:

> Al-Tamimi, A.-K. (2026). *Negotiating Style Assessment* [Web application]. Retrieved from https://negotiating-style-assessment.netlify.app/

BibTeX:

```bibtex
@misc{altamimi2026nsa,
  author       = {Al-Tamimi, Abdel-Karim},
  title        = {Negotiating Style Assessment},
  year         = {2026},
  howpublished = {\url{https://negotiating-style-assessment.netlify.app/}},
  note         = {Web application}
}
```

## License

**Proprietary — All rights reserved © 2026 Abdel-Karim Al-Tamimi.**

The source code in this repository is provided for transparency and academic reference. Unauthorised copying, modification, reverse-engineering, redistribution, or commercial use of the application or its underlying logic is **strictly prohibited** without prior written permission from the author. Educators interested in using the assessment with their classes are encouraged to link to the live URL or to contact the author for permission.

## Contact

**Abdel-Karim Al-Tamimi** — University Professor
For collaboration, classroom adoption, or licensing enquiries, please reach out via [LinkedIn](https://www.linkedin.com/in/abdelkarim-altamimi) or email.

---

<sub>Keywords: Negotiating Style Assessment · Negotiation Style Test · Thomas-Kilmann Conflict Mode Instrument · TKI · Wharton · G. Richard Shell · Bargaining for Advantage · conflict resolution · negotiation training · Abdel-Karim Al-Tamimi · Abdelkarim Al-Tamimi · Abdel Karim Tamimi · university course · negotiation course.</sub>
