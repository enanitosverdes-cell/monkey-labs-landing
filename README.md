# Monkey Labs AI — Landing Page

Marketing site for [monkeylabsai.com](https://monkeylabsai.com).

## What this is

Single-file static landing page (HTML + inline CSS + inline JS, no build step) served from Hostinger Premium Web Hosting.

- **Domain:** `monkeylabsai.com`
- **Host:** Hostinger Premium (LiteSpeed)
- **Deploy path:** `/home/u866977923/domains/monkeylabsai.com/public_html/index.html`
- **Demo app (separate):** [app.monkeylabsai.com](https://app.monkeylabsai.com) lives under `/app/` in the same hosting account and is deployed from the [`monkey-labs-demo`](https://github.com/enanitosverdes-cell/monkey-labs-demo) repo — **do not** touch that path from this repo.

## Stack

- Plain HTML5 — no React, no Vite, no framework
- Inline CSS (CSS custom properties, OKLCH-aware)
- Inline JS (vanilla, ~60 lines)
- Inline SVG icons + logo (zero external image assets)
- Google Fonts: Instrument Serif + Inter + JetBrains Mono

## Deploy

Production deploys land via SSH:

```
host:  147.93.42.213
port:  65002
user:  u866977923
path:  /home/u866977923/domains/monkeylabsai.com/public_html/index.html
```

Always back up the live file before overwriting:

```
ssh -p 65002 u866977923@147.93.42.213 \
  "cp /home/u866977923/domains/monkeylabsai.com/public_html/index.html \
      /home/u866977923/domains/monkeylabsai.com/public_html/index.backup.$(date +%s).html"
```

## Repository status

The initial commit captures the **production landing as of 2026-05-28** — the version still framed as a marketing-agency chatbot for aesthetic clinics. A full repositioning to the unified SaaS platform narrative ("Tu empresa trabajando 24/7 con IA") is planned next.
