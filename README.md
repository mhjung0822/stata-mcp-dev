# stata-mcp-dev

Stata MCP 의 **개발용(베타)** 배포입니다. 시험 빌드가 수시로 올라옵니다. 정식 배포는 [mhjung0822/stata-mcp](https://github.com/mhjung0822/stata-mcp).

현재 빌드: `0.14.1-dev.202611170834` · 서버 `0.14.0`

정식보다 먼저 나가는 시험 빌드입니다. 구조(드론 · ado · 스킬 · Go 서버)는 정식과 같습니다.

## 설치

Stata 에서:

```
net install stata-mcp, from("https://raw.githubusercontent.com/mhjung0822/stata-mcp-dev/main/release") replace
mcp_setup
```

`mcp_setup` 이 도움말 자료와 서버 실행 파일을 받아 둡니다 (서버는 `~/.stata_mcp/bin/`). 이후 갱신은 `mcp_setup, update`.

Claude 에서: 마켓플레이스 `mhjung0822/stata-mcp-dev` 를 추가해 `stata-mcp-dev` 플러그인을 켭니다 (정식 `stata-mcp` 플러그인은 끕니다).

정식으로 돌아가려면 정식 주소로 다시 `net install … replace` 한 뒤 `mcp_setup` 을 실행합니다. 베타 판이 정식보다 높으면 서버 실행 파일은 그대로 남습니다 — `~/.stata_mcp/bin/` 의 두 파일을 지우고 다시 `mcp_setup`.
