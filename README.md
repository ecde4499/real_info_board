# 오늘의 진짜 정보판 — T04 카드 3 연결본

실제 측정 기록(`realInfoBoard_v1`)은 그대로 사용합니다. 합성 replay는 별도 상태로 관리하므로 Replay 초기화나 실패 재생이 실제 측정 기록을 지우지 않습니다.

카드 3 정상 순서: Replay 초기화 → D1-A → D1-B → D2
실패 순서: Replay 초기화 → D1-A → D1-B → 실패 5종 중 하나
복구 순서: Replay 초기화 → D1-A → D1-B → 느린 응답 → T04-RECOVER-D2

과제 제공 fixture 9종과 원본 manifest/contract/schema 파일은 `assets/t04-real-information-board/`에 포함되어 있습니다. fixture 값은 HTML에도 내장하여 `file://` 로컬 실행에서도 Replay가 동작합니다.

실제 이틀 증거는 fixture로 대신하지 않습니다. 서로 다른 실제 KST 날짜에 공개 원천을 정상 조회하여 실제 기록 2건을 만들어야 합니다.
