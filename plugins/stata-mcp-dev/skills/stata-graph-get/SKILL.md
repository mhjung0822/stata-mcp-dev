---
name: stata-graph-get
description: "/stata-graph-get 전용 — getGraphSpec 로 현재 그래프의 spec 을 조회 (해석 없음). 자연어 요청에는 쓰지 않음."
---

# stata-graph-get

`/stata-graph-get` 호출 시:

1. `StataMCP:getGraphSpec`을 빈 문자열(`name=""`)로 호출하여 현재 그래프 spec 조회
2. 결과 JSON을 코드 블록으로 감싸서 그대로 반환
3. 에러 발생 시 에러 메시지를 코드 블록으로 감싸서 그대로 반환

인자를 받지 않으며, 결과를 수정·정제·평가하지 말 것. 코드 블록 앞뒤에 어떠한 설명도 추가하지 말 것.
