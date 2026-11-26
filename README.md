# QuoteCraft Studio — Hub & Live Interactive Demos

**Serverless Web & Workflow Automation Studio for US Roofing & Remodeling Contractors.**

High-converting, mobile-first landing pages, interactive multi-step instant quote calculators, and `$0/month` serverless Google Workspace (Sheets + Drive + Gmail) lead pipelines engineered for 100% client ownership.

## Live Site Architecture (Cloudflare Pages · `$0/mo`)

```text
quotecraft-hub/
├── index.html                        # QuoteCraft Studio Hub, USD Packages, Agency Rates & Contact Page
├── demos/
│   ├── summit-ridge/
│   │   └── index.html                # Flagship Demo #1: 4-Step Roofing & Remodeling Page + <canvas> Photo Upload + JSON Inspector
│   └── roof-calculator/
│       └── index.html                # Technical Demo #2: Standalone US Roof Pitch, Squares & Waste Factor Estimator
├── _headers                          # Cloudflare Pages security & caching headers
├── robots.txt                        # Public indexing rules
└── .gitignore                        # Public repository hygiene & guardrails
```

## Key Engineering Highlights

- **Zero External Build Step:** Self-contained HTML5, CSS3, and Vanilla JavaScript files with embedded optimized WebP architectural photography for sub-second mobile loads.
- **Centralized Single-Block Configuration:** Update studio links, email, or booking URL in one block (`STUDIO_CONFIG` in `index.html`) or rebrand the flagship demo in minutes (`CLIENT_CONFIG` in `demos/summit-ridge/index.html`).
- **Client-Side Photo Compression:** HTML5 `<canvas>` pipeline resizes and compresses large mobile jobsite photos by 85–95% in the browser before upload.
- **Security by Default:** XSS-safe DOM rendering, honeypot & dwell-time spam defenses, spreadsheet formula-injection protection, and Cloudflare Pages security headers.

## Adding Future Live Demos

1. Create a new subfolder under `demos/<demo-slug>/index.html`.
2. Add a return link to `../../` so visitors can navigate back to the QuoteCraft Studio Hub cleanly.
3. Push to `main` — Cloudflare Pages automatically deploys the new route at `/demos/<demo-slug>/`.

---

**Wahyu Pamungkas — Founder, QuoteCraft Studio**
- Book a 15-Min Discovery Call: https://cal.com/quotecrafthq/15min
- Direct Email: `quotecrafthq@gmail.com`
- Fiverr: https://www.fiverr.com/quotecrafthq
- Instagram: https://www.instagram.com/quotecraft.hq
- GitHub: https://github.com/quotecrafthq
