# ai-career-roadmap

퍼블리셔 → Python · FastAPI · LLM 풀스택 40주 학습 기록 (2026-11-04 시작)

계획은 노션 체크리스트\_v3, 기록과 코드는 여기에 남깁니다.

## 폴더

```
weeks/week01/       주차 폴더
  README.md         그 주 체크리스트 + 회고
  11-04.md          하루 기록 (날짜별)
  *.py              연습 코드
coding-test/        프로그래머스 풀이
```

## 직접 친 코드 남기는 법

그날 공부하면서 직접 친 연습 코드를 파일로 저장해 커밋합니다.

- 위치: 그 주 폴더(`weeks/week01/`)
- 파일 이름: 번호 + 주제, 주제 하나당 파일 하나 (`01_basics.py`)
- 치는 방법: 예제를 한 번 보고 덮은 뒤 치고, 값을 바꿔서 실행까지 하기
- 대화형 셸에서 친 코드는 저장되지 않으니 된 코드를 `.py`로 옮기기 (`.ipynb`는 그대로 커밋 가능)
- 주석은 내 말로 짧게 (`# JS의 "ab".repeat(3)과 같음`)
- 설명하지 못하는 코드는 `이해 못 한 것`에 적고, 이해한 뒤에 커밋
- 개념만 읽은 날은 확인용 코드를 5줄이라도 치기

## 코딩 테스트 남기는 법

- 프로그래머스에서 직접 풀고, 내 코드를 `coding-test/`에 저장
- 파일 이름: `문제번호_제목.py` (JS 풀이는 `.js`)
- 파일 맨 위에 링크, 유형, 결과, 배운 점을 주석으로 쓰기
- 지문은 옮기지 않고 링크만 남기기
- 힌트를 봤거나 못 풀었으면 결과에 그대로 쓰기
- `coding-test/README.md` 표에 한 줄 추가

## 매일 할 일

1. 공부 시작 전에 최신 내용 받기

   ```bash
   git pull
   ```

2. 연습 코드 커밋

   ```bash
   git add weeks/week01/01_basics.py
   git commit -m "feat: 변수 숫자 문자열 연습"
   ```

3. 코테 풀이 커밋

   ```bash
   git add coding-test
   git commit -m "solve: 120822 뒤집힌 문자열"
   ```

4. `weeks/weekNN/`에 오늘 날짜 파일(`11-04.md`)을 만들고 3줄 쓴 뒤 커밋

   ```
   # 11/04 (수)
   - 배운 것:
   - 구현한 것:
   - 이해 못 한 것:
   ```

   ```bash
   git add weeks/week01/11-04.md
   git commit -m "docs: 11/04 기록"
   ```

5. push하고 GitHub에서 파일 확인

   ```bash
   git push
   ```

6. 노션에서 그날의 `완료` 체크

## 금요일에 추가로 할 것

1. 그 주 `README.md`의 체크리스트와 회고 채우기
2. 완료 기준을 통과했으면 아래 진행 현황의 ⬜를 ✅로 바꾸기
3. `docs: 1주차 회고`로 커밋하고 push

   ```bash
   git add weeks/week01/README.md README.md
   git commit -m "docs: 1주차 회고"
   git push
   ```

## 지킬 것

- 파일을 지정해서 `git add`하고, 올리기 전에 `git status`로 확인
- 잔디는 `main`에 올린 커밋이고 커밋 이메일이 GitHub 계정에 등록돼 있어야 표시됨. 쉬는 날 억지로 채우지 않기
- API 키는 `.env`에만 넣기. 한 번 push하면 파일을 지워도 기록에 남음
- 미니 프로젝트와 대표 프로젝트는 저장소를 따로 만들고, 일일 기록에는 링크만 남기기

## 커밋 메시지

| 타입    | 언제             | 예시                          |
| ------- | ---------------- | ----------------------------- |
| `docs`  | 기록·회고        | `docs: 11/04 기록`            |
| `solve` | 코테 풀이        | `solve: 120822 뒤집힌 문자열` |
| `feat`  | 연습 코드·결과물 | `feat: 변수 숫자 문자열 연습` |
| `fix`   | 고친 것          | `fix: 파일 경로 오류 수정`    |

## 40주 진행 현황

**A구간 · Python + CS 복구 (1~4주, 11월)**

| 주  | 시작  | 주제                                               | 완료 |
| --- | ----- | -------------------------------------------------- | ---- |
| 1   | 11/04 | [Python 기초 1](weeks/week01/README.md)            | ⬜   |
| 2   | 11/09 | [Python 기초 2](weeks/week02/README.md)            | ⬜   |
| 3   | 11/16 | [Python 실전 문법](weeks/week03/README.md)         | ⬜   |
| 4   | 11/23 | [자료구조 복구 + API 호출](weeks/week04/README.md) | ⬜   |

**B구간 · FastAPI + DB + 풀스택 (5~16주, 12~2월)**

| 주  | 시작  | 주제                                                                    | 완료 |
| --- | ----- | ----------------------------------------------------------------------- | ---- |
| 5   | 11/30 | [HTTP·REST + FastAPI 기본](weeks/week05/README.md)                      | ⬜   |
| 6   | 12/07 | [Pydantic 검증 + 예외 처리](weeks/week06/README.md)                     | ⬜   |
| 7   | 12/14 | [SQL 기초](weeks/week07/README.md)                                      | ⬜   |
| 8   | 12/21 | [PostgreSQL + SQLAlchemy 1 (연결·모델)](weeks/week08/README.md)         | ⬜   |
| 9   | 12/28 | [PostgreSQL + SQLAlchemy 2 (관계·마이그레이션)](weeks/week09/README.md) | ⬜   |
| 10  | 01/04 | [TypeScript + Next.js 연동 1 (TypeScript)](weeks/week10/README.md)      | ⬜   |
| 11  | 01/11 | [TypeScript + Next.js 연동 2 (FastAPI 연결)](weeks/week11/README.md)    | ⬜   |
| 12  | 01/18 | [인증과 보안 기초 1 (해싱·JWT)](weeks/week12/README.md)                 | ⬜   |
| 13  | 01/25 | [인증과 보안 기초 2 (쿠키·테스트)](weeks/week13/README.md)              | ⬜   |
| 14  | 02/01 | [리눅스 기초 + Docker + Git 협업](weeks/week14/README.md)               | ⬜   |
| 15  | 02/08 | [미니 프로젝트 1 마감](weeks/week15/README.md)                          | ⬜   |
| 16  | 02/15 | [고정 버퍼 1](weeks/week16/README.md)                                   | ⬜   |

**C구간 · LLM 실무 (17~23주, 2~4월)**

| 주  | 시작  | 주제                                                    | 완료 |
| --- | ----- | ------------------------------------------------------- | ---- |
| 17  | 02/22 | [LLM API 기초 + 비동기 호출](weeks/week17/README.md)    | ⬜   |
| 18  | 03/01 | [구조화 출력 + 검증](weeks/week18/README.md)            | ⬜   |
| 19  | 03/08 | [스트리밍 채팅 UI](weeks/week19/README.md)              | ⬜   |
| 20  | 03/15 | [프레임워크 없이 직접 RAG](weeks/week20/README.md)      | ⬜   |
| 21  | 03/22 | [RAG 품질 개선 + 보안](weeks/week21/README.md)          | ⬜   |
| 22  | 03/29 | [프레임워크 비교 + 평가 자동화](weeks/week22/README.md) | ⬜   |
| 23  | 04/05 | [고정 버퍼 2](weeks/week23/README.md)                   | ⬜   |

**D구간 · 대표 프로젝트 + 베타 사용자 + 지원 시작 (24~31주, 4~5월)**

| 주  | 시작  | 주제                                                        | 완료 |
| --- | ----- | ----------------------------------------------------------- | ---- |
| 24  | 04/12 | [대표 프로젝트 설계](weeks/week24/README.md)                | ⬜   |
| 25  | 04/19 | [백엔드 구현 1](weeks/week25/README.md)                     | ⬜   |
| 26  | 04/26 | [백엔드 구현 2](weeks/week26/README.md)                     | ⬜   |
| 27  | 05/03 | [프론트 구현](weeks/week27/README.md)                       | ⬜   |
| 28  | 05/10 | [품질 평가·개선](weeks/week28/README.md)                    | ⬜   |
| 29  | 05/17 | [배포 + 베타 오픈](weeks/week29/README.md)                  | ⬜   |
| 30  | 05/24 | [피드백 반영 + 포트폴리오와 이력서](weeks/week30/README.md) | ⬜   |
| 31  | 05/31 | [지원 시작](weeks/week31/README.md)                         | ⬜   |

**E구간 · 보강 + 지원 병행 (32~40주, 6~8월)**

| 주  | 시작  | 주제                                                                  | 완료 |
| --- | ----- | --------------------------------------------------------------------- | ---- |
| 32  | 06/07 | [머신러닝 기본 1](weeks/week32/README.md)                             | ⬜   |
| 33  | 06/14 | [머신러닝 기본 2](weeks/week33/README.md)                             | ⬜   |
| 34  | 06/21 | [딥러닝·Transformer 개념 (1주로 축소)](weeks/week34/README.md)        | ⬜   |
| 35  | 06/28 | [CI/CD + 클라우드 기초 (1주로 축소)](weeks/week35/README.md)          | ⬜   |
| 36  | 07/05 | [과제 전형·프론트 면접 집중](weeks/week36/README.md)                  | ⬜   |
| 37  | 07/12 | [프로젝트 2: 퍼블리싱 업무 자동화 에이전트 1](weeks/week37/README.md) | ⬜   |
| 38  | 07/19 | [프로젝트 2: 퍼블리싱 업무 자동화 에이전트 2](weeks/week38/README.md) | ⬜   |
| 39  | 07/26 | [면접·코테 점검](weeks/week39/README.md)                              | ⬜   |
| 40  | 08/02 | [전체 점검](weeks/week40/README.md)                                   | ⬜   |
