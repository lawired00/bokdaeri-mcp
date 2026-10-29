# Connect to Bokdaeri · 복대리 연결 방법

[English overview](../README.en.md) · [한국어 소개](../README.ko.md) · [Compatibility](compatibility.md)

## Connection details · 연결 정보

| Field / 항목 | Value / 값 |
| --- | --- |
| Name / 이름 | Bokdaeri / 복대리 |
| MCP server URL / 연결 주소 | `https://mcp.bokdaeri.com/mcp/agent` |
| Transport / 전송 방식 | Streamable HTTP |
| Authentication / 인증 | OAuth Authorization Code with PKCE |
| Authorization server / 인증 서버 | `https://mcp.bokdaeri.com` |
| OAuth discovery / 인증 정보 발견 | `https://mcp.bokdaeri.com/.well-known/oauth-authorization-server` |
| Official guide / 공식 안내 | `https://mcp.bokdaeri.com/agents` |

## Add the remote service

1. Open the client's remote MCP server or custom connection settings.
2. Add the MCP server URL above and select Streamable HTTP where a transport is requested.
3. Complete the OAuth connection approval in the browser opened by the client. DCR-capable clients can register automatically; manually pre-registered clients require a separate supported setup.
4. Confirm that Bokdaeri's tools are available. A successful connection is not a submitted consultation.
5. Ask the assistant to prepare your request. Complete the phone verification, required consent and final confirmation requested by Bokdaeri.

Do not paste a phone verification code or access token into the connection settings. The public MCP URL does not contain a credential.

## 일반 연결 순서

1. AI 서비스에서 원격 MCP 또는 사용자 지정 연결 설정을 엽니다.
2. 위 MCP 주소를 입력하고, 전송 방식 항목이 있으면 Streamable HTTP를 선택합니다.
3. 클라이언트가 연 브라우저에서 OAuth 연결 승인을 진행합니다. DCR 지원 클라이언트는 자동 등록이 가능하며, 수동 사전 등록 방식의 제품은 해당 연결 구성이 필요합니다.
4. 복대리 도구가 표시되는지 확인합니다. 연결됐다는 것과 상담이 접수됐다는 것은 다릅니다.
5. AI에 상담 내용 준비를 요청하고, 복대리 웹 확인 흐름의 번호 인증·필수 동의·최종 제출을 진행합니다.

연결 설정에 문자 인증번호나 토큰을 붙여 넣지 마세요. 공개 연결 주소에는 자격증명이 포함되지 않습니다.

## Claude Code

For a client with Claude Code's HTTP configuration format, the public configuration is in [config/claude-code.mcp.json](../config/claude-code.mcp.json). It contains only the server name, transport and public URL.

Claude Code의 원격 HTTP 연결 명령은 다음과 같습니다. 명령은 서비스 연결 설정을 추가하며, 복대리 서버를 설치하거나 상담을 신청하지 않습니다.

```text
claude mcp add --transport http bokdaeri https://mcp.bokdaeri.com/mcp/agent
```

Then open `/mcp` in Claude Code, select Bokdaeri and follow the OAuth authentication flow. Menu labels can vary by client version. In a project that already has MCP configuration, merge the Bokdaeri entry instead of overwriting existing connections.

이후 Claude Code에서 `/mcp`를 열어 복대리를 선택하고 OAuth 인증을 진행합니다. 메뉴 이름은 버전에 따라 다를 수 있습니다. 기존 MCP 설정이 있으면 파일 전체를 덮어쓰지 말고 복대리 항목만 추가하세요.

[Claude Code's official MCP instructions](https://code.claude.com/docs/en/mcp)

## Other clients · 다른 클라이언트

Use the same URL only where the product supports remote MCP and the required OAuth flow. Read the [compatibility notes](compatibility.md) before assuming support. This configuration is not a universal installer for ChatGPT, Claude web, Gemini, Dot or Hermes.

원격 MCP와 해당 OAuth 흐름을 지원하는 제품에서 같은 주소를 사용합니다. ChatGPT·Claude 웹·Gemini·Dot·Hermes의 메뉴·권한·연결 방식이 모두 같지는 않습니다. 제품별 연결이나 플러그인 심사 상태를 이 문서가 바꾸지는 않습니다.

If your client cannot use MCP, open the [web consultation service](https://mcp.bokdaeri.com/consult) directly. A browser-capable agent can consult the [official browser-agent guide](https://mcp.bokdaeri.com/agents); browser automation support is separate from MCP support.

MCP 연결을 지원하지 않으면 [웹 상담 신청](https://mcp.bokdaeri.com/consult)을 이용할 수 있습니다. 브라우저 조작 에이전트는 [공식 이용 안내](https://mcp.bokdaeri.com/agents)를 참고하세요. 브라우저 조작 기능과 MCP 연결 지원은 별개입니다.
