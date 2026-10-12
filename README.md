# XW Edukasi Arcade — Project Workspace

The root application is XW Edukasi Arcade, a responsive React/TypeScript/Vite educational arcade interface with original cosmic/Olympus-inspired styling. This repository also maintains a project index for the other applications planned for consolidation.

## All projects index

See [PROJECTS.md](./PROJECTS.md) for the central index, current source-import status, and deployment architecture. Project requirements are documented under [projects/](./projects/).

**Important:** listing a project or documenting its requirements does not mean its full source has been imported. The existing root app is the only app currently configured as the Vercel Vite deployment. The separate DyiazAnoying web tools and bot projects still need their actual source files imported and tested.

## Root app features
- Responsive desktop/mobile arcade UI, navigation, search, categories and game cards.
- Original XW logo and artwork direction, sound toggle, motion accessibility.
- Educational probability demos and a space/rocket arcade scene.
- Browser-local virtual credits, demo history, simulated transactions, referrals and promotions.
- Local demo admin controls.
- Indonesian copy and explicit virtual-credit limitations.

## Demo limitations
- No real-money betting, payment processing, transfer, or cash-out.
- Balances, history and demo admin preferences are stored in browser localStorage; they are not shared between devices and are not secure.
- Deposit/withdraw screens are simulations; payment tiles/QR artwork are illustrative.
- The local admin view is not production authentication.
- The root app has no configured backend or external database.

## Run locally
1. Install Node.js 22 or another supported current version.
2. Run `npm install`.
3. Run `npm run dev`.
4. Open the local URL printed by Vite.

## Build
```bash
npm run build
npm run preview
```

The production bundle is written to `dist/`.

## Vercel
- Repository: `davidlee787/edukasi`
- Framework: Vite
- Build command: `npm run build`
- Output directory: `dist`
- Install command: `npm install`
- `vercel.json` rewrites routes to `/index.html` for client-side routing.

Separate Node.js bots require a persistent backend/worker; placing their source in this repository does not make them run on Vercel. API tokens and bot credentials must be stored server-side and never committed to Git.
