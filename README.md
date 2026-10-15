# CRACK THE SAFE

A responsive Telegram Mini App prototype built with React and Vite.

## Prototype scope
- Premium graphite interface with a CSS-built animated 3D-style vault (no generated image assets).
- Russian and English UI.
- First-run briefing, case screen, countdown, attempts, dynamic navigation.
- Code entry keypad with whole-combination result feedback.
- Missions, demo attempt store, demo wallet, channel placeholder, referral screen, profile and preferences.
- Reduced-motion support and responsive mobile/Desktop layouts.

## Run locally
```bash
npm install
npm run dev
```

## Deploy to Vercel
Import this repository in Vercel. Framework preset: **Vite**. Build command: `npm run build`. Output directory: `dist`. No environment variables are required for this UI-only prototype.

## Important prototype limitations
- Game state and demo balances are local to the browser and are not shared across players or devices.
- Code checks currently simulate a failed attempt. No secret code is stored in the client, and there is no live winner selection yet.
- Store actions add demo attempts only. There are no real payments, cash prizes, or withdrawals.
- Missions, referral tracking, Telegram membership verification, and channel data are placeholders until a backend and Telegram integration are added.
- Before production, implement server-authoritative case state, atomic attempt deductions and winner selection, rate limiting, Telegram initData validation, idempotent payment processing, persistent ledger, admin tools, monitoring, backups, and the applicable legal/payment checks.

## Suggested next milestone
Connect a server/database and Telegram Mini App authentication, then implement shared case scheduling and secure attempt checking before enabling real purchases or prizes.
