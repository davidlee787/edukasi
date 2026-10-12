# Project Hub — Muhammad Dyiaz

This repository is the central workspace for the projects listed below. The current root app is the XW Edukasi Arcade Vite application. A project is marked **source present** only when its implementation is actually included in the repository; a specification/entry in this index is not a claim that its complete source code has been imported.

## Project index

| Project | Scope | Current status |
|---|---|---|
| XW Edukasi Arcade | Responsive original arcade UI, educational probability demos, virtual points, local demo admin | **Source present** in the root Vite app |
| Ex-Withdraw | Withdrawal/transaction interface previously started in this repository | **Needs source audit and testing**; do not treat as payment-ready |
| DyiazAnoying Web / DyiazFitur | Indonesian/English utility portal; media URL tools, generators, Brat-style stickers, QR/UUID/text utilities, Gemini/RapidAPI integrations | **Specification recorded; complete source not yet imported here** |
| DyiazAnoying WhatsApp Bot | Baileys-based WhatsApp bot with menus and modular commands | **Specification recorded; complete bot source not yet imported here** |
| Telegram Utilities Bot | Telegram bot concept for safe utility workflows and customer support | **Specification recorded; complete source not yet imported here** |
| Downloader Tools | Link-based media helper for supported providers, with server-side API keys and provider-compliant handling | **Part of the DyiazAnoying web scope; source not yet audited/imported** |
| Football & Prayer Dashboard | Football fixtures/results for supported leagues, Jakarta/West Java prayer schedule, date/time, audio and support links | **Specification recorded; complete source not yet imported here** |

## Repository layout target

- `src/` and `public/`: existing XW Edukasi Arcade frontend and assets
- `projects/xw-arcade/`: scope and limitations
- `projects/ex-withdraw/`: transaction UI audit notes
- `projects/dyiazanoying-web/`: web tools requirements
- `projects/dyiazanoying-bot/`: WhatsApp bot requirements
- `projects/telegram-utilities/`: Telegram bot requirements
- `projects/football-prayer/`: football and prayer dashboard requirements

## Important integration notes

- Vercel currently builds the **root Vite app only**. Separate Node.js bots must run as separate services/workers; a GitHub folder alone does not keep them online.
- Do not put API tokens in frontend code. Use server-side environment variables and an appropriate backend for Gemini, RapidAPI, or bot credentials.
- Never commit `.env` files, session credentials, WhatsApp auth state, bot tokens, or private keys.
- Downloader integrations must comply with each provider's terms and copyright rules; do not bypass access controls.
- Any payment, withdrawal, or balance feature remains a non-production mock until a secure backend, authorization, ledger, and provider integration are implemented and tested.
- XW remains an educational arcade using virtual points, with no real-money wagering or cash-out.

## Next integration stages

1. Import the actual source files for projects that currently live elsewhere or in earlier ZIPs.
2. Audit each app's package manifest, environment variables, routes, assets, and secrets.
3. Separate deployable targets (Vercel web apps versus always-on Node.js bot services).
4. Run builds and tests for each target and record verified results here.

See the project-specific READMEs under `projects/` for requirements and import status.
