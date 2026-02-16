# PlanExplorer PX — Premiere Pro UXP Extension (Scaffold)

This repository contains an initial scaffold for a Premiere Pro UXP panel extension with a backend and admin approval flow. The scaffold is a starting point for development and includes: 

- server/: Node.js + Express backend (Google OAuth PKCE loopback starter, pending → approve flow, JWT issuance)
- admin/: Minimal React admin UI (list pending users, Approve/Reject)
- plugin/: UXP panel scaffold (React + Spectrum recommended)
- .github/workflows/ci.yml: CI template (build / package placeholders)
- .env.example: example environment variables

Important: This scaffold is intentionally minimal. You must add required secrets/environments before running in production. See server/README.md and plugin/README.md for local run instructions.

## Next steps
1. Add Google OAuth credentials (GOOGLE_CLIENT_ID, GOOGLE_CLIENT_SECRET).
2. Add admin credentials (ADMIN_EMAIL, ADMIN_PASSWORD) to repo secrets or .env for local dev.
3. Run the server and admin locally, then load the plugin using UXP Developer Tool for testing.

