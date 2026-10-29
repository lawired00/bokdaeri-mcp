# FAQ · 자주 묻는 질문

[English](../README.md) · [한국어](../README.ko.md) · [Connection guide](connecting.md)

### Is this a server I install? · 서버를 설치해야 하나요?

No. Bokdaeri operates the remote MCP service. Register the public endpoint in a compatible client. This repository distributes information and connection settings only, with no server source code or self-hosting package.

아닙니다. 복대리가 원격 MCP 서비스를 운영합니다. 지원하는 AI에 연결 주소를 등록하면 됩니다. 이 저장소는 안내와 연결 설정만 제공하며 서버 소스코드나 직접 운영용 설치물을 배포하지 않습니다.

### Can any AI chat use it? · 일반 AI 채팅에서도 바로 되나요?

A client needs remote MCP tools and the required OAuth support. Reading this repository or mentioning Bokdaeri does not automatically install a connector. Browser-agent access is a separate route described in the [official guide](https://mcp.bokdaeri.com/agents).

원격 MCP 도구와 OAuth를 지원해야 합니다. 저장소를 읽거나 “복대리”라고 말하는 것만으로 연결이 설치되지는 않습니다. 브라우저 에이전트 이용은 [공식 안내](https://mcp.bokdaeri.com/agents)의 별도 경로를 참고하세요.

### Which URL do I enter? · 어느 주소를 입력하나요?

Use **`https://mcp.bokdaeri.com/mcp/agent`** as the MCP endpoint. `/agents` is the usage guide and `/consult` is the web consultation service.

MCP 주소는 **`https://mcp.bokdaeri.com/mcp/agent`**입니다. `/agents`는 이용 안내, `/consult`는 웹 상담 신청 서비스입니다.

### Does connecting submit a request? · 연결하면 바로 접수되나요?

No. Connection approval, a prepared draft and phone verification are separate from final submission. Review the details, required consent and fees, then complete the service's confirmation steps.

아닙니다. 연결 승인·상담 초안·번호 인증과 최종 접수는 별개입니다. 내용·필수 동의·비용을 확인한 뒤 서비스의 최종 확인 절차를 진행해야 합니다.

### How much does it cost? · 비용이 있나요?

There is no fee for the first consultation inquiry. Any further consultation or legal representation fees are agreed directly with the lawyer. This is not a promise that all legal services are free.

첫 상담 문의에는 비용이 없습니다. 추가 상담·사건 의뢰 비용은 변호사와 협의합니다. 모든 법률 서비스가 무료라는 뜻은 아닙니다.

### Are overseas numbers supported? · 해외 전화번호도 되나요?

The current verification flow accepts domestic South Korean `010` mobile numbers. International-format or foreign mobile numbers are not supported. Receiving a Korean number's SMS while abroad depends on the carrier and roaming conditions.

현재 인증은 국내 `010` 휴대전화번호를 사용합니다. 국제 형식이나 해외 통신사 번호는 지원하지 않습니다. 한국 번호를 해외에서 사용하는 경우 문자 수신 가능 여부는 통신사·로밍 환경에 따라 달라집니다.

### Does acceptance mean a call has finished? · 수락됐으면 상담까지 끝난 건가요?

No. Acceptance means a lawyer accepted the request. It does not establish that a call took place or that consultation was completed.

아닙니다. 수락은 변호사가 요청을 수락했다는 뜻이며, 실제 통화·상담 완료는 아닙니다.

### Can I see someone else's requests? · 다른 사람의 상담도 볼 수 있나요?

No. Access is limited to your own authorized requests. The public repository does not provide access to consultation records or private lawyer contact data.

본인에게 권한이 있는 상담만 확인할 수 있습니다. 공개 저장소에서 상담 기록이나 비공개 변호사 연락처를 조회할 수 없습니다.

### What if the client says it completed something? · AI가 완료했다고 하면 된 건가요?

Check the actual service result. A prepared draft is not a receipt, and an interrupted or unclear response does not establish failure or success. Check the existing request's state before trying again.

실제 서비스 처리 결과를 확인하세요. 초안은 접수가 아니고, 응답이 끊기거나 불명확하다고 실패·성공을 단정할 수 없습니다. 재시도 전에 기존 상담의 상태부터 확인하세요.

### Will this repository automatically appear in search? · GitHub에 있으면 검색에 바로 나오나요?

A public repository provides another place to discover the service. Search indexing, ranking and automatic use by an AI client depend on those platforms and are not guaranteed. The official MCP Registry and service website are linked from the README.

공개 저장소는 서비스 발견 경로를 늘립니다. 검색 수집·순위·AI의 자동 이용을 보장하지는 않습니다. README에 공식 MCP Registry와 서비스 페이지를 연결해 두었습니다.
