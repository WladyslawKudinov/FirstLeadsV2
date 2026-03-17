# Positioning Agent — Client Feedback

<!--
Group by theme, not by client or date.
Each entry: client name, version, date, quote or paraphrase.
Track action taken and resolution status.

## Theme: [description]
- Client (version, date): "quote"
- Resolved in vX / Not yet resolved
-->

---

## Theme: Positioning assumes full product scope — misses phased GTM reality

- **NapoleonIT** (v4, 2026-02-16): "хочу начать с очень понятного простого сервиса... если мы будем еще сопоставлять с бимом то такие пилоты они будут очень долго длится... давай BIM пока будем просто озвучивать, но первый этап — это просто обходы"
- **Impact:** 🔴
- **Pattern:** Positioning doc framed BIM-integration as "must have for Primary segment". Client explicitly said NO — BIM is Phase 2, not entry product. The agent prompt doesn't ask about phased product strategy or MVP scope.
- **Suggested prompt change:** Add validation question in "Проверьте наше понимание" section: "Какой минимальный продукт вы планируете выводить первым? Полный scope или упрощённая версия?" Then adjust positioning to match actual Phase 1 product, not full roadmap.
- **Status:** ⬜ Not yet resolved

---

## Theme: Primary segment framing — company type vs buyer role confusion

- **NapoleonIT** (v4, 2026-02-16): Doc said "генподрядчики с BIM (ТОП-200 России)" as Primary. Client corrected: "Стройконтроль (гос и частный) думаю они ключевые в этой технологии"
- **Impact:** 🟡
- **Pattern:** "Генподрядчик" is a company type. "Стройконтроль" is a function/role. The positioning conflates company segment with buyer persona. Client thinks the ROLE (construction control inspector) is primary, not the company type.
- **Suggested prompt change:** In segment validation, separate two questions: (1) Company type/segment (генподрядчики, промышленность, etc.) (2) Buyer persona/role (стройконтроль, директор по строительству, etc.). Don't conflate them.
- **Status:** ⬜ Not yet resolved

---

## Theme: Use case scope too narrow — GPS-denied outdoor not captured

- **NapoleonIT** (v4, 2026-02-16): "На самом деле мы можем траекторию прострагивать и на открытых пространствах, это особенно актуально в москве где GPS сейчас глушат"
- **Impact:** 🟢
- **Pattern:** Positioning focused on "indoor where GPS doesn't work". Missed outdoor use case where GPS is jammed (real problem in Moscow). This expands addressable market.
- **Suggested prompt change:** In use case discovery, ask explicitly: "Работает только indoor или также outdoor? Есть ли сценарии где GPS недоступен по другим причинам (глушилки, помехи)?"
- **Status:** ⬜ Not yet resolved

---

## Theme: Agent produces generic positioning — doesn't understand product differentiation

- **RAGProduct/Лёша** (v3, 2026-02-19): "он слабо понял продукт и он слабо понял дифференциацию вообще, что зачем... предложил такую усредненно говняную формулу монетизации... очень примитивная, неизощренная"
- **Impact:** 🔴
- **Pattern:** Agent output feels generic and "averaged" — doesn't capture what makes this specific product different. Client expected agent to deeply understand differentiation and produce non-obvious, tailored recommendations. This may indicate agent doesn't ask enough probing questions about competitive positioning or unique value props.
- **Suggested prompt change:** Add explicit requirement for agent to: (1) Identify and articulate what's UNIQUE about this product vs alternatives, (2) Challenge generic formulations, (3) Ask follow-up questions if differentiation is unclear from input materials.
- **Status:** ⬜ Not yet resolved

---

## Theme: Segments too abstract — need concrete verticals with expressed pain

- **RAGProduct/Лёша** (v3, 2026-02-19): "сегменты просто ужас... вообще не сегменты... Компания без сильной ИТ экспертизы, например: ферма с коровами, там 50 человек, неплохая выручка, но им ИИ нах не нужен. Сегмент хреновый. Или Торговый дом, где менеджеры целый день звонят — там наш продукт как нельзя к стати"
- **Impact:** 🔴
- **Pattern:** Agent segmented by company SIZE (50+ employees) and LACK of capability (no IT team). Client says this is wrong — segment by ACTIVITY TYPE and EXPRESSED PAIN. Farm with 50 people = bad segment. Trading house with sales reps = good segment. Size/capability are secondary to business activity.
- **Suggested prompt change:** In Target Segments section, require agent to: (1) Identify segments by ACTIVITY/VERTICAL first, then filter by size/capability, (2) For each segment, explicitly state the PAIN POINT that makes product relevant, (3) Include counter-examples (who looks like the segment but ISN'T a fit).
- **Status:** ⬜ Not yet resolved

---

## Theme: Value prop focuses on wrong pain — bottlenecks > onboarding

- **RAGProduct/Лёша** (v3, 2026-02-19): "помимо онбординга, боттлнеки. 5 бухгалтеров могут заддосить юриста запросами. Вместо этого юрист готовит базу для ИИ и бухгалтера сначала работают с ИИ... юрист только быстро вникает в контекст и говорит да нет"
- **Impact:** 🟡
- **Pattern:** Agent emphasized "onboarding" and "knowledge transfer" as main pain points. Client corrected: main pain is BOTTLENECKS — experts being overloaded by routine requests. The accountant/lawyer example is a concrete, relatable pain story.
- **Suggested prompt change:** In pain discovery, ask about: (1) Who are the internal "experts" everyone goes to? (2) How much of their time is spent on routine requests? (3) What happens when they're unavailable? These questions surface bottleneck pain better than generic "slow onboarding".
- **Status:** ⬜ Not yet resolved

---

## Theme: Product scope broader than RAG — AI assistant capabilities underrepresented

- **RAGProduct/Лёша** (v3, 2026-02-19): "это не только RAG, но и ИИ в чистом виде. Он подготовит ответ на письмо, даст справку и поищет в интернете, суммаризирует документ, предложит варианты решения вопросов, снижает количество боттлнеков"
- **Impact:** 🔴
- **Pattern:** Agent framed product as "RAG system with role-based access". Client says it's broader: AI assistant that writes emails, analyzes conversations, summarizes docs, suggests solutions. RAG is just one capability. This affects positioning dramatically — it's not a "knowledge base", it's an "AI work assistant".
- **Suggested prompt change:** In product capability discovery, explicitly map capabilities to: (1) Internal data access (RAG), (2) External data access (web search), (3) Content creation (writing, summarization), (4) Analysis (conversation analysis, pattern detection). Don't assume product is single-purpose.
- **Status:** ⬜ Not yet resolved

---

## Theme: Copilot comparison wrong for RU market — no dominant players

- **RAGProduct/Лёша** (v3, 2026-02-19): "Сравнение с Copilot — проиграете по функциям и бренду / только по бренду и то возможно. В рынке РФ нет игроков, которые бы захватили рынок ИИ интеграции и трансформации. Ну разве что Just AI"
- **Impact:** 🟡
- **Pattern:** Agent wrote "vs Copilot — you'll lose on features and brand". Client corrected: RU market is EMPTY. Copilot is not a real threat in Russia. Just AI is the only notable player. This changes competitive framing entirely.
- **Suggested prompt change:** In competitive analysis, explicitly ask: "What geography is this for?" and adjust competitor landscape accordingly. For RU market, don't assume global players (Copilot, OpenAI) are the main competition.
- **Status:** ⬜ Not yet resolved

---

## Theme: Segment-specific positioning required — one-size-fits-all doesn't work

- **RAGProduct/Лёша** (v3, 2026-02-19): "под каждый сегмент из пункта 4 готовятся свои метрики... предложение для девелопера будет сильно отличаться от предложения для торгового дома. а они могут выглядеть как один сегмент"
- **Impact:** 🟡
- **Pattern:** Agent produced one positioning statement for all segments. Client says each segment needs its own: (1) Market category, (2) Metrics/proof points, (3) Value proposition. Developer ≠ trading house even if both are "50+ employees without IT".
- **Suggested prompt change:** In positioning doc structure, explicitly note: "This positioning may need segment-specific variants. For each segment, consider whether a separate value prop, market category, or proof point set is needed."
- **Status:** ⬜ Not yet resolved
