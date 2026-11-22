# Security

DHRUV is a student prototype built for Smart India Hackathon 2026 and is not an official NCPOR, MoES or Government of India service.

Report vulnerabilities privately through GitHub's "Report a vulnerability" option on the Security tab, not a public issue.

Design points worth knowing about:
- Public pages read only published items, enforced by Postgres row-level security.
- Staff actions are written to an audit log, and a post needs approval from a second staff member before it is published.
- `.env.local` holds the Supabase service-role key and AI keys. It is git-ignored; never commit it.
- `PRODUCTION_PLAN.md` lists what a real deployment would still need (rate limiting, backups, a security review).
