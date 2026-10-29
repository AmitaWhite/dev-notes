# SI 현장 분석 노트 템플릿

현장 코드와 업무를 이해하기 위한 빈 템플릿 모음이다.
템플릿을 복사해서 내 노트 폴더(Private-memo 등)에 채워 나간다.

## 보안 규칙 (가장 중요)

- 이 저장소에는 **빈 템플릿만** 둔다. 실제 테이블명, 코드, 데이터, 고객사 정보는 절대 넣지 않는다.
- 현장(VDI)에서는 **받기만** 한다. `git clone` 또는 ZIP 다운로드만 하고, 현장에서 커밋·푸시하지 않는다.
- 현장 VDI에서 개인 GitHub 계정으로 로그인하지 않는다. 공개 저장소는 로그인 없이 받을 수 있다.
- 채운 노트는 현장 안(내 노트 폴더)에만 둔다. 집에서 정리할 때는 일반적인 예제 이름으로 바꿔서 새로 쓴다.

## 템플릿 목록

| 파일 | 언제 쓰나 |
| --- | --- |
| `templates/01-self-check.md` | 2~3주마다 내 실력 점검 |
| `templates/02-screen-flow.md` | 화면 하나의 흐름을 API부터 테이블까지 추적할 때 |
| `templates/03-query-analysis.md` | 긴 쿼리 하나를 읽을 때 |
| `templates/04-glossary.md` | 낯선 테이블명, 컬럼명, 약어를 모을 때 (계속 누적) |
| `templates/05-method-names.md` | 메서드명을 계층별로 정리할 때 (계속 누적) |
| `templates/06-feature-analysis.md` | 기능 하나를 분석하거나 새로 만들 때 |
| `templates/07-daily-note.md` | 매일 퇴근 전 |

## 추천 노트 폴더 구조 (현장 안에서)

```
Private-memo/
  glossary.md            <- 04 템플릿, 하나만 두고 계속 추가
  method-names.md        <- 05 템플릿, 하나만 두고 계속 추가
  self-check.md          <- 01 템플릿, 회차별로 칸 채우기
  daily/
    2026-11-02.md        <- 07 템플릿을 날짜별로 복사
  screens/
    (화면이름).md         <- 02 템플릿을 화면별로 복사
  queries/
    (쿼리id).md           <- 03 템플릿을 쿼리별로 복사
  features/
    (기능이름).md         <- 06 템플릿을 기능별로 복사
```

## 쓰는 순서

1. 화면 하나를 고른다.
2. `02-screen-flow`로 사용자 행동, API, 백엔드, 테이블을 연결한다.
3. 그중 핵심 쿼리 하나를 `03-query-analysis`로 읽는다.
4. 읽다가 나온 낯선 이름은 바로 `glossary.md`, `method-names.md`에 추가한다.
5. 정리가 끝나면 `06-feature-analysis`로 그 기능을 한 장에 요약한다.
6. 퇴근 전 `07-daily-note`를 쓴다.
