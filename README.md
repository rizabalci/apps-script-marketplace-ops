# Marketplace Ops Toolkit

**Case studies:** [rizabalci.github.io/case-studies](https://rizabalci.github.io/case-studies/)

Google Apps Script and Looker Studio templates for running seller-fulfilled marketplace operations (Amazon SFP, bol, Otto, ManoMano) across several 3PL warehouses. Built and run in production, then cleaned into templates: no company names, IDs or business data.

## Apps Script

| Repo | What it does |
|---|---|
| [apps-script-marketplace-health-collector](https://github.com/rizabalci/apps-script-marketplace-health-collector) | Daily account health from Amazon SP-API, bol and Otto APIs, weekly late dispatch per warehouse from JTL SQL, job heartbeat, ManoMano monitor |
| [apps-script-prime-badge-check](https://github.com/rizabalci/apps-script-prime-badge-check) | Prime badge and delivery promise per product and postcode, EU health views, watchdog and US alerts |
| [apps-script-account-health-dashboard](https://github.com/rizabalci/apps-script-account-health-dashboard) | Single-marketplace health page with rolling-window roll-off estimates |
| [apps-script-sfp-weekly-dashboard](https://github.com/rizabalci/apps-script-sfp-weekly-dashboard) | Weekly SFP KPIs, tier headroom and freshness strip |
| [apps-script-ops-action-engine](https://github.com/rizabalci/apps-script-ops-action-engine) | Turns findings into owner-assigned actions and drafts-only partner emails |

## Looker Studio

| Repo | What it shows |
|---|---|
| [looker-studio-marketplace-account-health](https://github.com/rizabalci/looker-studio-marketplace-account-health) | One page per marketplace: latest reading, headroom in units, trends, breach history |
| [looker-studio-sfp-us-dashboard](https://github.com/rizabalci/looker-studio-sfp-us-dashboard) | SFP control room: on-time per size tier, late packages by cause, weekly trend |
| [looker-studio-3pl-scorecard](https://github.com/rizabalci/looker-studio-3pl-scorecard) | Weekly warehouse scorecard: same-day dispatch, week over week, late reasons, label-to-scan timing, cost per parcel |
| [looker-studio-landed-cost-monitor](https://github.com/rizabalci/looker-studio-landed-cost-monitor) | Per-unit COGS, shipping and fees by marketplace and channel, outliers and missing COGS |

Each Looker repo has the Sheet schema, every calculated field, the page layout, build steps and fake sample data.

## Principles

Read-only towards marketplaces. Drafts, never sends. Never estimate a missing number. Warehouse scorecards rate sites, not people.

## License

MIT
