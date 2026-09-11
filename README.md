# IDCOL DRS Platform — interactive demo prototype

Live demo: **https://sadiasajarun.github.io/DRS-demo/**

A connected demo of the Domestic Rooftop Solar (DRS) Program web platform across three roles — **Household**, **DA Agent** and **IDCOL Staff** — sharing one live state in the browser. No backend, no build step: all data is simulated in `localStorage`.

| Entry point | What it shows |
|---|---|
| `index.html` → `app/home.page.html` | Demo landing — enter a role (Household → DA → IDCOL), platform areas, then the Simulation as the last step |
| `app/simulation.page.html` | Connected Journey Simulation — 6 guided journeys over an 11-step lifecycle, with the three live portals side by side (Next / Prev / Auto-play / Reset, +1 / +10 days) |
| `household/*.page.html` (6) | Household portal — system, loan, pay, receipts, complaint |
| `da/*.page.html` (10) | DA Agent portal — walled to the active DA; households, inventory, collections, claims, monitoring, tickets, IDCOL facility |
| `idcol/*.page.html` (23) | IDCOL Staff portal — MIS, Inspection, RMP, CRM / Finance (loan ledger, reconciliation, halt/resume, tickets), reports, audit, settings |
| `app/modules.page.html` | Module requirements map (reference) |

Shared files: `drs-sim.js` (state engine: seed data, domain rules, scenario), `drs-ui.js` (shell + renderers), `drs-theme.css` (design system).

Demo tips: on IDCOL pages use the top-bar **acting user** selector to show maker-checker (review as A. Karim, approve as S. Chowdhury). **Reset data** (profile menu) restores the seed. Business thresholds shown in the demo are illustrative and labelled as such.

All data is simulated in your browser; nothing is sent anywhere.
