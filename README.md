# Tripletex Partner Cloud

A partner management portal built for Tripletex, designed to help internal teams manage and monitor the partner ecosystem — tier status, leads, customers, support cases, training, and kickbacks.

## Features

- **Plan / Årshjul** — Annual goal tracking with quarterly breakdown, editable targets per partner
- **Partner Overview** — Full list of partners with tier status, points, revenue, YTD kickback, and contact info
- **Tier System** — Automatic Bronze / Silver / Gold classification based on accumulated points
- **Lead Management** — Submit and track leads including referrals and accounting office referrals
- **Customer Roster** — Per-partner customer list with ARR and status tracking
- **Support Cases** — Log and manage support cases with priority, category, and comment threads
- **Training & Certification** — Course library with point rewards and certification bonuses
- **Analytics** — Charts for ARR per partner, lead status, submissions over time, and tier mix

## Tier Structure

| Tier   | Points Required | Kickback | MDF (NOK/yr) |
|--------|----------------|----------|--------------|
| Bronze | 0–999          | 5%       | —            |
| Silver | 1,000–2,999    | 10%      | 5,000        |
| Gold   | 3,000+         | 18%      | 20,000       |

## Tech Stack

- **React 18** (via CDN — no build step required)
- **Chart.js 4** (via CDN — analytics charts)
- Single `index.html` — fully self-contained, no server needed

## File Structure

```
tripletex-partner-cloud-deploy/
├── index.html        # The app — open locally or deploy directly
├── vercel.json       # Vercel routing config
├── README.md
├── src/
│   └── app.jsx       # React source (readable reference)
└── docs/
    ├── use-cases.pdf
    └── salesforce-pitch.pdf
```

## Run Locally

Open `index.html` in a browser — no install, no server needed.

## Deploy

### Vercel
1. Connect this repo at [vercel.com/new](https://vercel.com/new)
2. Leave root directory as `/`
3. Done — you get a public URL instantly

### Netlify
1. Go to [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag `index.html` onto the page
3. Done

## Status

Internal prototype / demo using mock data. Not connected to live Tripletex systems.
