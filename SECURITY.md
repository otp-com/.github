# Security Policy

We take the security of otp.com and everything under this organization seriously.

## Reporting a vulnerability

**Please do not report security vulnerabilities through public GitHub issues.**

Email **security@otp.com** with:

- a description of the issue and its impact,
- steps to reproduce (a proof of concept if you have one),
- affected repo / version.

You'll get an acknowledgement within **2 business days** and a status update within **5 business
days**. Please give us reasonable time to investigate and ship a fix before any public disclosure;
we're happy to credit you once it's resolved.

## Scope

These repos are clients of the OTP API (SDKs, the MCP server, the contract). Report issues in the
client code here; report issues in the hosted API or your account directly to security@otp.com.

## Handling API keys

Never commit API keys. All tools here read your key from the environment or configuration at
runtime; keep `otp_live_…` keys out of source control, logs, and screenshots.
