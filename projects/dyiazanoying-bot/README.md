# DyiazAnoying WhatsApp Bot

**Status:** Requirements recorded; complete bot source has not yet been imported into this repository.

## Requested scope
- Node.js bot with modular command handlers, a readable text menu, configuration, and error handling.
- Use the supported WhatsApp library/API within its terms.
- Keep authentication/session state private; never commit session files or tokens.
- Store secrets in runtime environment variables and add health logging without exposing credentials.

## Hosting
This bot is a long-running Node.js service and is separate from the Vercel frontend. Deploy it to an appropriate persistent Node.js host; a GitHub folder alone does not keep it running.
