# Partners Group demo: what changed from the 26N version, and why

Built 16 October 2026 from the 26N master demo. Same format, same 40-step Microsoft 365 tour, same Vercel deploy. Everything Partners Group-specific was rewritten.

## What Partners Group cares about in 2026, and how the demo answers it

| Partners Group focus (public) | What the demo now shows |
|---|---|
| Marks and valuation evidence are under scrutiny across private markets, and evergreens with regular NAVs hold USD 54bn, nearly 30% of AUM | A **Valuation view** replaces the 26N insurance view: maintainable EBITDA, multiple inputs, NAV look-through, each traced to source rows, corrected before the NAV is struck |
| Several PE holdings carry heavy debt with 2028 maturities; lenders and CLO holders want earlier warning | The **Credit view**: covenant EBITDA recomputed from source, a springing test, leading monitors 4–12 weeks ahead of quarterly reports |
| Private credit is a USD 40bn business, a new global evergreen launched 9 Oct, and AIFMD II requires credit-monitoring policies for loan-originating funds from April 2026 | The platform's lending book and the "same view on every private credit borrower" panel, framed for Andrew Bellis's team |
| Value creation in large holdings, with an IPO seen as possible for Breitling in 2027–29 (FT) | The **Equity view**, the weekly board and the value bridge: seven levers worth about CHF 23.5M of EBITDA without a new boutique |
| One integrated platform across PE, credit and valuation, with information walls | **One evidence set**: one fact base, three views, permissions and walls enforced in Microsoft 365 |

## The main changes

1. **Holding: Onelife Fitness → Breitling.** Breitling is Partners Group's flagship consumer holding (about 51% since 2023, with CVC). It lets one company speak to all three audiences: the board and deal team, the lenders and CLO holders, and the valuation committee behind the evergreen NAV.
2. **Insurance view → Valuation view.** 26North runs an insurer; Partners Group runs evergreens. The third audience is now the valuation committee, the auditors and evergreen investors. The Word "holdings note" became a "September valuation note".
3. **The restatement event.** Was a USD 1.2M pre-opening add-back at three gyms. Now CHF 1.9M booked as non-recurring restructuring that is really recurring hiring cost for 14 back-filled boutique roles. It moves covenant EBITDA (160.4 → 158.5), maintainable EBITDA (154.3 → 152.4) and value (−2.4% equity, about −3 bps of NAV), all before the lender report is sent and the NAV is struck.
4. **New packet.** `breitling-packet.html` (9 tabs, 79 graphs, about 60 tables) replaces the Onelife packet: Swiss watch market, Breitling, weekly board, value plan, one evidence set, assumptions and FAQ. Brand rules kept: About CreditSwan is tab 02, motion audit passes.
5. **Diagnostic pages.** Capex gate became a boutique gate (company boutique CHF 3.5–9.5M vs partner boutique CHF 0.8M). Weekly charts now track US dealer weeks of stock, pre-owned prices, inventory days, the revolver against the springing trigger, and so on.
6. **Naming throughout.** Hub "Partners Group Platform", PG brand mark in navy, Teams channel "Breitling", Copilot questions, Planner tasks, Power Automate flows, the "How it is built" panel and the disclaimer. The deal history now runs from 1996, Partners Group's founding year.
7. **Roll-out page.** Aroma-Zone first (Partners Group lent to it from 2021 and in August entered exclusive talks to buy a majority, so it shows credit and equity on one company), then KinderCare, Confluent Health, Foundation Risk Partners and Version 1.
8. **Markdown edition** rewritten for Breitling and Partners Group (three documents).

## Choices worth a second look before sending

- **Signed-in user: Andrew Bellis, Head of Private Credit.** The base platform is a lender's command center, so the credit head fits it best. Swapping to someone else (for example Roberto Cagnati, incoming Co-CEO) is a one-line change to `window.__BRAND` in `index.html`.
- **Tone.** The demo does not mention the April short-seller report, the June evergreen gates, the share price or the "wall of debt" headlines. It frames valuation and monitoring scrutiny as industry-wide.
- **Illustrative numbers.** Every Breitling operating, debt and valuation figure is a labelled model anchored to public facts (FY Mar-26 sales CHF 769M, adjusted EBITDA CHF 162M). The 13.0x multiple is stated as not Partners Group's mark. If you would rather not show a value effect on a Partners Group holding at all, the Valuation view's figures are the ones to soften.
- **The FT-reported owners' marks** (about 0.7x for Partners Group, 0.5x for CVC) appear only in the internal `evidence-baseline.md` public anchors, not in the demo or the packet. Delete that line before sending if the baseline file goes too.
- **Unchanged:** the veterinary care Diligence File (PDF, workbook, interactive edition) and the synthetic lending book (Juniper, Saffron and others) are the same synthetic samples as before.
