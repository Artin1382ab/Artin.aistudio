# Security, deployment and operations

1. Never execute untrusted installer scripts as an implicit effect of reading SKILL.md.
2. Require explicit approval for destructive changes, public deployments, credential access or financial operations.
3. Check dependency risks, CSP, XSS, CSRF, authz, rate limits and secrets hygiene.
4. Follow safe branching, backup, rollback, CI gates, logging and incident review.
5. Do not expose private API keys, customer records or environment variables in output.
