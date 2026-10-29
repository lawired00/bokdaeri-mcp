# Compatibility and check scope

[Overview](../../README.en.md) · [한국어](../compatibility.md)

The connection checks below were performed on 2026-10-28. They describe specific capabilities, not a guarantee for every version, AI model or product account. This documentation package was prepared on 2026-10-29.

| Client | Checked | Scope |
| --- | --- | --- |
| Claude Code 2.1.220 | OAuth connection, token refresh, authenticated tool discovery | Hosted-service connection checked; no live consultation or message sent in this check |
| MCP Inspector 2.12.0 | Remote initialization and public tool discovery | Discovery check, not proof of the complete consultation flow |
| Official MCP Client SDK 2.3.1 | New DCR registration, PKCE OAuth, authenticated discovery and revocation | New hosted connection checked; no consultation tools executed |
| DCR/Claude Code isolated workflow checks | Authentication and consultation-management permission boundaries | Synthetic local data and simulated delivery; not real legal requests |
| Google/Gemini | Product-specific integration remains unverified | This page is not a Google listing or approval claim |
| Other MCP clients | Requires remote MCP and compatible OAuth | No blanket compatibility claim |

Browser automation by Dot, Hermes or similar agents is a separate usage route. A successful browser-agent test does not prove that the product supports this remote MCP connection. Conversely, a missing browser tool does not mean an MCP connection is unavailable. Follow the client's actual capabilities and the [official guide](https://mcp.bokdaeri.com/agents).

OAuth discovery and DCR support do not establish Google-specific account-linking compatibility. The platform's client registration, callback and token-refresh behavior still require a product-specific check. No change to existing security or other channels is implied by this documentation.
