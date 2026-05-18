
# **루퍼스 웹 백엔드 3기 김진수**

> 김진수의 루퍼스 활동 내용 아카이브입니다.

## [루퍼스란?](https://www.loopers.im/)

- 빅테크 현업 시니어 개발자가 주관하는 백엔드 개발자 교육 프로그램
- 루퍼스 과정은 AI 시대에 빠른 '구현자'가 아닌, 상황에 맞게 기술을 선택하고 설명할 수 있는 '판단자'를 양성하는 `10주 집중 프로그램`으로 진행
- 모든 학습은 현업 문제 중심의 `개인 미션`과, 주차별 핵심 개념을 토론하고 설계 관점을 공유하는 `팀 코어 타임` 기반으로 진행
- 설계·정합성·성능·안정성·확장 구조 등의 하드 스킬뿐만 아니라, `테크니컬 글쓰기`, `현업 멘토 1:1 피드백`, `AI 활용 사고 정리` 등의 소프트 스킬 교육 제공

## 💬 고민을 나누며 시야를 넓힌 아고라
아고라는 멘토·동료들과 학습 내용과 판단 근거를 자유롭게 나누는 공간으로, 자기 주도적인 성장을 지향하는 루퍼스의 문화 중 하나입니다.
이런 판단 고민들을 아고라에 던졌습니다:

📌 랭킹 집계 단위 선택 — weekly vs daily 입력, 스케줄러 간 의존성 트레이드오프

<table>
<tr>
<th align="center">📝 질문</th>
<th align="center">💬 댓글</th>
</tr>
<tr>
<td><img width="700" alt="아고라 질문" src="https://github.com/user-attachments/assets/d803e839-a3b7-4a1e-84f4-972867f23f1e" /></td>
<td><img width="700" alt="아고라 답변1" src="https://github.com/user-attachments/assets/6cc323a5-28bf-450a-ba71-976cb90f722b" /></td>
</tr>
</table>

---

## 1️⃣ Level 1 - "AI와 설계의 기본기" (2026.02.07 ~ 2026.02.27)

- AI를 단순 도구가 아닌 협업 에이전트로 활용하기 위한 워크플로우 탐구
- 요구사항을 도메인 관점에서 해석하고 객체 책임을 나누는 설계 연습 진행
- API 명세를 먼저 정의하고, 이를 기준으로 서버 구조를 설계하는 흐름 학습
- TDD를 통해 설계 의도를 코드로 검증하는 피드백 루프 활성화 연습

### ✍️ 글로 남긴 학습 기록

- 🔗 [**AI 협업의 적정 지점을 찾아 네 번 부딪힌 기록**](https://plan22plan.tistory.com/entry/%EC%84%A4%EA%B3%84%EB%8A%94-%EB%82%B4%EA%B0%80-%EA%B5%AC%ED%98%84%EC%9D%80-AI%EA%B0%80-TDD-%ED%98%91%EC%97%85-%EB%B0%A9%EC%8B%9D-%ED%83%90%EC%83%89%ED%95%98%EB%A9%B0-%EB%8A%90%EB%82%80%EC%A0%90)
- 🔗 [**Claude Code로 개발하며 만든 컨벤션 검증 시스템 — Skills, Hook, ArchUnit, 서브 에이전트**](https://plan22plan.tistory.com/entry/Claude-Code-Skills-%EA%B8%B0%EB%B0%98-%EC%95%84%ED%82%A4%ED%85%8D%EC%B2%98-%EC%BB%A8%EB%B2%A4%EC%85%98-%EC%9E%90%EB%8F%99%ED%99%94-%EC%8B%9C%EC%8A%A4%ED%85%9C-%EC%84%A4%EA%B3%84-1)
- 🔗 [**회원 요구사항 분석부터 도메인 책임 분배까지**](https://plan22plan.tistory.com/entry/%EA%B0%84%EB%8B%A8%ED%95%9C-%ED%9A%8C%EC%9B%90-%EC%9A%94%EA%B5%AC%EC%82%AC%ED%95%AD%EC%9C%BC%EB%A1%9C-%E3%85%A1-%EC%84%A4%EA%B3%84-%EA%B3%A0%EB%AF%BC%ED%95%98%EA%B8%B0)
- 🔗 [**변경에 흔들리는 시퀀스 다이어그램을 다시 그리며 배운 것**](https://plan22plan.tistory.com/entry/%ED%9B%88%EB%A0%A8%EA%B8%B0-%EB%82%98%EC%9D%98-%EC%8B%9C%ED%80%80%EC%8A%A4-%EB%8B%A4%EC%9D%B4%EC%96%B4%EA%B7%B8%EB%9E%A8%EC%9D%B4-%EC%99%84%EC%84%B1%EB%90%98%EA%B8%B0%EA%B9%8C%EC%A7%80)

### 💻 주차별 PR

| 주차 | PR |
| --- | --- |
| 1주차 | [바로가기](https://github.com/Loopers-dev-lab/loop-pack-be-l2-vol3-java/pull/41) |
| 2주차 | [바로가기](https://github.com/Loopers-dev-lab/loop-pack-be-l2-vol3-java/pull/72) |
| 3주차 | [바로가기](https://github.com/Loopers-dev-lab/loop-pack-be-l2-vol3-java/pull/116) |

---

## 2️⃣ Level 2 - "데이터 정합성과 성능" (2026.02.28 ~ 2026.03.13)

- 단순 CRUD를 넘어 트래픽 증가 상황에서 발생하는 데이터 정합성과 성능 문제 탐구
- 트랜잭션 경계와 락 전략을 통해 동시성 이슈를 해결하는 연습 진행
- 조회 패턴 기반 인덱스 설계와 캐시 도입을 통해 성능을 비교·분석하는 학습

### ✍️ 글로 남긴 학습 기록

- 🔗 [**상품이 바뀌면 좋아요(찜) 데이터는 어떻게 해야 할까?**](https://plan22plan.tistory.com/entry/%EC%B0%9C-%EB%8D%B0%EC%9D%B4%ED%84%B0%EC%9D%98-%EC%A0%95%ED%95%A9%EC%84%B1-vs-%EC%8B%9C%EC%8A%A4%ED%85%9C-%EB%B3%B5%EC%9E%A1%EB%8F%84)
- 🔗 [**같은 상품에 좋아요를 두 번 누르면 어떻게 될까?**](https://plan22plan.tistory.com/entry/%EA%B0%99%EC%9D%80-%EC%83%81%ED%92%88%EC%97%90-%EC%A2%8B%EC%95%84%EC%9A%94%EB%A5%BC-%EB%91%90-%EB%B2%88-%EB%88%84%EB%A5%B4%EB%A9%B4-%EC%96%B4%EB%96%BB%EA%B2%8C-%EB%90%A0%EA%B9%8C)
- 🔗 [**상품 정렬 조회 2,490ms → 35ms, 무엇이 병목이었나**](https://plan22plan.tistory.com/entry/%EC%A2%8B%EC%95%84%EC%9A%94%EC%88%9C-%EC%83%81%ED%92%88-%EC%A1%B0%ED%9A%8C-%EC%9D%BD%EA%B8%B0-%EC%84%B1%EB%8A%A5-%EC%B5%9C%EC%A0%81%ED%99%94)
- 🔗 [**동시성 처리 방법론과 기준 세우기**](https://plan22plan.tistory.com/entry/%EB%8F%99%EC%8B%9C%EC%84%B1-%EC%A0%9C%EC%96%B4%EB%A5%BC-%EC%9C%84%ED%95%B4-%EB%B9%84%EA%B4%80%EC%A0%81-%EB%9D%BD-vs-%EB%82%99%EA%B4%80%EC%A0%81-%EB%9D%BD-%EA%B3%A0%EB%AF%BC-%EB%B0%8F-%EC%A0%81%EC%9A%A9-%EA%B2%BD%ED%97%98)
- 🔗 [**동시성 테스트로 레이스 컨디션을 재현하는 방법 — CountDownLatch · ExecutorService**](https://plan22plan.tistory.com/entry/%EB%8F%99%EC%8B%9C%EC%84%B1-%ED%85%8C%EC%8A%A4%ED%8A%B8-%EA%B8%B0%EB%B2%95-CountDownLatch-ExecutorService)
- 🔗 [**비관적 락은 정말 순서를 보장할까? — MySQL의 트랜잭션 스케줄링 CATS**](https://plan22plan.tistory.com/entry/%EC%BF%A0%ED%8F%B0-%EB%8F%84%EB%A9%94%EC%9D%B8-%EB%AA%A8%EB%8D%B8%EB%A7%81)
- 🔗 [**Lost Update를 막는 두 가지 방법 — SERIALIZABLE vs 비관락 비교하기**](https://plan22plan.tistory.com/entry/%EB%9D%BD)
- 🔗 [**DeadLock 미리 고민하고 예방하자**](https://plan22plan.tistory.com/entry/%EB%B9%84%EA%B4%80%EC%A0%81-%EB%9D%BD%EC%97%90%EC%84%9C-%EB%8D%B0%EB%93%9C%EB%9D%BD%EC%9D%84-%EC%9E%AC%ED%98%84%ED%95%98%EB%A9%B0-%EB%8A%90%EB%82%80%EC%A0%90)

### 💻 주차별 PR

| 주차 | PR |
| --- | --- |
| 4주차 | [바로가기](https://github.com/Loopers-dev-lab/loop-pack-be-l2-vol3-java/pull/159) |
| 5주차 | [바로가기](https://github.com/Loopers-dev-lab/loop-pack-be-l2-vol3-java/pull/200) |

---

## 3️⃣ Level 3 - "안정성과 확장 구조" (2026.03.14 ~ 2026.04.03)

- 장애를 예외가 아닌 전제로 두고 시스템 구조를 재설계하는 연습 진행
- 기능 단위로 책임을 분리하여 장애 전파를 최소화하는 설계 학습
- 동기 처리의 한계를 이해하고 비동기 이벤트 기반 구조로 전환하는 경험

### ✍️ 글로 남긴 학습 기록

- 🔗 [**Spring ApplicationEvent 로그 찍으며 이해하기 — @EventListener · @TransactionalEventListener · @Async**](https://plan22plan.tistory.com/entry/Spring-ApplicationEvent-%EB%A1%9C%EA%B7%B8%EB%A1%9C-%EC%A6%9D%EB%AA%85%ED%95%98%EB%A9%B0-%ED%95%99%EC%8A%B5%ED%95%98%EA%B8%B0)
- 🔗 [**락을 줄이는 게 아니라 락이 필요한 구조를 없앴다 — 선착순 쿠폰 다시 설계기**](https://plan22plan.tistory.com/entry/%EC%84%A0%EC%B0%A9%EC%88%9C-%EC%BF%A0%ED%8F%B0-%EB%B0%9C%EA%B8%89-%EB%AC%B8%EC%A0%9C%EB%A5%BC-%EC%96%B4%EB%96%BB%EA%B2%8C-%EB%8B%A4%EB%A3%A8%EB%A9%B4-%EC%A2%8B%EC%9D%84%EA%B9%8C)
- 🔗 [**60명을 48명으로 깎았다가 결국 상한 자체를 없앤 기록 — 대기열 시스템 만들기**](https://plan22plan.tistory.com/entry/%EB%8C%80%EA%B8%B0%EC%97%B4%EC%97%90%EC%84%9C-%EC%B0%B8%EC%97%AC%EC%97%B4-%EC%83%81%ED%95%9C%EA%B0%92-%EA%B2%B0%EC%A0%95%ED%95%98%EA%B8%B0)

### 💻 주차별 PR

| 주차 | PR |
| --- | --- |
| 6주차 | [바로가기](https://github.com/Loopers-dev-lab/loop-pack-be-l2-vol3-java/pull/256) |
| 7주차 | [바로가기](https://github.com/Loopers-dev-lab/loop-pack-be-l2-vol3-java/pull/283) |

---

## 4️⃣ Level 4 - "집계와 운영 설계" (2026.04.04 ~ 2026.04.17)

- 실시간 처리만으로 해결되지 않는 문제를 운영 관점에서 재해석
- Redis와 배치 프로세스를 활용해 랭킹·집계 구조를 설계하는 연습 진행
- 운영 중 발생하는 데이터 누락·지연 상황을 가정하고 대응 전략을 학습

### ✍️ 글로 남긴 학습 기록

- 🔗 [**Redis SortedSet은 어떻게 동작하는 걸까?**](https://plan22plan.tistory.com/entry/Redis-SortedSet%EC%9D%80-%EC%96%B4%EB%96%BB%EA%B2%8C-%EB%8F%99%EC%9E%91%ED%95%98%EB%8A%94-%EA%B1%B8%EA%B9%8C)
- 🔗 [**머릿속이 복잡해서 일단 그려본 랭킹 시스템 설계**](https://plan22plan.tistory.com/entry/%EB%9E%AD%ED%82%B9-%EC%8B%9C%EC%8A%A4%ED%85%9C-%EB%A7%8C%EB%93%A4%EB%A9%B4%EC%84%9C-%EB%8A%90%EB%82%80%EC%A0%90)
- 🔗 [**'이 잡이 느리다'가 아니라 '얼마나 걸릴지 모른다' — Spring Batch 비선형 곡선 추적기**](https://plan22plan.tistory.com/entry/%EB%B9%84%EC%84%A0%ED%98%95-%EB%B0%B0%EC%B9%98-%EA%B3%A1%EC%84%A0%EC%9D%84-%EC%84%A0%ED%98%95%EC%9C%BC%EB%A1%9C-%ED%8E%B4%EA%B8%B0-Spring-Batch-ReaderWriter-%EA%B2%A9%EB%A6%AC-%EC%B8%A1%EC%A0%95-%EC%9A%B4%EC%98%81-%EC%95%88%EC%A0%95%EC%84%B1-%EA%B0%9C%EC%84%A0%EA%B8%B0)

### 💻 주차별 PR

| 주차 | PR |
| --- | --- |
| 8주차 | [바로가기](https://github.com/Loopers-dev-lab/loop-pack-be-l2-vol3-java/pull/333) |
| 9주차 | [바로가기](https://github.com/Loopers-dev-lab/loop-pack-be-l2-vol3-java/pull/375) |

---

## ✍️ 사고의 근육을 단련한 시간

AI에게 사고의 주체를 점점 넘기면서, 스스로 판단하는 시간이 줄어들고 성장도 천천히 멈춰가는 듯한 느낌이 들었습니다. **"기술이 바뀌어도 변하지 않는 것은 사고하는 능력이다"** 라는 말에 마음이 닿아, 무뎌진 사고의 근육을 다시 단련해보고 싶어 루퍼스를 신청했습니다.

이전이라면 *"좋아 보인다"* 는 직관으로 골랐을 기술을, 이제는 트레이드오프를 따져 현재 워크로드에 적합한지를 논리적으로 판단해 선택할 수 있게 — **결정의 근거가 직관에서 논리로 바뀌었다** 는 점에서 가장 큰 성장을 체감하고 있습니다.
