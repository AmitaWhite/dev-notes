# 템플릿

| 파일 | 용도 |
| --- | --- |
| `templates/01-self-check.md` | 주기적으로 실력을 점검하는 체크리스트 |
| `templates/02-screen-flow.md` | 화면 하나의 흐름을 API부터 테이블까지 추적 |
| `templates/03-query-analysis.md` | 긴 SQL 쿼리를 단계별로 읽고 정리 |
| `templates/04-glossary.md` | 테이블·컬럼 약어와 용어 사전 (누적형) |
| `templates/05-method-names.md` | 메서드명·DTO 이름 해석과 계층별 정리 (누적형) |
| `templates/06-feature-analysis.md` | 기능 하나의 입력·출력·처리 순서 분석 |
| `templates/07-daily-note.md` | 하루 작업 기록과 질문 목록 |

## 사용법

템플릿을 복사해서 각자의 노트 폴더에서 채워 쓴다.

```
notes/
  glossary.md          <- 04, 하나만 두고 계속 추가
  method-names.md      <- 05, 하나만 두고 계속 추가
  self-check.md        <- 01, 회차별로 칸 채우기
  daily/               <- 07, 날짜별로 복사
  screens/             <- 02, 화면별로 복사
  queries/             <- 03, 쿼리별로 복사
  features/            <- 06, 기능별로 복사
```

추천 순서:

1. 분석할 화면 하나를 고른다.
2. `02-screen-flow`로 사용자 행동, API, 백엔드, 테이블을 연결한다.
3. 핵심 쿼리 하나를 `03-query-analysis`로 읽는다.
4. 낯선 이름은 그때그때 `glossary.md`, `method-names.md`에 추가한다.
5. `06-feature-analysis`로 기능 하나를 한 장에 요약한다.
6. 하루를 마칠 때 `07-daily-note`를 쓴다.

## 원칙

- 이 저장소에는 일반적인 내용만 둔다. 특정 회사나 프로젝트의 코드, 데이터, 내부 정보는 올리지 않는다.
- 예제가 필요하면 게시판, 주문, 회원처럼 일반적인 이름을 쓴다.
