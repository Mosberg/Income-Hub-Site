---
name: digital-product-newsletter-pipeline
description: Runs a low-effort digital-product shop + weekly newsletter for a Denmark-based seller. Use when the user asks to create a product, draft the newsletter, process sales, deliver files, or produce the monthly P&L/tax summary.
---

# Digital Product + Newsletter Pipeline (DK/EU)

## Context (fill once)
- Niche, audience, tone; storefront = PayPal links | Gumroad
- Tax status: hobby | enkeltmandsvirksomhed (CVR); VAT registered: yes/no
- Folders: Drive/Dropbox paths for products; Sheets ledger ID; Calendar name

## Hard rules
- Never publish or send to subscribers without explicit user approval.
- Never send unsolicited marketing email (markedsføringsloven § 10).
- Label affiliate links "Reklamelink"; disclose AI use on product pages.
- No mass page generation (Google scaled content abuse); max 1 new product/month.
- Flag turnover approaching 50,000 kr. (moms) and €10,000 cross-border B2C (OSS) if not using a merchant of record.

## Scheduled routines
1. Every 4h: check PayPal transactions → send delivery email (Gmail) with Drive/Dropbox link → append row to ledger.
2. Weekly (Mon): research + draft newsletter issue → save to Docs → email user for approval.
3. Monthly (1st): P&L summary, fee totals, top products, next product proposal.
4. Yearly (Feb): totals for årsopgørelse (rubrik 20 hobby / 111 business) + reminder to verify with Skattestyrelsen.

## Procedures
- create_product.md: niche brief → outline → build (Sheets/Docs/PDF) → QA checklist → listing copy
- deliver_order.md: match payment → template email → log → handle refund requests (escalate)
- newsletter_issue.md: structure, length, CTA, disclosure lines
- compliance_checklist.md: AI disclosure, ad labelling, withdrawal-right wording, GDPR basics

## Escalate to user
- Any customer complaint, refund, chargeback (PayPal fees 100–120 DKK), platform warning, or legal/tax question.
