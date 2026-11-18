# 3 — Deployment

## Common causes of "works in preview, breaks in production"

- [ ] Environment variables missing or named differently on the host.
- [ ] Build command / output directory wrong (`dist`, `.next`, `build`).
- [ ] SPA routes return 404 on refresh — add a rewrite to `index.html`.
- [ ] Server endpoints assumed to exist on a static host — add a proxy or move to a server host.
- [ ] Case-sensitive imports break on Linux (works on macOS/Windows).
- [ ] Mixed content: HTTP API called from an HTTPS page.
- [ ] API key restricted by referrer and the production domain not allowlisted.
- [ ] Free-tier sleep / cold start mistaken for an outage.

## Vercel

- [ ] Project linked to the right repo and branch.
- [ ] Build command and output directory verified.
- [ ] Env vars set for Production, Preview and Development as needed.
- [ ] `vercel.json` rewrites checked for client-side routing.
- [ ] Deployment logs read after a fresh deploy.

## Firebase

- [ ] `firebase.json` hosts config points to the correct public folder.
- [ ] Rewrites configured for SPA fallback.
- [ ] Functions deployed (if used) and region noted.
- [ ] Firestore rules and indexes deployed together with the app.

## Replit

- [ ] Correct run command and port binding (`0.0.0.0`).
- [ ] Always-on / deployment configuration confirmed with the client.
- [ ] Secrets stored in Replit secrets, not in files.

Output of this step: a live URL, verified in a clean browser session.
