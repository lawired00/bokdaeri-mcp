# Connect to Bokdaeri

[Overview](../../README.en.md) · [한국어](../connecting.md)

## Connection URL

Enter this URL in your AI client's remote MCP server settings.

```text
https://mcp.bokdaeri.com/mcp/agent
```

- **Transport:** Streamable HTTP
- **Authentication:** OAuth Authorization Code + PKCE
- **Client registration:** DCR-capable clients can register automatically without a separate manual pre-registration request.

[Compatibility and check scope](compatibility.md) · [Authorization server metadata](https://mcp.bokdaeri.com/.well-known/oauth-authorization-server)

## Connection steps

1. Open the client's remote MCP or custom connection settings.
2. Add the URL above and select Streamable HTTP if a transport is requested.
3. Complete the OAuth connection approval in the browser opened by the client.
4. Confirm that Bokdaeri's tools are available.

Then ask your assistant to prepare a consultation request. Submission is completed after phone verification, required consent and final confirmation in Bokdaeri's web flow. Connection approval alone does not submit a consultation.

Do not put verification codes or tokens into connection settings. Products using manual client registration require their supported connection setup.

## Claude Code

Add the connection with:

```text
claude mcp add --transport http bokdaeri https://mcp.bokdaeri.com/mcp/agent
```

Then open `/mcp`, select Bokdaeri and follow the OAuth flow. This command adds a connection; it does not install the Bokdaeri server or submit a consultation.

The [configuration example](../../config/claude-code.mcp.json) contains only the server name, transport and public URL. If you already have MCP configuration, merge the Bokdaeri entry instead of overwriting existing connections. Menu labels may vary by version.

[Official Claude Code MCP instructions](https://code.claude.com/docs/en/mcp)

## Other AI clients and web access

Use the same URL in products supporting remote MCP and the required OAuth flow. Menus, permissions and connection methods vary. This guide does not establish listing or review approval by any platform.

If MCP is unavailable, use the [web consultation service](https://mcp.bokdaeri.com/consult). **A browser-capable agent can start without an MCP connection or prior client registration** by following the [agent guide](https://mcp.bokdaeri.com/agents). Phone verification, required consent and final confirmation still apply.
