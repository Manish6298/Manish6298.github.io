# manish6298.github.io

Personal portfolio website — built from scratch as a single-file HTML/CSS/JS app with Three.js for 3D background effects.

## What's in here

A frontend I put together to replace my older portfolio (which was getting stale — it still said 3 years of experience). This one reflects where I actually am now: 5 years at TCS, two major enterprise clients, and a proper backend engineering background.

The whole thing lives in one `index.html` file. No frameworks, no build tools, no npm. Just vanilla JS, CSS variables, and Three.js loaded from a CDN. Easier to maintain and deploy on GitHub Pages without any CI config.

## Stack used

- **Three.js (r128)** — particle field, wireframe geometries, parallax camera on mouse move
- **Vanilla CSS** — custom properties, scroll-triggered animations via IntersectionObserver, no Tailwind or Bootstrap
- **Space Mono + Syne** — loaded from Google Fonts
- **Zero dependencies** beyond the above — no React, no bundler

## Structure

```
manish6298.github.io/
├── index.html                        # entire site
├── Manish_Srivastava_Resume_2026.pdf # linked from the resume download button
└── README.md
```

## Sections

1. **Hero** — name, role, four key metrics, CTA buttons
2. **About** — summary + four highlight cards (AI tooling, cloud, performance, client wins)
3. **Tech Stack** — eight skill cards grouped by category
4. **Experience** — timeline with both TCS projects (Avis Budget Group, British Telecom) + internship
5. **Key Wins** — six achievement cards with real numbers
6. **Education & Certs** — B.Tech, two TCS iEvolve certifications
7. **Contact** — links + resume download

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

GitHub Pages serves static files directly from the repo root. Keeping everything in one HTML file means there's no routing to configure, no 404s on refresh, and the PDF sits right next to it in the root — the download link just works.

## Contact

- Email: manish.sri9559@gmail.com
- LinkedIn: [linkedin.com/in/manish-srivastava-b564701a7](https://linkedin.com/in/manish-srivastava-b564701a7)
- GitHub: [github.com/Manish6298](https://github.com/Manish6298)
