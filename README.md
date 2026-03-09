# Tripletex Partner Cloud

A partner management portal built for Tripletex, designed to help internal teams manage and monitor the partner ecosystem — tier status, leads, customers, support cases, training, and kickbacks.

## Features

- **Partner Overview** — Full list of partners with tier status, points, revenue, YTD kickback, and contact info
- **Tier System** — Automatic Bronze / Silver / Gold classification based on accumulated points
- **Lead Management** — Partners can submit and track leads; status changes trigger points and kickback calculations
- **Customer Roster** — Per-partner customer list with ARR and status tracking
- **Support Cases** — Log and manage support cases with priority, category, and comment threads
- **Training & Certification** — Course library with point rewards and certification bonuses
- **Activity Log** — Real-time feed of partner activity (leads, upgrades, completions)
- **Analytics Dashboard** — Revenue, lead conversion, and tier distribution overview

## Tier Structure

| Tier   | Points Required | Kickback | MDF (NOK/yr) |
|--------|----------------|----------|--------------|
| Bronze | 0–999          | 5%       | —            |
| Silver | 1,000–2,999    | 10%      | 5,000        |
| Gold   | 3,000+         | 18%      | 20,000       |

## Tech Stack

- **React** (via CDN — no build step required)
- **Tailwind CSS** (via CDN)
- Single `.html` file — fully self-contained, no server needed

## File Structure

```
tripletex-partner-cloud-deploy/
├── tripletex-partner-cloud_1.jsx    # React source (component logic)
├── tripletex-partner-cloud_1.html  # Standalone all-in-one HTML file
└── vercel-deploy/
    ├── index.html                   # Production build (Vercel/Netlify ready)
    ├── vercel.json                  # Vercel routing config
    └── README.md                    # Deploy instructions
```

## Run Locally

Just open `tripletex-partner-cloud_1.html` in a browser — no install, no server needed.

## Deploy

### Vercel
1. Go to [vercel.com/new](https://vercel.com/new)
2. Deploy from the `vercel-deploy/` folder
3. Done — you get a public URL instantly

### Netlify
1. Go to [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag the `vercel-deploy/index.html` file onto the page
3. Done

## Status

This is an internal prototype / demo application using mock data. Not connected to live Tripletex systems.
