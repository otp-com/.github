<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./otp-logo-dark.svg">
    <img src="./otp-logo-light.svg" alt="otp.com" height="34">
  </picture>
</p>

<p align="center">
  Open-source tools and SDKs for the <a href="https://otp.com">otp.com</a> OTP API:
  send and verify one-time passwords over SMS, WhatsApp, email, and Telegram.
</p>

---

## Repositories

| Repo | What it is |
| --- | --- |
| [**sdk**](https://github.com/otp-com/sdk) | The OpenAPI contract (source of truth). The SDKs generate from it. |
| [**mcp**](https://github.com/otp-com/mcp) | MCP server: plug the OTP API into your own AI system with your API key. |
| [**sdk-node**](https://github.com/otp-com/sdk-node) | Official Node.js / TypeScript client. |
| [**sdk-php**](https://github.com/otp-com/sdk-php) | Official PHP client. |
| [**sdk-go**](https://github.com/otp-com/sdk-go) | Official Go client. |
| [**sdk-python**](https://github.com/otp-com/sdk-python) | Official Python client. |

## Get started

1. Create an account and an API key at [otp.com](https://otp.com).
2. Pick your language SDK above, or wire the [MCP server](https://github.com/otp-com/mcp) into your
   AI agent.
3. Two calls: **send** a code, then **verify** what the user entered. The code is never returned by
   the API.

## Contributing & security

- Contributions welcome; see each repo's `CONTRIBUTING.md`.
- Found a vulnerability? Please **don't** open a public issue; see [SECURITY.md](../SECURITY.md).
