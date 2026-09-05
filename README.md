# Agentic Forge — Website

Live site: [agenticforge.com.au](https://www.agenticforge.com.au)

## Stack & Hosting

- **Code:** Single static `index.html` (HTML/CSS, no framework, no build step).
- **Repo:** GitHub — connected directly to Vercel.
- **Hosting:** Vercel. Every push to the main branch on GitHub auto-deploys.
- **Domain:** `agenticforge.com.au` — custom domain connected via Vercel's Domains tab. DNS is pointed at Vercel's nameservers/records (check Vercel → Project → Settings → Domains for exact A/CNAME records if it ever needs re-pointing).

## How to deploy a change

1. Edit `index.html` locally (or directly on GitHub).
2. Commit and push to the main branch.
3. Vercel auto-builds and deploys — check the **Deployments** tab in the Vercel dashboard for status (green = live, red = failed).
4. Changes go live at the domain automatically within a minute or two once the deploy is green.

## How to check if the site is healthy

- Open [vercel.com/dashboard](https://vercel.com/dashboard) → the Agentic Forge project → **Deployments** tab.
- Green check = live and working.
- Red X = build failed — click into the deployment to see the error log.
- Visit the live domain in an incognito window to confirm what's actually published (avoids cache confusion).

## Current site structure (as of Sept 2026)

Single page (`index.html`) with sections:
- Hero
- Marquee (AI Agents / Automation / Model Evaluation / etc.)
- "What we forge" — 3 service cards (Agents, Automation, Evaluation)
- "How we work" — 3-step timeline
- Quote/glow panel
- Contact CTA (currently a `mailto:` link)
- Footer (X/Twitter link only)

## Known issues / TODO

- [ ] Mobile nav breaks under 880px width — nav links disappear, only logo shows. Needs a hamburger menu or stacked layout.
- [ ] No `/work` page — no case studies or proof of past projects. Highest priority for recruiter/client trust.
- [ ] No `/about` page.
- [ ] No `/contact` page — currently just a `mailto:` link, weak conversion.
- [ ] No Open Graph / social share meta tags — links shared on LinkedIn/X/Slack show no preview image or description.
- [ ] No favicon reference confirmed in `<head>`.
- [ ] No `/privacy` page — needed once the site collects any emails via a form.
- [ ] Footer only links to X — add LinkedIn, GitHub, email.

## Notes to self

- Domain registrar: [fill in — e.g. GoDaddy / VentraIP / Crazy Domains].
- If domain ever stops resolving: check DNS records in the registrar match what Vercel's Domains tab expects.
- This README exists so I stop forgetting my own stack setup.
