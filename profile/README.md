# KeelTube

**An even keel for creators.**

KeelTube is an open, federated video protocol built around creator ownership, real due process, content protection, and transparent payouts.

## What we are building

- **Creator-owned:** your archive, your audience relationship, your data, and a real exit.
- **Moderation-first:** specific reasons, human review before irreversible harm, real appeals, and published error rates.
- **Protected:** piracy, impersonation, spam, scams, and fraud are treated as serious harms.
- **Federated:** PeerTube-compatible where possible; no single instance is the only gateway.

## Repositories

- [`keel-dev`](https://github.com/keel-foundation/keel-dev) — start here for local development.
- [`keel-spec`](https://github.com/keel-foundation/keel-spec) — protocol, RFCs, schemas.
- [`keel-core`](https://github.com/keel-foundation/keel-core) — API and domain.
- [`keel-pipeline`](https://github.com/keel-foundation/keel-pipeline) — media pipeline.
- [`keel-web`](https://github.com/keel-foundation/keel-web) — viewer and creator studio.
- [`keel-moderation`](https://github.com/keel-foundation/keel-moderation) — moderation and content protection.
- [`keel-docs`](https://github.com/keel-foundation/keel-docs) — public documentation.

Governance, production infrastructure, and security operations are maintained in private repositories. The Constitution and whitepaper are not public until ratification.

## Status

Pre-alpha. The local creator-appeal demo is working: a synthetic automated signal, a case, an enforcement action, an independent appeal review, and an append-only hash-chained ledger with verification and export. A PostgreSQL-backed core read API and a fully built web preview (feed, watch, channels, search, library, creator studio, and moderation console) are also working. Upload, transcoding, HLS, subscriptions, federation, payouts, content protection, and the production moderation console are not implemented yet.

Start with [`keel-dev`](https://github.com/keel-foundation/keel-dev) for the local demo, [`keel-docs`](https://github.com/keel-foundation/keel-docs) for creator and developer guidance, and [`keel-spec`](https://github.com/keel-foundation/keel-spec) for RFC-0001 and the schemas.
