# 메서드명 해석표

이 파일은 하나만 두고 계속 추가한다.

긴 메서드명은 **동사 + 대상 + 형태**로 끊어 읽는다.
예: `selectCustomerAllowanceList` = select(조회) + CustomerAllowance(고객 수당) + List(목록)

같은 이름이 Controller, Service, Mapper에 거의 그대로 이어지는 경우가 많다.
하나를 찾으면 VS Code에서 `Shift+F12`(참조 찾기)로 나머지를 따라간다.

## 참고: 흔한 동사 (앞부분)

| 동사 | 뜻 | SQL |
| --- | --- | --- |
| `select`, `get`, `find`, `search`, `retrieve` | 조회 | SELECT |
| `insert`, `save`, `create`, `add`, `register` | 등록 | INSERT |
| `update`, `modify`, `change` | 수정 | UPDATE |
| `delete`, `remove` | 삭제 | DELETE (또는 `DEL_YN` UPDATE) |
| `merge`, `upsert`, `saveOrUpdate` | 있으면 수정, 없으면 등록 | MERGE |
| `check`, `validate`, `is`, `exists` | 검사, 여부 확인 | 보통 COUNT |
| `count` | 건수 | COUNT |
| `process`, `handle`, `execute` | 여러 단계를 묶은 처리 (Service에 많음) | 여러 개 |
| `convert`, `to`, `make`, `build` | 데이터 모양 바꾸기 | 없음 |

## 참고: 흔한 형태 (끝부분)

| 끝부분 | 뜻 |
| --- | --- |
| `List` | 여러 건 (목록 화면) |
| `Detail`, `Info`, `One` | 한 건 (상세 화면) |
| `Count`, `TotalCount` | 전체 건수 (페이징) |
| `ByXxx` | Xxx 조건으로 (`selectUserById`) |
| `Excel`, `Download` | 엑셀 다운로드용 |
| `Popup`, `Combo`, `Code` | 팝업, 콤보박스, 코드 목록용 |

## 참고: DTO 이름 끝부분

| 끝부분 | 용도 |
| --- | --- |
| `Req`, `Request`, `Param`, `Condition` | 들어오는 값 (검색 조건, 등록·수정 값) |
| `Res`, `Response`, `Result`, `Vo` | 나가는 값 (목록 한 줄, 상세) |

## 내가 본 메서드 (계층별로 같은 줄에)

| Controller | Service | Mapper | 한 줄 뜻 |
| --- | --- | --- | --- |
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |
