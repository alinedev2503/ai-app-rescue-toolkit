# AI App Rescue Toolkit

Checklists and small scripts used to debug, secure and deploy web apps that were
generated with AI tools (Google AI Studio, Replit, Lovable, Bolt, v0) or that
break when moved from preview to production.

> Portfolio repository for **Upwork Project D — AI-generated app fixed and deployed**.
> This repository contains **methodology only**. It is not a fabricated client
> case study. Screenshots used in the portfolio come from real apps.

---

## Service tiers

| Tier | Scope |
|---|---|
| **Quick Fix** | 1 critical bug or deployment issue |
| **Audit and Fix** | Review, up to 5 fixes, API keys and database rules secured, deployed |
| **Full Rescue** | Deeper review, key module refactoring, performance tips, documentation |

Source code is returned in every tier. Responsive design, design customization
and content upload are intentionally out of scope for this service.

---

## Process

1. **Access and review** — get the repo link or an invite, reproduce the problem,
   confirm the scope before starting.
2. **Fix** — fix only what is needed, then secure keys and database rules.
3. **Test and deploy** — test the main flows, deploy to Vercel / Firebase / Replit.
4. **Handover** — notes on every change and why it was made.

## Checklists

- [checklists/01-access-and-repro.md](checklists/01-access-and-repro.md)
- [checklists/02-secrets-and-rules.md](checklists/02-secrets-and-rules.md)
- [checklists/03-deployment.md](checklists/03-deployment.md)
- [checklists/04-performance.md](checklists/04-performance.md)
- [checklists/05-handover.md](checklists/05-handover.md)

A client never needs to paste an API key in chat. Exposed keys are moved to
server-side settings and then rotated by the client.

## Rules of engagement

- No full rewrite unless the Full Rescue tier was hired.
- If the review shows a larger scope, tell the client before starting.
- No invented before/after numbers and no fake client screenshots.
