# XW Edukasi Arcade

XW is a responsive, dark-and-gold educational arcade interface built with React, TypeScript, Vite, and React Router. Its visual direction uses original cosmic/Olympus-inspired artwork and layouts; it does not bundle proprietary Gates of Olympus artwork or claim to be an official game.

## Included
- Responsive desktop and mobile layouts, navigation, search, categories, and game cards.
- Original XW logo, animated loading screen, sound toggle, and reduced-motion support.
- Six featured original arcade concepts plus the wider demo catalogue.
- Slot-style probability demonstration and a space/rocket arcade scene for learning about randomness and risk.
- Local virtual-credit balance, play history, demo transactions, referral and promotion screens.
- Local demo admin controls for interface testing.
- Indonesian copy and clear notices that credits and transactions are simulated.

## Important demo limits
- No real-money betting, payment processing, transfer, or cash-out is provided.
- Balances, transaction history, and demo admin settings are stored in the current browser's localStorage. They are not shared between devices and can be edited by the browser user.
- Demo deposit/withdraw screens are simulations only; payment tiles and QR artwork are illustrative and not scannable.
- The local admin view is not authentication and must never be treated as production security.
- The project does not have a backend or external database configured.

## Run locally
1. Install Node.js 22 (or a supported current Node.js version).
2. Run `npm install`.
3. Run `npm run dev`.
4. Open the local URL printed by Vite.

## Build
```bash
npm run build
npm run preview
```

The production bundle is written to `dist/`.

## Deploy on Vercel
- Import `davidlee787/edukasi` from GitHub.
- Framework preset: **Vite**.
- Build command: `npm run build`.
- Output directory: `dist`.
- Install command: `npm install`.
- `vercel.json` rewrites application routes to `/index.html` for client-side routing.

No API keys or environment variables are required for this frontend-only educational demo. Do not add payment credentials or secrets to client-side environment variables.

## Quality and accessibility
- Keyboard focus indicators are included.
- Motion respects `prefers-reduced-motion`.
- Sound is generated locally through Web Audio after user interaction; it can be switched off.
- Verify `npm run build` and inspect the Vercel deployment before treating any release as production-ready.
