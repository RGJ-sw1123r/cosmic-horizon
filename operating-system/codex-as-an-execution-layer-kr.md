---
description: 인간의 판단을 상위에 두고 AI 실행을 하위에 두는 운영체계에서 Codex가 적합한 이유.
tags:
  - operating-system
---

# Codex as an Execution Layer (KR)

> 항법 로그

## 현재 좌표계

* 도구는 유행이나 애착이 아니라 항해의 목적에 맞게 선택되어야 한다.
* AI-assisted development에서 핵심은 더 빠른 코드 생성이 아니라, 무엇을 사람이 판단하고 무엇을 AI에게 실행시킬지 나누는 능력이다.
* 이 운영체계에서 ChatGPT는 관측, 기획, 질문, 정제, 문서화의 공간이다.
* Codex는 이미 선언된 좌표 안에서 움직이는 하위 실행 계층이다.
* 이 문서에서 말하는 Codex는 ChatGPT 웹 대화 공간과 분리해, 프로젝트 컨텍스트를 읽고 CLI에서 파일 수정과 명령 실행을 수행하는 하위 실행 계층을 가리킨다.
* 핵심은 OpenAI 생태계 일반이 아니라, 웹 기획 공간과 CLI 실행 공간의 분리다.
* 이 문서는 ChatGPT를 기획 공간으로, Codex를 실행 계층으로 배치하는 운영 방식을 설명한다.
* AGENTS.md와 agent instruction file은 특정 벤더에 종속된 문법이 아니라, AI agent를 선언된 경계 안에서 움직이게 만드는 운영 장치다.
* 도구의 비용 구조와 작업 흐름은 단순한 가격 문제가 아니라, 작업자가 생각하고 실행하는 방식을 바꾸는 운영 조건이다.

## 좋은 도구의 기준

좋은 도구는 유행하는 도구가 아니다.

좋은 도구는 지금 나서는 항해에 맞는 도구다.

**성능** 중요하다.\
**비용** 중요하다.\
**작업 흐름** 중요하다.

OpenAI Codex로 항해를 시작한 이유도 여기에 있다.

물론 익숙함도 작용했다.

ChatGPT는 AI를 본격적인 작업 도구로 받아들이게 만든 첫 번째 인터페이스였다. 2023년 무렵부터 ChatGPT는 사고, 초안 작성, 검토, 개발 보조, 문서화에 계속 사용되어 왔다.

오래 사용한 만큼 익숙하고, 정이 든 것도 사실이다.

하지만 Codex를 사용하는 이유가 단지 익숙함이나 브랜드 애착에 있는 것은 아니다.

이 선택은 철저히 계산되었다.

## 더 잘 하는 일의 구분

AI에게 모든 일을 맡길 필요는 없다.

사람이 더 잘 해야 하는 일이 있고, AI가 더 빠르게 처리할 수 있는 일이 있다.

이 운영체계에서 Codex는 하위에 놓인 일만 철저하게 처리한다.

상위에는 관측이 있다.\
상위에는 요구 해석이 있다.\
상위에는 UX 판단이 있다.\
상위에는 제약 선언이 있다.\
상위에는 완료 기준 선언이 있다.

Codex는 이 모든 것이 결정된 후에 호출된다.

이미 관측되고, 구조화되고, 문서화되고, 선언된 좌표 안에서 구현을 담당하는 계층이다.

Codex는 고객을 만나지 않는다.\
Codex는 사용자의 피로를 직접 관측하지 않는다.\
Codex는 어떤 화면이 왜 필요한지 최종적으로 책임지지 않는다.\
Codex는 사업 맥락, 조직의 비용, 기존 시스템의 불만, 고객의 숨은 요구를 인간처럼 책임지지 않는다.

그래서 Codex는 선장이 아니다.

Codex는 내가 정한 좌표 안에서 움직이는 실행 계층이다.

## 인간이 해야 하는 일

이 운영체계는 다음 작업을 상위에 둔다.

* 고객이 실제로 무엇을 원하는지 관측하는 일.
* 고객이 어디에서 피로감을 느끼는지 읽는 일.
* 기존 시스템에 존재하던 UX 불만을 분리하는 일.
* 화면에서 최종적으로 도출되어야 하는 결과를 정하는 일.
* MVP에 포함할 것과 제외할 것을 결정하는 일.
* 요구사항과 소음을 구분하는 일.
* 색상 톤, 브랜드 맥락, 화면의 리듬을 잡는 일.
* 구현이 반드시 지켜야 할 제약을 선언하는 일.
* 완료 기준을 정의하는 일.
* AI가 추론해도 되는 영역과 추론해서는 안 되는 영역을 나누는 일.

이 일들은 구현 세부사항이 아니다.

이 일들은 개발자가 책임져야 하는 항로 설정이다.

AI는 이 과정을 도울 수 있다.

질문을 던질 수 있다.\
놓친 조건을 지적할 수 있다.\
대안을 비교할 수 있다.\
문장을 정리할 수 있다.\
프롬프트를 더 선명하게 만들 수 있다.

하지만 책임 있는 결정은 상위에 남아야 한다.

상위가 비어 있으면 하위 실행은 빠를수록 더 크게 흔들린다.

## 문서는 실행에 앞선다

> Pre-AI: code without docs.\
> Post-AI: docs without code.

이전 시대의 개발은 코드를 다 작성한 후 거기에 맞는 문서를 만드는 일이 잦았다.

AI 활용 개발에서는, 문서화가 먼저 온다.

이 운영체계에서 문서는 인간의 판단을 AI가 따라갈 수 있는 좌표로 바꾸는 계층이다.

좋은 지시는 단순한 요청이 아니다.

좋은 지시는 설계된 artifact다.

목표가 무엇인지, 어떤 맥락을 보존해야 하는지, 어떤 제약을 넘지 말아야 하는지, 무엇이 완료 상태인지가 문서 안에 명시되어야 한다.

OpenAI의 Codex best practices도 좋은 작업 지시에 Goal, Context, Constraints, Done when을 넣으라고 설명한다.

이 기준은 AI의 추론 여백을 줄이는 엔지니어링이다.

AI가 추론만으로 빈칸을 채워야 하는 여지를 줄이는 방법이다.

웹에서 ChatGPT와 오래 논의하는 이유도 여기에 있다.

Codex가 실행될 때 추론으로 메워야 할 빈칸을 줄이기 위해서다.

인간이 충분히 관측하고, 질문하고, 정제하고, 문서화하면 Codex는 더 안전한 경로를 따라 움직인다.

## 실행 계층이 맡는 일

상위의 판단이 정리되면 Codex는 자신이 잘하는 일을 맡는다.

파일을 읽는다.\
코드를 수정한다.\
명령을 실행한다.\
반복 구조를 빠르게 구현한다.\
라이브러리를 연결한다.\
import를 정리한다.\
테스트를 돌린다.\
diff를 남긴다.\
검토 가능한 결과물을 만든다.

이 작업이 항상 인간의 손으로 직접 수행되어야 하는 것은 아니다.

구현은 선언된 프레임 안에서 실행으로 가치를 갖는다.

무게중심이 이동했다는 뜻이다.

AI가 더 빠르게 구현할 수 있다면, 인간 개발자의 주의력은 더 상위로 이동해야 한다.

더 나은 관측.\
더 명확한 제약.\
더 강한 검증.\
더 선명한 완료 기준.\
더 회귀 가능한(Return to Origin) 작업 기록.

Codex는 이 운영체계에서 구현 담당자다.

무엇이 존재해야 하는지를 결정하는 주체가 아니다.

이미 관측되고, 구조화되고, 선언된 것을 코드로 옮기는 실행 계층이다.

## 분리 개념이 중요한 이유

이 워크플로우에서는 분리 개념이 중요하다.

상위에서는 오래 생각해야 한다.

고객 요구를 해석해야 한다.\
MVP를 좁혀야 한다.\
UX 불만을 정리해야 한다.\
화면의 목적을 잡아야 한다.\
제약을 선언해야 한다.\
AI에게 맡길 수 있는 단위로 지시를 다시 써야 한다.

이 단계는 기획과 구상의 영역이며, 항해를 안전하게 만들기 위한 항법이다.

생각하는 단계를 축소하면, 결과물은 빠르게 받을 수 있다.

하지만 검토 비용, 되돌리기 비용, 책임 비용은 뒤에서 커진다.

현재 OpenAI의 Codex는 ChatGPT 플랜 안에서 사용할 수 있지만, 플랜별 사용 한도가 있고 agentic usage limit에 포함된다.

이 문서의 핵심은 기획/구상 공간과 CLI 실행 공간의 분리다.

현재의 작업 방식에서 ChatGPT는 관측하고, 질문하고, 정제하고, 문서화하는 공간으로 쓰인다.

Codex CLI는 준비된 좌표를 실제 프로젝트 안에서 실행하는 공간으로 쓰인다.

이 분리가 유지되면 실행 전에 충분히 생각할 수 있다.

그리고 실행할 때는 더 좁고 명확한 지시를 넘길 수 있다.

도구가 작업자의 사고를 제한해서는 안 된다.

좋은 항법은 상위 계층에서 충분히 관측하고 판단한 뒤, 항해를 안전하고 빠르게 만들어야 한다.

## 2025 개발자 통계가 보여주는 좌표

2025년 개발자 통계는 이 구분이 왜 필요한지 보여준다.

AI 사용 자체는 이미 희귀한 일이 아니다.

Stack Overflow Developer Survey 2025에 따르면 응답자의 84%는 개발 과정에서 AI 도구를 사용하거나 곧 사용할 계획이라고 답했다. 전문 개발자 중 50.6%는 AI 도구를 매일 사용한다고 답했다.

하지만 질문을 일반적인 AI 사용에서 agentic work로 좁히면 숫자는 크게 줄어든다.

전문 개발자 중 업무에서 AI agent를 매일 사용하는 비율은 14.9%, 주간 사용은 9.2%, 월간 또는 가끔 사용은 7.7%다. 합치면 전문 개발자 중 약 31.8%가 업무에서 AI agent를 사용한다고 답한 것이다.

같은 조사에서 Stack Overflow는 vibe coding을 LLM 프롬프트로 소프트웨어를 생성하는 과정으로 정의했다. 이 문항에서 “Yes, emphatically”는 0.4%, “Yes”는 11.9%, “Yes, somewhat”는 2.8%였다. 반면 “No”는 72.2%, “No, emphatically”는 5.3%였다.

| 범주                                  | 2025 지표 | 해석                                             |
| ----------------------------------- | ------: | ---------------------------------------------- |
| 개발 과정에서 AI를 쓰거나 쓸 계획이 있는 응답자        |     84% | AI 사용 자체는 이미 주류다.                              |
| AI 도구를 매일 쓰는 전문 개발자                 |   50.6% | AI는 일상 도구가 되고 있다.                              |
| 업무에서 AI agent를 매일 쓰는 전문 개발자         |   14.9% | agentic work는 아직 소수의 실천이다.                     |
| 업무에서 AI agent를 사용한다고 답한 전문 개발자      |   31.8% | agent에게 실제 작업을 넘기는 경험은 늘고 있지만 보편화되지는 않았다.      |
| vibe coding이 전문 개발 업무 일부라고 답한 응답자   |   15.1% | 프롬프트 기반 소프트웨어 생성을 자기 업무 방식으로 받아들이는 층은 더 좁다.    |
| vibe coding이 자신의 업무 일부가 아니라고 답한 응답자 |   72.2% | 많은 개발자는 AI를 쓰더라도 자기 일을 vibe coding이라고 부르지 않는다. |

이 통계 수치가 이 항법체계를 직접 증명해 주지는 않는다.

하지만 한 가지 경계는 보여준다.

AI 사용은 주류가 되었다.

업무에서 AI agent를 쓰는 층은 더 좁다.

프롬프트 기반 소프트웨어 생성을 전문 업무 방식으로 받아들이는 층은 더 좁다.

그리고 이 조사는 개발자가 고객 요구, UX 판단, 제약 조건, 완료 기준을 먼저 문서화한 뒤 AI agent를 하위 실행 계층으로 호출하는지까지 묻지는 않는다.

바로 그 지점에 이 문서의 좌표가 있다.

인간의 판단을 상위에서 명시하고, AI 실행을 하위에서 통제하는 방식은 아직 일반적인 설문 언어 안에 뚜렷하게 잡히지 않는다.

이 문서는 통계가 아직 이름 붙이지 못한 사용법을 기록하려는 시도다.

## 통계가 말하지 않는 사용법

Stack Overflow 조사는 또 다른 경계도 보여준다.

개발자들은 AI를 검색, 학습, 코드 작성, 문서화, 테스트 같은 영역에는 비교적 쉽게 들인다. 반면 배포와 모니터링에는 76%, 프로젝트 계획에는 69%가 AI를 사용할 계획이 없다고 답했다.

이 경계는 합리적이다.

프로젝트 계획, 고객 요구 해석, 화면 목적 정의, UX 판단은 그대로 AI에게 넘길 일이 아니다.

하지만 AI가 이 영역에서 아무 역할도 하지 못한다는 뜻도 아니다.

AI는 판단자가 아니라 관측 보조자, 질문자, 정리자, 검산자, 실행 지시 정제자가 될 수 있다.

프로젝트 계획을 AI에게 넘기는 것과, 프로젝트 계획을 사람이 책임질 수 있도록 AI로 더 잘 문서화하는 것은 다른 일이다.

책임을 넘기는 것과, 책임을 더 선명하게 만들기 위해 AI를 쓰는 것은 다른 작업 방식이다.

이 운영체계는 후자를 선택한다.

## 도구 선택은 운영 결정이다

도구 선택은 브랜드 선호가 아니다.

도구는 운영체계의 일부다.

따라서 이 문서는 현재 작업 방식에서 어떤 도구가 실행 계층으로 적합한지 판별하는 기준을 다룬다.

이 문서가 말하는 것은 특정 제품의 우월성이 아니라, 현재의 작업 방식에서 어떤 도구가 가장 적합한 실행 계층으로 놓이는가이다.

AGENTS.md나 agent instruction file도 같은 기준에서 보아야 한다.

그것은 Codex 전용 문법이 아니다. Claude Code, Gemini CLI, Antigravity, Codex처럼 프로젝트 문맥을 읽고 실행하는 AI agent에게 모두 적용될 수 있는 운영 경계다.

벤더는 달라질 수 있다.

하지만 agent가 어디를 봐야 하는지, 언제 움직여야 하는지, 무엇을 추론하면 안 되는지, 어디서 멈춰야 하는지를 선언해야 한다는 원칙은 달라지지 않는다.

Claude Code는 강력한 도구일 수 있다. 하지만 Anthropic은 Pro와 Max 플랜에서 Claude와 Claude Code의 사용량 한도가 공유된다고 설명한다.

Google의 Gemini Code Assist 문서도 Gemini Code Assist agent mode와 Gemini CLI의 요청 쿼터가 결합되어 있으며, agent mode나 CLI에서는 하나의 prompt가 여러 model request로 이어질 수 있다고 설명한다.

이런 세부사항은 단순한 과금 정보가 아니다.

워크플로우의 행동을 바꾼다.

상위의 사고 단계는 비용 낭비가 아니다.

상위의 사고 단계는 하위의 실패를 줄이는 곳이다.

문서화 단계는 agent가 나중에 만들 실수를 태어나기 전에 줄이는 곳이다.

검증 기준을 먼저 선언하는 일은 인간의 책임을 보이게 만드는 일이다.

이 단계를 비싸게 만들거나 취약하게 만드는 도구는 이 운영 모델에 잘 맞지 않는다.

## 시장 신호로서의 Codex

이것이 OpenAI가 모든 한도를 없앴다는 뜻은 아니다.

Codex에는 플랜별 사용 한도가 있다. 한도에 가까워지거나 도달하면 플랜에 따라 크레딧 추가, 업그레이드, reset 대기 같은 선택지가 필요할 수 있다.

하지만 시장에서 드러난 신호도 있다.

Claude Code의 가격과 플랜을 둘러싼 혼선이 있었을 때, OpenAI Codex 쪽에서는 Codex가 Free와 Plus 플랜에서도 제공된다는 방향의 공개 반응을 보였다. Sam Altman도 같은 흐름에서 “We want you to have a lot of AI!”라고 반응했다.

이 발언은 공식 가격 정책 문서가 아니다.

하지만 제품 방향을 보여주는 시장 신호로는 읽을 수 있다.

적어도 그 순간 OpenAI는 Codex를 별도의 고가 코딩 제품으로만 분리하기보다, ChatGPT 플랜 안에서 넓게 제공하려는 방향을 공개적으로 보여주었다.

상위에서 충분히 관측하고, 문서화하고, CLI에서는 실행만 맡기는 워크플로우에서는 이 차이가 크다.

도구가 작업자의 사고를 제한해서는 안 된다.

도구는 충분한 관측과 판단이 끝난 뒤 실행을 빠르게 만들어야 한다.

## 운영 문장

Codex는 이 운영체계의 중심이 아니다.

중심은 Codex가 실행되기 전에 존재하는 관측과 판단이다.

ChatGPT는 상위의 관측, 질문, 정제, 문서화를 돕는다.

Codex는 하위의 구현, 수정, 실행, 검증을 돕는다.

둘 사이의 분리는 비용 문제가 아니라 운영 문제다.

AI가 더 빠르게 구현할수록, 인간은 더 선명하게 관측해야 한다.

## 결론 (Conclusion)

OpenAI Codex는 이 워크플로우의 선장이 아니다.

Codex는 항법장치도 아니다.

Codex는 관측, 판단, 문서화 아래에 설치되는 실행 계층이다.

이 운영체계에서 인간의 일은 AI보다 빠르게 코드를 치는 것이 아니다.

인간의 일은 AI가 움직일 수 있는 좌표를 책임 있게 선언하는 것이다.

고객을 관측한다.\
구조를 이해한다.\
경계를 선언한다.\
완료 기준을 정한다.\
AI에게 실행을 맡긴다.\
결과를 검산한다.\
필요하면 좌표로 되돌아간다.

그래서 Codex를 사용한다.

**도구란 그래야 한다.**

⛵

## 이웃 좌표계

* [Ride, Don’t Race (KR)](../perspective/ride-dont-race-kr.md)는 도구의 속도에 끌려가지 않고, 자신의 리듬으로 도구를 통제하는 탑승자의 관점과 연결된다.
* [The Gravity Behind Market Language (KR)](../perspective/the-gravity-behind-market-language-kr.md)는 시장이 붙인 AI 도구의 이름표를 구조, 비용, 위험, 책임으로 번역해야 하는 이유를 다룬다. 이 문서는 그 관점을 Codex 선택에 적용한 기록이다.
* [AI-Assisted Development Models (KR)](ai-assisted-development-models-kr.md)는 이 도구 선택의 배경이 되는 observation system을 설명한다. 요구사항, 제약, 경계, 완료 기준이 선언된 뒤 Codex가 하위 실행 계층에 놓이는 이유와 연결된다.
* [\[pattern\] FTL-Bound Agents](pattern-ftl-bound-agents/)는 Codex 같은 실행 계층이 해석을 통해 작업 범위를 넓히지 않도록, agent instruction file을 운영 경계로 다루는 방식을 설명한다.
* [\[protocol\] AGENTS.md Blueprint](pattern-ftl-bound-agents/protocol-agents.md-blueprint.md)는 그 경계를 AGENTS.md 형태의 반복 가능한 프로젝트 지시 체계로 구현하는 방식을 보여준다.

## Source Notes

* **OpenAI Codex Best Practices** — OpenAI, [Best practices – Codex](https://developers.openai.com/codex/learn/best-practices). 좋은 작업 지시에 Goal, Context, Constraints, Done when을 넣으라고 설명한다.
* **OpenAI Codex CLI** — OpenAI, [Codex CLI](https://developers.openai.com/codex/cli). Codex CLI의 역할과 터미널 기반 실행 환경을 설명한다.
* **OpenAI Codex with ChatGPT Plan** — OpenAI Help Center, [Using Codex with your ChatGPT plan](https://help.openai.com/en/articles/11369540-using-codex-with-your-chatgpt-plan). Codex의 플랜별 사용 구조와 agentic usage limit 관련 내용을 설명한다.
* **Stack Overflow Developer Survey 2025 — AI Usage** — Stack Overflow, [Developer Survey 2025: AI](https://survey.stackoverflow.co/2025/ai). AI 도구 사용률, AI agent 사용률, vibe coding 관련 응답을 확인하는 데 사용했다.
* **Anthropic Claude Code Usage** — Anthropic Help Center, [Use Claude Code with your Pro or Max plan](https://support.claude.com/en/articles/11145838-use-claude-code-with-your-pro-or-max-plan). Claude와 Claude Code의 사용량 한도 공유 구조를 확인하는 데 사용했다.
* **Google Gemini Code Assist Quotas** — Google Developers, [Quotas and limits | Gemini Code Assist](https://developers.google.com/gemini-code-assist/resources/quotas). Gemini Code Assist agent mode와 Gemini CLI의 요청 쿼터 구조를 확인하는 데 사용했다.
* **OpenAI Codex Market Signal** — Business Insider, [Anthropic's Claude Code pricing pain is Sam Altman's pleasure](https://www.businessinsider.com/anthropic-claude-code-price-confusion-sam-altman-2026-4). Sam Altman의 “We want you to have a lot of AI!” 발언과 Codex Free/Plus 제공 관련 공개 반응을 시장 신호로 해석하는 데 사용했다. 관련 X 링크: [Sam Altman](https://x.com/sama/status/2046752492093165708), [Thibault Sottiaux](https://x.com/thsottiaux/status/2046740759056162816).
