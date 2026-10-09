# Income Hub

A free, private tracker for people building small online income streams with AI help. Log sales and costs, track hours, manage content approvals and leads, and see at a glance whether each pipeline is actually paying off.

**Live site:** https://mosberg.github.io/Income-Hub-Site/

Everything runs in your browser. There is no server, no account and no tracking, and nothing you enter is sent anywhere.

## What it does

| Tab | Purpose |
|---|---|
| Dashboard | Income, fees, costs, net, hours and net per hour. Per-pipeline table, a 6-month net chart, a 12-month income meter against your VAT-threshold setting, and "review due" alerts. |
| Ledger | Add, edit and delete income and expenses, by pipeline, with platform fees and buyer country. |
| Tasks & approvals | A content board (draft, needs approval, approved, published, dropped) so nothing goes public unreviewed. |
| Leads | A small client tracker for service work: stage, value, next step and date. |
| Pipelines | Status, start date, 90-day review date and a stop/change rule for each pipeline, plus an hours log. |
| Checklists | Shared compliance items plus extras for each pipeline. Progress is saved. |
| Prompts for Claude | Builds copy-paste prompts such as "Use the digital-product-newsletter skill. Draft this week's content." |
| Settings | Currency label, VAT threshold, tax-status note, JSON backup and restore, CSV export and import, erase all data. |

### The nine pipelines

Digital products + newsletter, AI admin automation service, freelance AI gigs, newsletter monetization, KDP ebooks, Etsy / POD / downloads, micro-SaaS / API, content / affiliate site (high risk), faceless video (high risk).

## Using it

1. Open the site and start logging in the Ledger tab.
2. For each pipeline you try, set a status and a 90-day review date on the Pipelines tab. Use the review to decide honestly whether to continue, change one thing or stop.
3. Work through the Checklists before you publish anything.
4. Export a JSON backup from Settings regularly.

Zero income in the first months is a normal result. The tracker only shows what you log.

## Your data

- Stored in your browser's `localStorage`, per browser and per web address.
- Clearing site data or using private browsing can erase or block it. Back up from Settings.
- To move to another device, export a JSON backup and import it there.
- CSV import and export covers the ledger only. Spreadsheet formulas in exported cells are neutralized.

## What it does not do

- It does not connect to PayPal, Gmail or any platform. You record sales yourself, or have Claude add rows in a chat.
- It does not give tax, legal or financial advice. The VAT threshold is an editable setting, not a verified rule: confirm current figures at [skat.dk](https://skat.dk). Hobby vs. business status, VAT registration and deductions are decisions to confirm with Skattestyrelsen or an accountant.
- It does not guarantee or predict earnings.

## Run or host it yourself

There is no build step. The whole app is one file, `index.html`, with no dependencies.

- **Locally:** open `index.html` in a browser.
- **GitHub Pages:** push to a public repository, then Settings → Pages → Deploy from a branch → `main` / `(root)`. The `.nojekyll` file tells Pages to serve the file as is.

## Repository contents

```
index.html   the entire app (HTML, CSS and JavaScript)
.nojekyll    serve files as is on GitHub Pages
README.md    this file
LICENSE      MIT
```

## Contributing

Issues and pull requests are welcome. Keep it dependency-free and single-file, keep all user data local, and escape anything rendered into the page.

## License

[MIT](LICENSE) © 2026 Mosberg
