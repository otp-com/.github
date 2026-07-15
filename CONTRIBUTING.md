# Contributing

Thanks for helping improve the otp.com open-source tools!

## Ground rules

- **Be kind.** By participating you agree to our [Code of Conduct](./CODE_OF_CONDUCT.md).
- **One focused change per PR.** Keep diffs small and reviewable.
- **Tests + lint green** before you open a PR (see the repo's README for its commands).
- **Never commit secrets.** No real API keys, tokens, or credentials; use placeholders.

## The SDKs are generated

`sdk-node`, `sdk-php`, `sdk-go`, and `sdk-python` are generated from the OpenAPI spec in
[`otp-com/sdk`](https://github.com/otp-com/sdk). **Don't hand-edit generated client code**: it will
be overwritten on the next regeneration. For an API-surface change, open a PR against `otp-com/sdk`
(`openapi.yaml`); the SDKs regenerate from it. Bug fixes in generator config, templates, hand-written
helpers, docs, or CI are always welcome directly in the SDK repos.

## Workflow

1. Fork and branch from `main`.
2. Make your change; add or update tests.
3. Run the repo's lint + test.
4. Open a PR with a clear description of what and why.

## Reporting bugs / security

- Bugs: open an issue with steps to reproduce.
- Vulnerabilities: **not** a public issue; see [SECURITY.md](./SECURITY.md).
