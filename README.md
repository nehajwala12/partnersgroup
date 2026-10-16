# CreditSwan · Partners Group master demo

Prepared for Partners Group, with Andrew Bellis (Head of Private Credit) as the signed-in user. Built 16 October 2026 in the same format as the CreditSwan Microsoft 365 demo. The worked example is Breitling, Partners Group's majority-owned watchmaker.

## What is in it

| File | What it is |
|---|---|
| `index.html` | The demo: a simulated Microsoft 365 window (SharePoint, Teams, Outlook, Excel, Word, Planner, Power Automate, Copilot) with a 40-step guided tour |
| `creditswan-overview.html` | The 14-page CreditSwan overview, cover set to Partners Group · Andrew Bellis |
| `breitling-packet.html` | The Breitling packet (9 tabs, 79 graphs), also embedded in the demo's Portfolio site |
| `Veterinary_care_Diligence_File_Oct-26.pdf` / `.xlsx` | The synthetic sample Diligence File the demo opens and downloads |
| `vercel.json` | Clean URLs and `noindex, nofollow` |
| `markdown/` | The Markdown edition: Breitling private credit diligence, Breitling company diagnostic, and One evidence set for equity, credit and valuation |
| `evidence-baseline.md` | The one illustrative number set every part of the demo uses |

## The tour

- Steps 1–18: the platform (command center, knowledge graph over thirty years of deal rooms, pipeline, Diligence File, Copilot, a deal-room change, the monthly package check, the covenant workbook), as Partners Group's hub with Andrew as the user.
- Steps 19–28: Breitling after close. The portfolio monitor, a 15-finding diagnostic, the full Breitling packet in SharePoint, the 27-monitor Monday board, the value-bridge levers (CHF 160.4M → ~CHF 184M without a new boutique), the boutique gate (company boutiques against partner boutiques), the breach flow, the Teams board, Planner and the Word board note.
- Steps 29–37: One set of evidence for equity, credit and valuation. One fact base of 20 facts from six Breitling systems; this morning's restatement of the non-recurring add-back (CHF 5.7M → CHF 3.8M), replayable; the equity, credit and valuation views; permissions and walls; three Teams notes; the September valuation note in Word; Copilot; and a roll-out page across Partners Group holdings.
- Steps 38–40: model choice, the decision on the command center, the CreditSwan overview.

Use the arrow keys or the tour buttons. "Play" runs it hands-free. "Reset" goes back to step 1.

## Deploy to Vercel

The demo is a static site with no build step.

1. `npm i -g vercel` (once), then from this folder run `vercel deploy --prod`. Or drag the folder into a new project at vercel.com.
2. Framework preset: Other. No build command, and the output directory is the folder root.
3. `vercel.json` already sets clean URLs and keeps the site out of search engines.

Locally, open `index.html` in a browser. The PDF and workbook download links work once the site is served, for example with `npx serve .`.

## Changing the signed-in user

One line near the top of `index.html` sets the firm and the user: `window.__BRAND = {...}`. Change `user`, `first`, `ini`, `email` and `prepared` (for example to Roberto Cagnati) and everything in the demo follows. The overview's cover is set in `creditswan-overview.html` (`window.CS_WHY_CONFIG`) and in the copy embedded in `index.html`.

## What is real and what is illustrative

- **Public and sourced:** Partners Group's AUM, businesses and leadership; Breitling's ownership (minority 2021, majority from CVC 2023), FY Mar-26 sales and adjusted EBITDA, rating, store count in 2022, House of Brands; Swiss watch exports and US tariffs.
- **Illustrative model:** every Breitling operating figure, the weekly board, the debt terms and covenant, and the valuation multiple. Breitling publishes no full accounts and its debt terms are not public. The 13.0x multiple is a calibration to listed peers, not Partners Group's mark.
- **Synthetic:** the private credit borrowers (Juniper, Saffron and others), the veterinary care Diligence File and the colleagues in Teams and Outlook.
- **Simulated:** the Microsoft 365 window, with no live connection to any tenant.
- **Cross-side flag:** any Partners Group credit position in a Partners Group equity holding is a matter for compliance. The demo shows the evidence, not an allocation.
