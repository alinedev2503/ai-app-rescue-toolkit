# 2 — Secrets and database rules

## Secrets

- [ ] Search the repo (including history if available) for key patterns:
      `AIza`, `sk-`, `gho_`, `sk_live_`, `AKIA`, `service_account`, `private_key`.
- [ ] Check `.env.example` for real-looking values — examples must be placeholders.
- [ ] Check client-side bundles for keys that should be server-side only.
- [ ] Move Gemini / OpenAI / payment secrets to a server proxy or host secrets.
- [ ] Keep only public identifiers in `VITE_*` / `NEXT_PUBLIC_*` variables.
- [ ] Confirm `.gitignore` covers `.env`, credentials folders and local data.
- [ ] Tell the client which keys were exposed so they can **rotate** them.
- [ ] Never ask a client to paste a key in chat or e-mail.

## Database rules

- [ ] Firestore / Supabase rules are not in "allow all" mode.
- [ ] Auth required where user data is read or written.
- [ ] Per-user document ownership enforced (auth.uid / RLS policy).
- [ ] Admin-only collections blocked from client writes.
- [ ] Storage bucket rules restrict uploads by type and size.
- [ ] Rules tested with an unauthenticated request and with a second test user.

## Other common leaks

- [ ] Error responses do not include stack traces or credentials.
- [ ] Logs do not print request bodies containing personal data.
- [ ] CORS allows only the expected origins.
