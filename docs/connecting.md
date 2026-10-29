# 복대리 연결 방법

[처음으로](../README.md) · [English](en/connecting.md)

## 연결 주소

사용 중인 AI 서비스의 MCP 서버 추가 설정에 아래 주소를 입력하세요.

```text
https://mcp.bokdaeri.com/mcp/agent
```

- **전송 방식:** Streamable HTTP
- **인증 방식:** OAuth Authorization Code + PKCE
- **클라이언트 등록:** DCR 지원 클라이언트는 별도의 사전 등록 요청 없이 자동 등록

[지원 환경과 확인 범위](compatibility.md) · [인증 서버 메타데이터](https://mcp.bokdaeri.com/.well-known/oauth-authorization-server)

## 연결 순서

1. AI 서비스에서 원격 MCP 또는 사용자 지정 연결 설정을 엽니다.
2. 위 MCP 주소를 입력하고, 전송 방식 항목이 있으면 Streamable HTTP를 선택합니다.
3. 클라이언트가 연 브라우저에서 OAuth 연결 승인을 진행합니다.
4. 복대리 도구가 표시되는지 확인합니다.

연결을 마쳤다면 AI에 상담 내용 준비를 요청하세요. 상담 신청은 복대리 웹 화면에서 번호 인증·필수 동의·최종 확인을 마친 뒤 완료됩니다. 연결 승인만으로 상담이 접수되지는 않습니다.

연결 설정에 문자 인증번호나 토큰을 넣지 마세요. 수동 사전 등록 방식을 사용하는 제품은 해당 제품의 연결 구성이 필요합니다.

## Claude Code

다음 명령으로 복대리 연결을 추가합니다.

```text
claude mcp add --transport http bokdaeri https://mcp.bokdaeri.com/mcp/agent
```

이후 Claude Code에서 `/mcp`를 열어 복대리를 선택하고 OAuth 인증을 진행합니다. 이 명령은 연결 설정만 추가하며, 복대리 서버를 설치하거나 상담을 신청하지 않습니다.

[설정 파일 예제](../config/claude-code.mcp.json)에는 서버 이름·전송 방식·공개 주소만 들어 있습니다. 기존 MCP 설정이 있다면 파일 전체를 덮어쓰지 말고 복대리 항목만 추가하세요. 메뉴 이름은 버전에 따라 다를 수 있습니다.

[Claude Code 공식 MCP 안내](https://code.claude.com/docs/en/mcp)

## 다른 AI 서비스와 웹 이용

원격 MCP와 해당 OAuth 흐름을 지원하는 제품에서 같은 주소를 사용합니다. 제품별 메뉴·권한·연결 방식은 다를 수 있으며, 이 문서가 각 플랫폼의 등록·심사 완료를 뜻하지는 않습니다.

MCP 연결을 지원하지 않으면 [웹 상담 신청](https://mcp.bokdaeri.com/consult)을 이용하세요. **브라우저를 조작하는 에이전트는 MCP 연결이나 사전 클라이언트 등록 없이** [에이전트 이용 안내](https://mcp.bokdaeri.com/agents)에서 신청을 시작할 수 있습니다. 번호 인증·필수 동의·최종 확인은 동일하게 필요합니다.
