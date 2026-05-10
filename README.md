# manish6298.github.io

Personal portfolio website — built from scratch as a single-file HTML/CSS/JS app with Three.js for 3D background effects.

## What's in here

A frontend built to replace an older, stale portfolio. This one reflects where I actually am: 5 years at TCS, two major enterprise clients (British Telecom and Avis Budget Group), and a solid backend engineering background.

The whole thing lives in one `index.html` file. No frameworks, no build tools, no npm. Vanilla JS, CSS variables, and Three.js loaded from a CDN — easier to maintain and deploy on GitHub Pages without any CI config.

## Stack used

- **Three.js (r128)** — particle field, line segments, parallax camera on mouse move
- **Vanilla CSS** — custom properties, scroll-triggered animations via IntersectionObserver, no Tailwind or Bootstrap
- **DM Serif Display + Sora** — loaded from Google Fonts
- **Zero dependencies** beyond the above — no React, no bundler

## Structure

```
manish6298.github.io/
├── index.html                        # entire site
├── images/
│   └── selfpic.png                   # profile photo used in About section
├── Manish_Srivastava_Resume_2026.pdf # linked from the resume download button
└── README.md
```

## Sections

1. **Hero** — name, role typewriter, four key metrics, CTA buttons
2. **About** — summary with profile photo and highlights
3. **Skills** — six skill cards (Java, REST/Microservices, AI tooling, Cloud/DevOps, DB/Caching, Testing) + tech pill tags
4. **Experience** — timeline: TCS (Avis Budget Group + British Telecom) and PrintIndiaMart internship
5. **Achievements** — three recognition cards with real numbers
6. **Education & Certifications** — B.Tech, Class XII, Class X + two TCS iEvolve certs
7. **Contact** — four direct connect buttons (Gmail, WhatsApp, LinkedIn, GitHub) + one-click email copy. No contact form.

## Contact section — design decision

The old contact section had a form that used `mailto:`, which opened the OS mail client instead of Gmail — confusing for visitors. It's been replaced with four direct connect buttons:

- **Gmail** — links to `https://mail.google.com/mail/?view=cm&to=...` so it opens Gmail in the browser, never the desktop mail app
- **WhatsApp** — deep link via `https://wa.me/918318241519` with a pre-filled message
- **LinkedIn** — direct profile link
- **GitHub** — links to the GitHub profile

There's also a one-click email copy button below the buttons for convenience.

## Running locally

No build step. Just open the file:

```bash
# Option 1 — direct
open index.html

# Option 2 — local server (avoids any CORS quirks with the PDF link)
python3 -m http.server 8080
# then visit http://localhost:8080
```

## Why single-file

GitHub Pages serves static files directly from the repo root. Keeping everything in one HTML file means there's no routing to configure, no 404s on refresh, and the PDF sits right next to it — the download link just works.

## Contact

- Email: [manish.sri9559@gmail.com](mailto:manish.sri9559@gmail.com)
- LinkedIn: [linkedin.com/in/manish-srivastava-b564701a7](https://linkedin.com/in/manish-srivastava-b564701a7)
- GitHub: [github.com/Manish6298](https://github.com/Manish6298)
- WhatsApp: [wa.me/918318241519](https://wa.me/918318241519)

---

© 2026 Manish Srivastava. All rights reserved.
