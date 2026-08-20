# KaamSetu Live Deployment

## Fastest route
1. Create a Git repository and upload this folder.
2. Create a web service on a Docker-compatible host.
3. Set:
   - `JWT_SECRET` = a long random secret
   - `PLATFORM_FEE_PERCENT` = `10`
   - `PAYMENT_MODE` = `sandbox` until payment webhooks are configured.
4. Deploy and open `/api/health`.
5. Add your custom domain in the hosting dashboard and enable HTTPS.

## Before real money
Do not switch to live payments just by changing an environment variable. Add your chosen payment provider's server-side order API, signature/webhook verification, refund handling, payout workflow, reconciliation, KYC and applicable Indian compliance. Keep all payment secrets server-side.

## Database
This starter uses SQLite for simplicity. For a serious multi-user launch, move to a managed PostgreSQL database and add automated backups/migrations before onboarding significant traffic.
