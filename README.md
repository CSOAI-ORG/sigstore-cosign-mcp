# Sigstore Cosign Verification MCP

[![PyPI](https://img.shields.io/pypi/v/sigstore-cosign-mcp)](https://pypi.org/project/sigstore-cosign-mcp/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![MEOK AI Labs](https://img.shields.io/badge/MEOK_AI_Labs-governance--mcp-purple)](https://meok.ai)

Sigstore cosign + rekor transparency log verification for signed container images + git tags + binaries.

## Install

```bash
pip install sigstore-cosign-mcp
```

## Tools

| Tool | Purpose |
|------|---------|
| `verify_image_signature` | Verify cosign signature on container image |
| `query_rekor_log` | Query Rekor transparency log entries |
| `verify_attestation` | Verify in-toto attestation on artifact |
| `check_keyless_identity` | Verify keyless (OIDC) signing identity |
| `list_trusted_certs` | List Fulcio trusted root certificates |

## Pairs with

- `meok-attestation-api` — POST results to https://meok-attestation-api.vercel.app/sign for cryptographically signed compliance certs
- `meok-attestation-verify` — public verification of any MEOK-signed cert
- Other MEOK governance MCPs via SOV3 `mcp_bridge_call`

## Pricing

- **Free**: 10 calls/day. No API key required.
- **Pro** £79/mo: unlimited + signed attestations. [Subscribe](https://buy.stripe.com/14A4gB3K4eUWgYR56o8k836)
- **Enterprise** £1,499/mo: white-label + on-premise + SLA. hello@meok.ai

## Status

Scaffold v1.0.0 ships the MCP framework + 5 tool stubs. v1.1.0 will add real regulation data ingestion.

If your team needs this MCP fully-loaded faster, ping hello@meok.ai for sponsored development.

## License

MIT © MEOK AI Labs
