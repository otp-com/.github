<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./otp-logo-dark.svg">
    <img src="./otp-logo-light.svg" alt="otp.com" height="34">
  </picture>
</p>

<p align="center">
  Official tools and SDKs for the <a href="https://otp.com">otp.com</a> OTP API:
  send and verify one-time passwords over SMS, WhatsApp, email, and Telegram.
</p>

---

## Repositories

| Repo | What it is |
| --- | --- |
| [**sdk**](https://github.com/otp-com/sdk) | The OpenAPI contract (source of truth). The SDKs generate from it. |
| [**mcp**](https://github.com/otp-com/mcp) | MCP server: plug the OTP API into your own AI system with your API key. |

### Server-side

Generated from the contract and MIT licensed. They authenticate with a **server key**, which never
leaves your backend.

| Repo | What it is |
| --- | --- |
| [**sdk-node**](https://github.com/otp-com/sdk-node) | Official Node.js / TypeScript client. |
| [**sdk-php**](https://github.com/otp-com/sdk-php) | Official PHP client. |
| [**sdk-go**](https://github.com/otp-com/sdk-go) | Official Go client. |
| [**sdk-python**](https://github.com/otp-com/sdk-python) | Official Python client. |

### Mobile

A drop-in verification screen, or a headless core if you want your own. They ship as binaries under a
commercial licence and authenticate with a **publishable key**, which is designed to sit inside your
app. A verification returns a short-lived token rather than a result, because an answer read off a
device you do not control is not proof; your backend exchanges that token with its server key.

| Repo | What it is |
| --- | --- |
| [**sdk-ios**](https://github.com/otp-com/sdk-ios) | Official iOS SDK, via Swift Package Manager or CocoaPods. |
| [**sdk-android**](https://github.com/otp-com/sdk-android) | Official Android SDK, from Maven Central. |
| [**sdk-react-native**](https://github.com/otp-com/sdk-react-native) | Official React Native SDK, a bridge over the two above. |
| [**sdk-flutter**](https://github.com/otp-com/sdk-flutter) | Official Flutter SDK, from pub.dev, a bridge over the two above. |

## Get started

1. Create an account at [otp.com](https://otp.com) and take the keys you need: a **server key** for
   your backend, plus a **publishable key** if you are shipping one of the mobile SDKs.
2. Pick your SDK above, or wire the [MCP server](https://github.com/otp-com/mcp) into your AI agent.
3. From a server, two calls: **send** a code, then **verify** what the user entered. From a device,
   the SDK verifies and hands you a token your backend **exchanges** for the result. Either way the
   code itself is never returned by the API.

## Contributing & security

- Contributions welcome on the open-source repos; see each one's `CONTRIBUTING.md`. The mobile repos
  carry no source, so issues there are the way in.
- Found a vulnerability? Please **don't** open a public issue; see [SECURITY.md](../SECURITY.md).
