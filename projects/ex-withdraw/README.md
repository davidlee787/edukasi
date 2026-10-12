# Ex-Withdraw

**Status:** A transaction/withdrawal interface was previously started in the root app. Audit the current source before claiming feature completeness.

## Required before production
- Treat all current balances and transactions as demo-only until verified.
- Implement server-side authentication and authorization.
- Use a durable transactional ledger and idempotent operations.
- Validate every request on the server and keep secrets out of client bundles.
- Add audit logs, rate limits, tests, and a documented provider integration before any real payment use.

No real payment or withdrawal is confirmed by this documentation.
