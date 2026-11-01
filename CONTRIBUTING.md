# Contributing to TubeKeel

Thank you for helping build a creator-owned video ecosystem.

## Before you start

1. Read the README of the repository you want to contribute to.
2. Read `keel-spec` RFC-0001 for the protocol direction.
3. For large changes, open a discussion or RFC before writing code.
4. For security issues, do not open a public issue. See `SECURITY.md`.

## Workflow

1. Fork the repository or create a branch if you have write access.
2. Keep the change focused. One logical change per pull request.
3. Run the repository checks and add or update tests. Python repos run `ruff` and `pytest`; Go repos run `gofmt`, `go vet`, and `go test`; `keel-core` database tests need `TUBEKEEL_TEST_DATABASE_URL` and `go test -p 1 ./...`; the web repo runs `npm test`, `npm run typecheck`, `npm run build`, and `npm run format:check`, with `npm run test:e2e` for watch/player changes; spec changes run `python scripts/validate_schemas.py`.
4. Update documentation when behavior changes.
5. Sign off every commit with the Developer Certificate of Origin (DCO). Web-interface commits must also use the sign-off option:

```sh
git commit -s -m "feat: add video manifest endpoint"
```

Do not add a CLA. Do not commit secrets, credentials, private governance documents, or customer data. Pull requests that fail formatting, tests, schema validation, or build checks are not mergeable once required checks are enabled.

## Review

- Protected branches require a pull request and at least one approval; some repos require two.
- CODEOWNERS review is required for protected paths.
- Main is linear; rebase rather than merge.
- A maintainer may close a PR that is out of scope, unsafe, or unmaintainable.

## Access

Contributors are added to a repository-specific `*-contributors` team. Organization membership alone does not grant repository write access. Do not ask for org-wide write.

## Licensing

- Code repositories: AGPL-3.0.
- Spec, RFCs, and public docs: CC-BY-4.0.
- SDKs: Apache-2.0.
- By contributing, you agree that your contribution is licensed under the repository's license and that you have the right to submit it.
