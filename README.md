# Vignesh Jogi · Portfolio & Resume

Live: **https://vignesh-jogi.vercel.app**

Personal portfolio of Vignesh Jogi, Full-Stack Engineer (Node.js · Next.js · MongoDB · GCP).

## What's inside

| File | Purpose |
| --- | --- |
| `index.html` | The site: sticky profile column, interactive **Live system map** (canvas), achievements, experience, live products, skills |
| `resume-print.html` | Print layout used to generate the PDF (not deployed) |
| `Vignesh-Jogi-Resume.pdf` | 2-page A4 resume, served by the Download PDF button |
| `og-image-v2.jpg` | Social share preview (LinkedIn, WhatsApp, X) |
| `robots.txt`, `sitemap.xml` | SEO |

## Tech

Plain HTML, CSS and vanilla JavaScript: no framework, no build step.

- Canvas 2D system map: apps → shared API → services, with animated request pulses, hover/tap highlighting, and pausing when off-screen or when reduced motion is preferred
- Light/dark themes via CSS custom properties, remembered per visitor
- Structured data (JSON-LD `Person`), Open Graph and Twitter cards
- Responsive down to 360px, accessible (semantic HTML, keyboard focus, ARIA labels)

## Update the PDF

```bash
"/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" --headless=new \
  --no-pdf-header-footer --print-to-pdf=Vignesh-Jogi-Resume.pdf \
  "file://$PWD/resume-print.html"
```

## Deploy

Pushing to `main` deploys to Vercel automatically (GitHub → Vercel, connected Sep 2026). Other branches get preview URLs.

Built with [Claude Code](https://claude.com/claude-code).
