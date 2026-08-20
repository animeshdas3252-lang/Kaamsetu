# KaamSetu Production V1
Run: `npm install`, copy `.env.example` to `.env`, set a strong JWT_SECRET, then `npm start`.
Includes signup/login, jobs, proposals, proposal acceptance, transaction ledger with 10% fee, disputes, admin summary, Helmet and rate limiting.
Payment endpoint is sandbox/internal ledger only. For live money, connect a compliant payment provider server-side, verify webhooks, implement KYC, refunds, payouts and applicable Indian compliance before launch.
