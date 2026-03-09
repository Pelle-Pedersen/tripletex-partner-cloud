# Tripletex Partner Cloud — Prototype

## Purpose

This is an interactive prototype built to demonstrate what a **Salesforce Partner Cloud** implementation could look like for Tripletex's partner programme.

Tripletex works with a network of accounting firms and resellers ("partners") who bring in new clients, refer businesses, and help customers get set up on the platform. Today, managing these relationships — tracking performance, rewarding partners, handling leads and support — is largely manual.

This prototype visualises how a dedicated Partner Cloud portal could:
- Give partners a single place to track their performance, rewards, and goals
- Give Tripletex an admin view to monitor the full partner ecosystem
- Replace manual follow-up with structured workflows for leads, cases, and training
- Motivate partners through gamification, tier progression, and visible incentives

It is **not** connected to live systems. All data is demo data. The purpose is to align stakeholders on scope, flow, and value before committing to a full Salesforce implementation.

---

## How It Works

The app has two views — **Partner View** and **Admin View** — switchable from the top navigation bar.

### Partner View
A partner logs in and sees their own dashboard. They can:
- Track progress toward annual goals (Årshjul) across clients, leads, Voucher Automation accounts, and revenue
- See quarterly breakdown of their performance
- Submit leads directly to the Tripletex sales team
- View their client roster and ARR
- Complete training courses and earn points toward tier upgrades
- See their commission (kickback) structure and YTD earnings
- Log support cases that route to Salesforce Service Cloud
- View their personal analytics

### Admin View
Tripletex staff see the full programme. They can:
- View all partners, their tier status, points, clients, and YTD commission
- Edit annual targets per partner (override tier defaults)
- Monitor the full lead pipeline across all partners
- Manage and update support cases
- View programme-wide analytics: ARR per partner, lead conversion, tier distribution, and submission trends

---

## Tabs

| Tab | Description |
|-----|-------------|
| **Plan** | Annual goals (Årshjul), quarterly progress breakdown, editable targets |
| **Enable** | Training courses and certifications with point rewards |
| **Recruit & Sell** | Lead submission and pipeline — New Client, Referral, Refer Accounting Office, Refer Business to Tripletex |
| **Incentivize** | Points breakdown, achievements, tier progress, and active challenges |
| **Support** | Support case management with priority, category, and comments |
| **Analytics** | Charts: ARR per partner, lead status, submissions over time, tier mix |

---

## Tier Programme

Partners earn points through activity and are automatically placed into tiers:

| Tier | Points | Kickback | MDF / yr |
|------|--------|----------|----------|
| 🥉 Bronze | 0 – 999 | 5% | — |
| 🥈 Silver | 1,000 – 2,999 | 10% | 5,000 NOK |
| 🥇 Gold | 3,000+ | 18% | 20,000 NOK |

Points are earned by submitting leads, onboarding clients, completing courses, winning deals, and earning certifications.

---

## Tech Stack

- **React 18** — via CDN, no build step required
- **Chart.js 4** — analytics charts, via CDN
- Single `index.html` — open in any browser, no install needed

---

## File Structure

```
├── index.html          # The application — open locally or deploy
├── vercel.json         # Vercel routing config
├── README.md
├── src/
│   └── app.jsx         # React source code (readable reference)
└── docs/
    ├── use-cases.pdf
    └── salesforce-pitch.pdf
```

## Run Locally

Open `index.html` in a browser — no install or server needed.

## Deploy

**Vercel:** Connect this repo at [vercel.com/new](https://vercel.com/new), leave root as `/`, done.

**Netlify:** Drag `index.html` onto [app.netlify.com/drop](https://app.netlify.com/drop), done.

---

## Status

`main` — v1 baseline
`Partner-Cloud-v2` — active development

Internal prototype using mock data. Not connected to live Tripletex or Salesforce systems.
