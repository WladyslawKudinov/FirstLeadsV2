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
