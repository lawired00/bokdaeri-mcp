<p align="center"><img src="assets/bokdaeri.png" alt="Bokdaeri · 복대리" width="56" height="56"></p>
<h1 align="center">Bokdaeri MCP · 복대리</h1>
<p align="center"><strong>English</strong> · <a href="README.md">한국어 안내</a></p>

<p align="center"><strong>Start a lawyer consultation with your AI assistant.</strong><br>Prepare your request, submit it and check the connection result.</p>

<p align="center"><a href="docs/connecting.md">Connection guide</a> &nbsp; · &nbsp; <a href="https://mcp.bokdaeri.com/consult">Request a consultation</a> &nbsp; · &nbsp; <a href="https://mcp.bokdaeri.com/agents">Agent guide</a></p>

<p align="center"><img src="assets/consultation.webp" alt="A lawyer and a client discussing a consultation across a table" width="720"></p>

## What you can do

Prepare a consultation request from your conversation with an AI assistant, then submit it through Bokdaeri. After submission, check its progress and the assigned lawyer information. You can edit or withdraw a request before a lawyer accepts it.

## Connect

Add this URL in your AI client's **MCP server settings**, then complete the connection approval.

```text
https://mcp.bokdaeri.com/mcp/agent
```

Your client must support remote MCP and OAuth. Supported clients can use dynamic client registration (DCR), without a separate manual registration request.

[Step-by-step setup](docs/connecting.md) · [Compatibility and check scope](docs/compatibility.md)

**Using a browser-capable agent?** It can follow the [agent guide](https://mcp.bokdaeri.com/agents) to use the web application without an MCP connection.

## Try a request

> My rental deposit has not been returned. Help me prepare and submit a Bokdaeri request to speak with a lawyer.

1. **Prepare** — Work with your assistant to describe the situation and your questions.
2. **Review and submit** — Complete phone verification, required consent and final confirmation in Bokdaeri's web flow.
3. **Check the result** — Confirm receipt and wait for the lawyer who accepts your request to contact you.

Drafting a request or verifying a phone number does not submit it. After submission, ask your assistant to check its status or update the details. [Status, editing and withdrawal examples](docs/usage.md)

## Before you use it

- **Fees:** No fee for the first consultation inquiry. Further consultation or representation fees are agreed directly with the lawyer.
- **Information sharing:** Participating lawyers review the consultation details. The contact number is provided to the lawyer who accepts the request.
- **Status:** Results reflect the state at the time of retrieval. Acceptance does not mean a call or consultation has already taken place.

See the [connection guide](docs/connecting.md) and [FAQ](docs/faq.md) for verification requirements, service availability and supported clients.

---

[Official service introduction](https://mcp.bokdaeri.com/ai) · [Official MCP Registry](https://registry.modelcontextprotocol.io/v0.1/servers/com.bokdaeri%2Fconsultation/versions/1.0.1) · [Support](mailto:admin@lawired.co.kr)

[Terms of service](https://mcp.bokdaeri.com/agents/policies/terms) · [Privacy policy](https://mcp.bokdaeri.com/agents/policies/privacy)

This repository contains usage guidance and connection information, not service source code. Do not post consultation details or authentication information in public issues.
