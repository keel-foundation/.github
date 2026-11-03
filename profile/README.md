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
- [`keel-core`](https://github.com/keel-foundation/keel-core) — API, domain, and media worker.
- [`keel-moderation`](https://github.com/keel-foundation/keel-moderation) — moderation and content protection.
- [`keel-docs`](https://github.com/keel-foundation/keel-docs) — public documentation.

Media ingest, scanning, transcoding, and HLS packaging now live in `keel-core` (`cmd/worker`);
there is no separate pipeline repository.

### Private repositories

These repositories are maintainer-only while the project is pre-alpha:

- `keel-web` — viewer, creator studio, Cases & appeals, and the versioned video editor. Private until the maintainer pool is established.
- `keel-governance` — Constitution, whitepaper, board, finance, and legal records.
- `keel-infra` — production infrastructure, environments, and runbooks.
- `keel-security` — threat model, incident response, and audits.
- `keel-branding` — brand system, source assets, and decisions.

The Constitution and whitepaper are not public until ratification.

## Status

Pre-alpha. The local creator-appeal demo is working: a synthetic automated signal, a case, an
enforcement action, an independent appeal review, and an append-only hash-chained ledger with
verification and export.

`keel-core` is PostgreSQL-backed with pgvector and implements identity and sessions, catalog and
discovery, subscriptions, comments, reactions, saves, watch history, creator uploads, FFmpeg/HLS
processing in a separate media worker, watch telemetry, creator analytics, and creator
notifications. `keel-moderation` provides creator-scoped cases, actions, appeals, and ledger reads
with reviewer independence. The web client is private and maintainer-only; it is fully built
against local mock data and wiring it to these APIs is the next integration step.

Federation, payouts, production OIDC/social providers, and the staff moderation portal are not
implemented yet.

Start with [`keel-dev`](https://github.com/keel-foundation/keel-dev) for the local demo, [`keel-docs`](https://github.com/keel-foundation/keel-docs) for creator and developer guidance, and [`keel-spec`](https://github.com/keel-foundation/keel-spec) for RFC-0001 and the schemas.
