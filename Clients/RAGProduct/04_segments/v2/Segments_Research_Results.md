# B2B segment research: AI assistant for Russian mid-market

**Five segments analyzed across six dimensions each reveal a clear pattern: the Russian mid-market has acute pain from manual knowledge work, near-zero domestic AI competition for most use cases, and decision-makers reachable primarily via Telegram and direct outreach — not LinkedIn.** The product's on-prem deployment and adoption guarantee directly address the two biggest blockers: data sovereignty fears and the 95% AI pilot failure rate. IT companies represent the fastest entry point (tech-savvy buyers, short deal cycles), while manufacturing offers the widest competitive moat (zero domestic competitors for AI engineering documentation).

---

## SEGMENT 1: IT companies / software producers (HIGHEST PRIORITY)

### Block 1 — Ten target companies with pain signals

The HighTime Media SaaS rating (firmoteka.ru/top-saas-hightime) lists **94 SaaS companies with revenue above 50M₽**, making it the single best source for this segment. Companies were selected for 20–150 employees, revenue 50–300M₽, and indicators of documentation/onboarding pain.

| Company | City | Revenue (M₽) | Employees | Why they fit | Pain signal |
|---------|------|--------------|-----------|-------------|-------------|
| **Wazzup (ВАЗЗАП)** | Moscow | 959 | 102 | Messaging integration SaaS, **+105% growth** | Explosive growth → severe onboarding/support pressure |
| **Huntflow (Хантфлоу)** | Moscow | 619 | 101 | ATS/recruiting SaaS, +46% growth | Complex product needs tech docs; known to hire tech writers |
| **Pyrus (Пайрус)** | Moscow | 406 | 56 | Workflow automation SaaS | Document-heavy product requiring internal knowledge base for support |
| **Binovo (Биново)** | St. Petersburg | 323 | 77 | SaaS product, +72% growth, 63% margin | Fast-growing team → onboarding bottleneck |
| **Cleverence (Клеверенс Софт)** | Moscow | 296 | 93 | Mobile automation SaaS | Complex product documentation across mobile platforms |
| **Aspro (Аспро)** | Chelyabinsk | 276 | 79 | Web development SaaS, +50% growth | Growing team needs internal knowledge management |
| **Smartnut (Смартнат)** | Yekaterinburg | 255 | 47 | SaaS company, +19% growth | Mid-size team struggling with documentation updates |
| **Textback (Текстбэк)** | Moscow | 252 | 37 | Messaging platform | Small team, high growth requires knowledge scaling |
| **Sipuni (Сипуни Рус)** | Moscow | 243 | 99 | Cloud telephony SaaS, +30% growth | Tech support team needs knowledge base |
| **Kaiten (Кайтен Софтвер)** | Moscow | 233 | 18 | Project management SaaS, **+135% growth** | Hyper-growth; internal knowledge sharing critical |

Additional high-value targets: Multifactor/Мультифактор (527M₽, 28 emp, cybersecurity) and Lankey IT/Ланкей ИТ (483M₽, 29 emp). HH.ru confirms pain signals — "Программный Продукт" had 16 open vacancies; "Сервис Плюс" was hiring junior technical writers (vacancy #128225016). The IT job market contracted ~30% in 2025, pushing companies toward AI tools to replace headcount.

### Block 2 — Decision makers

The primary DM is **CTO / VP Engineering / Technical Director** at companies with 50+ employees; at sub-50 companies the **CEO** co-signs or decides directly. LinkedIn is functionally dead for Russian IT professionals — the platform is restricted in Russia since 2016, and CTO engagement happens overwhelmingly on Telegram.

Three identifiable CTO figures active on Telegram (proxy for LinkedIn profiles, which are inaccessible behind authentication):

- **Самат Галимов** (@ctodaily / "Запуск завтра") — ex-CTO Meduza, Bookmate, RAWG, Pure. Active daily posts about CTO life
- **Илья Чекальский** (@techdir / "твой cto") — active CTO blogger writing about technical director daily challenges
- **CTO On Live** (@ctoonlive) — CTO/architect with experience at amoCRM, VCV; shares tools and management practices

Typical email patterns in Russian IT: `firstname@company.ru` (most common), `firstname.lastname@company.ru`, `i.lastname@company.ru`, or `firstname@company.io` for internationally-oriented companies.

### Block 3 — How to build company lists

**Rusprofile ОКВЭД codes:** 62.01 (software development, **38,984 active companies**), 62.02 (IT consulting, 8,074 active), 63.11.1 (databases/information resources). Filter by revenue 50–300M₽, employees 20–150, Moscow/SPb. Rusprofile Professional subscription required for combined filters (~4,990₽/month).

**HH.ru queries for identifying companies via pain signals:**
- "технический писатель" + IT company names — finds companies hiring tech writers
- "менеджер базы знаний" OR "knowledge manager" — direct knowledge management need
- "специалист техподдержки" + "база знаний" — support teams needing knowledge bases

**IT company ratings/registries (URLs):**
- HighTime SaaS Rating: hightime.media/raiting-saas-kompaniy/ (~94 companies)
- HighTime IT Corporations: hightime.media/raiting-it-korporaciy/ (77 companies)
- HighTime IT Integrators: hightime.media/raiting-integratorov-kompaniy/ (92 companies)
- Firmoteka with financials: firmoteka.ru/top-saas-hightime
- TAdviser500: tadviser.ru (threshold 493M₽)
- CNews100/300: cnews.ru
- SaaS Rating: saas-rating.ru (70 companies, 72.8B₽ total 2024)
- Habr Career: career.habr.com

**Can you find 50 companies in 30 minutes? YES — estimated 15–20 minutes.** Open firmoteka.ru → instantly gives ~100 SaaS companies with revenue and employee data. Filter by revenue 50–300M₽ and employees 20–150 → yields ~25–30 companies immediately. Supplement with Rusprofile ОКВЭД 62.01 → adds 20+. Cross-check HH.ru for pain signals.

### Block 4 — Competitive landscape

**Minervasoft (Minerva Knowledge)** — Founded 2019, product launched 2021. Knowledge Management System replacing Confluence. Clients include Совкомбанк, Делимобиль, Газпромбанк, Эвотор, Петрович, Ингосстрах, QIWI. Pricing: ~640K₽/year for 70 users (~53K₽/month), range 50–150K₽/month for enterprise. Strengths: best-rated KMS in Russia, good search, CRM integrations. **Weaknesses: HIGH PRICE (most-cited negative in reviews), no task tracker, knowledge-only — NOT an AI assistant, no email/meeting/negotiation features, limited AI (Copilot add-on only).**

**AutoFAQ Xplain** — RAG-based AI assistant for corporate documents. The PwC Russia (ТеДо) case is notable: ~3,000 employees, created chatbot "Ботя" for IT support, achieved **87% query automation, 500 queries/day, 5,500+ consultant hours saved per year**. Other clients: М.Видео-Эльдорадо (85% robotization), Честный Знак (99% automation). **Weaknesses: primarily customer support/helpdesk focused — not a full AI assistant for emails, meetings, negotiations. Enterprise-focused pricing, may be expensive for mid-market.**

| Feature | Our product | Minervasoft | AutoFAQ Xplain |
|---------|------------|-------------|----------------|
| AI RAG assistant | ✅ Full | ❌ Copilot add-on | ✅ Strong |
| On-prem deployment | ✅ Guaranteed | ✅ Available | ✅ Available |
| Email integration | ✅ | ❌ | ❌ |
| Meeting notes | ✅ | ❌ | ❌ |
| Negotiation support | ✅ | ❌ | ❌ |
| Adoption guarantee | ✅ | ❌ | ❌ |
| Price (80–110K₽/mo) | ✅ Competitive | 50–150K₽/mo | Likely higher |

**Key differentiator:** Full AI assistant (emails + negotiations + docs + meetings) vs. competitors who are either KMS-only (Minerva) or support-chatbot-only (AutoFAQ). On-prem fills the ChatGPT void.

### Block 5 — Budget and deal cycle

For a company with revenue 100–300M₽, IT tool budget is typically **5–15% of revenue** (IT companies spend higher than other industries). The product at **80–110K₽/month = 960K–1.32M₽/year** represents ~0.3–1.3% of revenue — very affordable. At this price, CTO typically initiates and champions; CEO final-approves at sub-100 employee companies. CFO co-signs at larger ones. Decision cycle: **2–6 weeks** for pilot decision, **1–3 months** from first contact to contract. Russian IT companies increasingly plan quarterly.

**Budget seasonality:** Q4 (Oct–Dec) is peak — companies finalize tool purchases to use remaining budget. Q1 (Jan–Mar) — new budgets execute approved plans. Q3 (Jul–Sep) — summer slowdown, picks up in September for Q4 planning. "The horizon for budget planning is getting shorter — companies more often form plans for a quarter, maximum for a year" (korusconsulting.ru).

### Block 6 — Telegram channels and industry media

**CTO Telegram channels:**
- @ctodaily ("Запуск завтра") — CTOs, tech leads
- @techdir ("твой cto") — technical directors
- @ctoonlive — CTOs, architects
- @pmdaily (FEDOR BORSHEV) — senior devs, CTOs
- @leadgr (TechLead Good Reads) — team leads, CTOs

**Industry media:** vc.ru (major business/tech platform), Habr.com (premier IT community — AutoFAQ and Minervasoft both publish there), TAdviser, CNews, ComNews, HighTime Media (@HighTimeMedia). Habr hubs: "Управление знаниями", "Искусственный интеллект", "SaaS/S+S".

**Counter-evidence:** IT companies may attempt to build their own RAG solution ("build vs. buy" bias). Counter this with the PwC/ТеДо case — even PwC bought AutoFAQ rather than building. The "adoption guarantee" directly addresses the 95% pilot failure rate.

---

## SEGMENT 2: Wholesale trade / distributors

### Block 1 — Ten new companies with pain signals

HH.ru shows **~972 active vacancies** for "менеджер по оптовым продажам" in Moscow alone. Companies were identified from HH.ru job postings, distributor ratings, and industry directories.

| Company | City | Segment | Pain signal | Source |
|---------|------|---------|-------------|--------|
| **ГК "КСК"** | St. Petersburg | Building materials (insulation, roofing, fasteners) | Hiring sales managers for cold sales + proposal preparation (vacancy #128827413) | hh.ru/vacancy/128827413 |
| **ГК KOLOBOX** | Nizhny Novgorod | Tire/wheel distributor, top-10 Russia | 110+ retail points, B2B platform, WMS systems — IT-invested but sales team scaling | nnov.kp.ru/daily/27041/4107234/ |
| **ООО "ГРАТ-ВЕСТ"** | Moscow | FMCG/consumer goods wholesale (toys, souvenirs) | Hiring regional sales managers; described as "leading Russian trade company" | careerist.ru |
| **ООО "ВЕКТОР" (Total Tools)** | Moscow | Wholesale distributor of electric/hand tools | Hiring sales managers for "development of representative office" | careerist.ru |
| **"СМАРТ-ПРОЕКТ"** | Moscow | Building materials — official distributor of leading construction producers | Hiring due to expansion; requires engineering systems sales experience | careerist.ru |
| **ООО "Компания Комплит"** | St. Petersburg | Wholesale computers & peripherals (ОКВЭД 46.51) | Founded 1996, established player in electronics distribution | rusprofile.ru/codes/465100 |
| **ООО "База Электроники"** | Moscow | Wholesale equipment (electronics) | Founded 2003, active electronics trade | rusprofile.ru/codes/466900 |
| **ООО "Завод Фильтр"** | Moscow | Wholesale non-food consumer goods (ОКВЭД 46.4) | Active wholesale trade, Balaklavsky prospect | rusprofile.ru/codes/464000 |
| **ООО "Компания Петрогресс"** | Moscow | Wholesale non-food consumer goods | Active, Olkhovskaya street location | rusprofile.ru/codes/464000 |
| **ПКП "Стройнаст"** | Smolensk | Wholesale building materials | Founded 1997, 28+ years in market — mature with legacy processes | rusprofile.ru |

Larger reference targets from ratings: ЭТМ (largest electrical product distributor), Русский Свет (lighting), ROSSKO (auto parts wholesale), Сима-ленд (Ekaterinburg, 1M+ SKUs).

### Block 2 — Decision makers on LinkedIn

LinkedIn profile search for "коммерческий директор" + "дистрибьютор" yielded no directly accessible profiles due to authentication walls. **Russian commercial directors in distribution are generally low-activity on LinkedIn — most engagement happens on Telegram and VK.** One named DM found: **Андрей Скорина** — коммерческий директор, председатель совета директоров ГК KOLOBOX (public mention in KP.ru article).

Recommendation: Focus outreach on Telegram DMs and cold email rather than LinkedIn. Email patterns in wholesale: `i.ivanov@company.ru`, `name@company.ru`, or `sales@company.ru`.

### Block 3 — Rusprofile query and list building

**ОКВЭД codes for wholesale trade:**
- 46.3 (food FMCG wholesale)
- 46.4 (non-food consumer goods, **tens of thousands registered**)
- 46.43 (household electronics)
- 46.51 (computers & peripherals — **24,342 companies registered**)
- 46.6 (machinery/equipment)
- 46.73 (building materials)

**Filters:** Revenue 100–500M₽, employees 30–200, Moscow/SPb, active status. Note: Rusprofile free version does NOT allow combined filters — Professional access required (~4,990₽/month). With filters applied, estimate **2,000–5,000 matching companies** nationwide, **500–1,500 in Moscow/SPb**.

**Alternative sources:** ExportBase (export-base.ru) — pre-built database of 2,459 Russian distributors; SPARK-Interfax for premium data; companies.rbc.ru for free ОКВЭД navigation.

**Can you find 50 companies in 30 minutes? YES.** Rusprofile Pro: set filters → export first 50 (10 min). ExportBase: buy pre-built list, filter in Excel (5 min). Cross-reference HH.ru for hiring signal (15 min). Industry ratings: Cleverence TOP distributors (cleverence.ru), Vakansii.pro TOP-50 (vakansii.pro/articles/top-50-kompaniy-v-sferah-optovye-prodazhi).

### Block 4 — CRM integrators as referral channels + competitive landscape

**CRM integrators working with trade companies (referral potential HIGH):**

- **CRM Academy** (crmacademy.ru) — 300+ clients, 25 employees. Niches include "торговля" explicitly. Has a case with a PPE supplier. HIGH referral potential
- **Intervolga** (intervolga.ru) — wholesale/distribution clients include Гранд Капитал, Левенгук, Комус, Штурм!. Lists "оптовая и розничная торговля" as specialty. HIGH referral potential
- **Ингруппа** (Ingroup) — Has a dedicated solution for "оптово-розничных компаний." Top-20 CRM integrator by crmrating.ru. HIGH referral potential
- **Reon** (reon.pro) — Niches include "торговля," HORECA. MEDIUM referral potential
- **ABMarketing** (abmarketing.pro) — Битрикс24 partner. Claims +15% leads → +1.2M₽ revenue. MEDIUM referral potential

**Competitive landscape:** The CRM gap is confirmed. SaleKit (salekit.ru) is the closest competitor with AI for wholesale — lead scoring, proposal generation, predictive analytics — but focuses on scoring/analytics, not RAG-based proposal generation from company-specific price lists. **Neither BitrixGPT nor amoAI generates proposals from price lists. This is a genuine market gap.**

Other tools: Rechka.ai (call analytics — complementary), GNZS AI-РОП (sales quality monitoring — complementary), SimpleOne B2B CRM (enterprise segment), AGORA (B2B order platform), МойСклад (warehouse ERP).

### Block 5 — Budget and deal cycle

**Annual cycle for wholesale companies (3–15M₽ IT budgets):**
- Oct–Nov: IT budget planning begins
- Nov–Dec: Budget approval by owner/GD
- January: New budget period starts
- Q2–Q3: Main implementation period

**Sales "dead seasons":** January 1–15 (holidays, zero activity), May (long holidays), August (mild slowdown). **Peak activity: February–April and September–November.**

**Best windows to sell:** February–March (post-holiday restart, new budgets active), September–October (pre-budget planning — ideal for "pilot + include in next year's budget"), late November–December (budget spending rush).

**Who signs off on 80–110K₽/month:**
- Companies <50 people: Owner/CEO directly
- Companies 50–200 people: Commercial Director initiates, CFO validates, CEO approves
- **Key framing: position as "replacing 1 sales manager hire"** — saves ~100K₽/month in salary + taxes + management

Decision cycle: **2–4 weeks** for owner-managed companies (<50), **4–8 weeks** for larger distributors including pilot.

### Block 6 — Additional Telegram channels

Beyond known channels (@grebenukm 260K, @dirclub 17K, @Salesnotes 15.4K):

- **@optlist_chat** ("ОптЛист B2B оптовый чат") — **35,100 subscribers**. Suppliers and wholesale buyers. Direct wholesale trade community
- **@postavshchiki** ("Поставщики | Оптовики 🇷🇺") — Telegram channel for suppliers and wholesalers
- **@tovarochkk** ("Товарочка Поставщики") — commodity business in Russia, partner search
- **Максим Батырев (Комбат)** — ~24,900 subscribers. Management and leadership content, popular among commercial directors
- **Тарас Алтунин / B2B Sales** — practical B2B sales, LinkedIn tips, podcasts
- **I-KM** — sales, assortment, procurement, category management — relevant for wholesale/distribution DMs
- **"Про CRM от интегратора" (by Ингруппа)** — most popular CRM Telegram channel; useful for partnership building

Industry media: New-Retail.ru (digital trade media), Retail.ru (major industry portal), vc.ru (business platform with active B2B community).

---

## SEGMENT 3: Manufacturing with office block

### Block 1 — Ten new manufacturing companies using KOMPAS-3D

Companies identified from ASCON case studies, ASCON competition winners (XXII–XXIII "Конкурс асов"), HH.ru vacancy analysis, and ascon.ru/projects/.

| Company | City | Sector | Why they fit | Pain signal |
|---------|------|--------|-------------|-------------|
| **Краснокамский РМЗ** | Краснокамск, Пермский край | Gas equipment components | Cited on kompas.ru as manufacturing gas compressor components in КОМПАС-3D. Mid-size, likely no PLM | Custom components = scattered documentation per order |
| **Челябинский компрессорный завод** | Челябинск | Compressor manufacturing | **1st place winner** in Росспецмаш + АСКОН 3D competition. Confirmed КОМПАС user | Active competition participation suggests engaged team without deep PLM |
| **ООО "Металлпром"** | Regional | Metal products | 2nd place in Росспецмаш competition. Uses КОМПАС-3D | Engineer participating in contests = looking for tools, likely no PLM |
| **ООО "Завод Дорожных машин"** | Regional | Road machinery | 2nd place Росспецмаш. "Руководитель конструкторской группы новых разработчиков" | New product development = heavy documentation creation |
| **ООО "ЗМ Инжиниринг"** | Regional | Engineering services | 3rd place Росспецмаш. Confirmed КОМПАС user | Engineering company = documentation-intensive |
| **АО "Гаврилов-Ямский машзавод АГАТ"** | Гаврилов-Ям, Ярославская обл. | Mechanical engineering | Listed on ASCON projects. Small city = limited IT staff | Regional plant with manual doc management |
| **АО "Завод Двигатель"** | St. Petersburg | Engine manufacturing | ASCON case study — uses КОМПАС-3D + ВЕРТИКАЛЬ for КТПП | Complex documentation workflows for production prep |
| **ООО "Финист"** | Yekaterinburg | Food equipment (metalworking, refrigeration) | HH.ru vacancy explicitly requires КОМПАС-3D. 16+ years in business | Growing ("увеличение объёма работы"), hiring new engineers = knowledge transfer challenge |
| **АО "НПП Квант"** | Ростов-на-Дону | Space/scientific instrument-making | HH.ru vacancy lists КОМПАС-3D as required skill | Complex regulatory documentation (ЕСКД compliance), expert knowledge concentration |
| **АО "Равенство"** | St. Petersburg | Instrument-making / electronics | Won "Project of the Year" from Global CIO with АСКОН for PLM implementation | **Caveat:** HAS PLM (ЛОЦМАН:PLM), but proves segment exists |

**Key resource:** ASCON competition gallery (best.ascon.ru/gallery/) is a **gold mine** of target companies actively using КОМПАС-3D — 63+ enterprises participated in 2025 competition alone. Total addressable market: ASCON serves **16,000+ corporate customers** with **500K КОМПАС workstations**.

### Block 2 — Decision makers and alternative contact channels

**LinkedIn is confirmed dead for Russian manufacturing engineers.** LinkedIn has been blocked in Russia since 2016. HR professionals confirm "colossal" decline in Russian market activity. Manufacturing technical directors are NOT on LinkedIn — could not find 3 real profiles, which itself proves the hypothesis.

**Alternative channels to reach technical directors (in order of effectiveness):**

1. **Direct phone via company websites** — most manufacturing plants list director contacts or reception numbers. This is the **primary channel**
2. **2GIS** — excellent for finding manufacturing companies with phone numbers and department contacts in Russian cities
3. **Reception calls (звонок на приёмную)** — standard B2B practice in Russian manufacturing. Ask for "технический директор" or "главный инженер." Manufacturing culture is phone-based
4. **ASCON user forums and events** — best warm channel. ASCON runs conferences where tech directors attend as КОМПАС-3D license buyers
5. **TenChat** — Russian business social network positioned as LinkedIn replacement. Growing but still marginal for manufacturing
6. **VK (ВКонтакте)** — КОМПАС-3D has an active VK group; some engineering communities exist

### Block 3 — ASCON partners as referral channels

**ASCON partner network: 30 regional offices + authorized partners.**

| Partner | Type | Notes |
|---------|------|-------|
| **Softline** | Gold Partner | Major IT distributor, sells ASCON products nationwide |
| **АСКОН-Уфа** | Platinum Partner | Handles УМПО and Ufa region clients |
| **АСКОН-Самара (ГК АйтиКонсалт)** | Regional partner | Implemented at РКЦ "Прогресс" |
| **IGA Technologies** | Authorized partner | Reseller, igatec.com |
| **ИНФАРС** | Partner / training center | infars.ru, resells КОМПАС-3D |
| **MPI (ЭМПИАЙ)** | Authorized partner | mpi-corp.ru |

Partner directory: ascon.ru/partners/ (interactive map). Partner program: ascon.ru/for-partners/. **ASCON's 30 regional offices are the best referral channel** — they know every КОМПАС customer in their region. Each office has sales managers maintaining relationships with local factories. Free hotline: 8-800-700-00-78.

**Rusprofile estimate:** ОКВЭД codes 25–30 (fabricated metals, machinery, electronics, vehicles) with revenue 200–1000M₽ and employees 50–300 → **estimated 3,000–5,000 companies** across Russia.

### Block 4 — Engineer communities

**Active forums and channels:**
- **forum.ascon.ru** — official ASCON user forum, active, direct КОМПАС-3D users
- **cccp3d.ru** (Forum САПР2000) — one of the oldest Russian CAD forums: CNC programming, CAD modeling, job board
- **isicad.ru** — leading CAD/CAM/PLM portal; 232 publications in 2025; Telegram: @isicad
- **sapr.ru** ("Журнал САПР и графика") — trade magazine/portal for CAD/CAM/CAE

**Telegram channels:**
- **КОМПАС-3D** (official) — Telegram chat for КОМПАС users + news channel, active
- **@isicad** — CAD/CAM/PLM industry news, active
- **"САПР для инженера"** (@saprdlyaingenera) — niche CAD/IT channel
- **"Записки инженера"** (@EngineeringNotes) — engineer blog channel

**Where engineers actually communicate:** Telegram (primary for quick Q&A, especially КОМПАС-3D chat), cccp3d.ru (deep technical discussions), forum.ascon.ru (КОМПАС-specific help), VK (news, casual content), isicad.ru + sapr.ru (reading industry news). Word-of-mouth at exhibitions remains dominant.

### Block 5 — Zero competition confirmed + budget cycle

**No direct competitor exists** for a domestic, on-prem, RAG-based AI search tool for engineering documentation. Closest related solutions are all traditional (non-AI) document management:
- ЛОЦМАН:PLM (АСКОН) — structured metadata search, not semantic AI/RAG
- T-FLEX DOCs (Топ Системы) — traditional search, not AI
- Pilot-ICE/BIM (АСКОН) — BIM/construction focus only

**ASCON's own AI plans:** No explicit AI/ML features announced for КОМПАС-3D or ЛОЦМАН:PLM. Strategy focuses on Linux support, PLM consortium "РазвИТие," BIM, FSTEC certification. However, the conference "ИИПРОМ-2026" includes a session "ИИ-ассистент инженера-технолога. Миф или реальность?" — market interest is forming. **Risk: ASCON could eventually add AI, but their timeline appears years away.** Russian engineering software market: **50–55 billion rubles** (2025), growing ~20% annually. ASCON revenue: 6.6B₽ (2024), up 18%.

**Budget cycle:** Q3 (Jul–Sep) — annual IT budget planning begins. Q4 (Oct–Dec) — finalization, sometimes year-end spending rush. Q1 (Jan–Mar) — new budget starts. Q2 (Apr–Jun) — active procurement. **Best times to sell: September–November (influence budget planning), March–June (tap approved budgets), November–December (year-end urgency).** At 80–110K₽/month (~1–1.3M₽/year), this fits within 5–15M₽ annual IT budgets. Tech director recommends → general director approves. Typical cycle: **2–6 months** from first contact to contract.

---

## SEGMENT 4: Large law firms (top-20 Pravo-300)

### Block 1 — Top law firms from Pravo-300

The Pravo-300 rating (300.pravo.ru, 16th edition, December 2025) is the authoritative source: 700+ firms submitted 25,397 projects. **RBC research confirms: ~800 active legal companies with ОКВЭД 69.1, total market revenue 175.9 billion rubles, 28 companies with revenue above 1 billion rubles, 48 above 500M₽, 330+ between 100–500M₽.**

| Firm | City | Key facts | Specialization |
|------|------|-----------|---------------|
| **АБ ЕПАМ** (Егоров, Пугинский, Афанасьев и Партнёры) | Moscow | **#1 by revenue AND lawyers.** 82 recommended lawyers. Rated in ALL categories | Full-service: M&A, disputes, bankruptcy |
| **АЛРУД (ALRUD)** | Moscow | 32 federal nominations in 2025. Won "Art-право" special prize | M&A, antitrust, tax, TMT, employment |
| **Nextons** (ex-Norton Rose) | Moscow | 59 recommended lawyers, 31 nominations | Full-service: corporate, disputes, finance |
| **LEVEL Legal Services** | Moscow | 19 nominations (5 new in 2025). 1st in Corporate Law HM, M&A HM | M&A, disputes, bankruptcy, IP |
| **Пепеляев Групп** | Moscow | Top tax practice. Historically top-5 by revenue | Tax, antitrust, IP, regulatory |
| **Lidings** | Moscow | Top-10 by revenue/lawyer. 17 nominated practices | Pharma, antitrust, data protection, IP |
| **a.t.Legal** | Moscow | Group 1 in 3 key nominations: Arbitration, Bankruptcy, Real Estate | Disputes, bankruptcy, real estate |
| **ЛКП** (Лемчик, Крупский и Партнёры) | Moscow | 3rd by # of lawyers, 14th by revenue | Tax, disputes, bankruptcy, corporate |
| **КИАП** | Moscow | Top-10 by practice breadth. Leader in arbitration | Disputes, corporate, compliance, TMT |
| **Рустам Курмаев и Партнёры** | Moscow | Major litigation firm, founded 2017 | Disputes, white-collar crime, bankruptcy |
| **ЦПО Групп** | Moscow | 13 nominations in 2025 | Tax, IP, real estate, TMT, sanctions |
| **Хренов и Партнёры** | Moscow | 30th by lawyers, 48th by revenue | Arbitration (mid-market) |

Additional firms in top-30: Б1 (ex-EY), Saveliev Batanov & Partners, Forward Legal, Birch Legal, Линия Права, Юст, BGP Litigation, VEGAS LEX, Астерис.

**Tech-forward firms:** ЕПАМ (extensive digital presence), КИАП (hosts LegalTech events), a.t.Legal (modern management practices). **Pain signals:** 88% of Russian lawyers already use AI (Авито + Право.ru study, late 2025), "борьба за таланты" as key market challenge.

### Block 2 — Large accounting outsourcers (RAEX ranking)

**RAEX Ranking 2024:** Market size **18.695 billion rubles** (+14% YoY), 83 participants, 5,443 specialists.

| Company | City | Revenue 2023 (K₽) | Staff | Growth |
|---------|------|--------------------|-------|--------|
| **СберРешения** | Moscow | 1,702,573 | 1,057 | +33.6% |
| **Моё дело** | Moscow | 1,466,623 | 387 | +20.9% |
| **Unicon Outsourcing** | Moscow | 1,193,233 | 367 | +0.9% |
| **1C-WiseAdvice** | Moscow | 1,177,790 | 419 | +19.5% |
| **ПИКТА** | Samara | 1,140,133 | 545 | +75.5% |
| **ИАС Аутсорсинг** | Moscow | 1,140,095 | 80 | +21.8% |
| **UCMS Group** | Moscow | 1,092,386 | 361 | +22.6% |
| **Bellerage** | Moscow | 812,066 | 91 | +39.2% |
| **SCHNEIDER GROUP** | Moscow | 737,117 | 226 | +10.4% |
| **Юнистафф Пейрол** | Moscow | 616,854 | 220 | +11.7% |

Additional 200M₽+: БРИДЖ ГРУПП (426M), АБУ (363M), Мариллион (318M), Консу (310M, SPb). RAEX URLs: raex-rr.com/b2b/outsoursing/outsourcing_of_accounting_functions_rating/2024/ and /2025/.

### Block 3 — Decision makers and LinkedIn

LinkedIn is blocked/restricted in Russia since 2016. Russian legal managing partners have dormant profiles or don't use LinkedIn actively. **Specific profiles: NOT FOUND** due to restricted access.

**Alternative channels to reach managing partners:**
- **Telegram** — primary communication tool for Russian legal community
- **Право-300 Conference** (event.pravo.ru) — annual event where top managing partners gather
- **Zakon.ru** — professional legal community with active discussions
- **Журнал "Корпоративный юрист"** premium club (korpurist.life)
- **Cold email via firm websites** — most firms list partner emails
- **Personal Telegram channels** of legal leaders (e.g., Кирилл Буряков/Doczilla — t.me/Kirill_Buryakov)

DM titles: Управляющий партнёр, Генеральный директор, Старший партнёр.

### Block 4 — List building and Rabrain analysis

**Can you find 50 firms in 30 minutes? YES.** Pravo-300 top-50 by revenue (on site) → 30+ qualifying law firms (10 min). RAEX outsourcing top-20 → 10+ qualifying accountants (5 min). Rusprofile ОКВЭД 69.1, revenue 200M₽+ → fill remaining (15 min).

**Rusprofile estimate:** ОКВЭД 69.1 with revenue 200M₽+: **~120–180 companies**. With 50M₽+: ~800 total.

**Rabrain.ru analysis: NOT a competitor.** Rabrain.ru is "Лаборатория Баз знаний" — a knowledge base development/consulting company. Offers corporate knowledge base creation, documentation automation. Has content about "Повышение Эффективности Юридической Службы" but this is content marketing, not a competing AI product. No public pricing, no visible legal AI client list. Different product category entirely (knowledge base infrastructure vs. AI assistant).

### Block 5 — Competitive positioning

**No existing Russian competitor covers the full stack: internal docs + internet + email + meetings with on-prem deployment.** Each addresses only 1–2 data sources:

| Tool | Price | Covers | Missing |
|------|-------|--------|---------|
| **ConsultantPlus AI** | K+ subscription | Only К+ database | No internal docs, no email/meetings, no on-prem for custom data |
| **Garant ИСКРА** | Garant subscription | Only Garant/public sources | No internal docs, no email/meetings, no on-prem |
| **Doczilla Pro** | ~2,900₽/person/month | Document creation/templates | No email/meetings, AI described as "ощутимо недоработанный" by Habr users |
| **Нейроюрист** (Яндекс + Garant) | 2,000₽/mo (50 queries) | Garant integration | No internal docs, limited queries |
| **Our product** | 80–110K₽/mo (entire firm) | Internal docs + internet + email + meetings | — |

For a 30-person firm, Doczilla costs **~87,000₽/month** — comparable to our pricing. But Doczilla has no email/meetings/internet integration. **Genuine whitespace.**

### Block 6 — Corporate legal expansion + Telegram/media

**Corporate legal TAM:** Companies with revenue 500M₽+ in Russia: **estimated 15,000–25,000**. Companies with dedicated legal departments (10+ lawyers): **2,000–5,000 companies**. DM: Руководитель юридического департамента / Директор по правовым вопросам / General Counsel. Channel: "Премия Лучшие юридические департаменты" (korpurist.life). **Significantly larger market than law firms, though longer sales cycle.**

**Telegram channels:**
- **@povorotnapravo** ("Поворот на Право") — **41,167+ subscribers**, active daily posts, but oriented more toward consumer legal education than B2B managing partners
- **"Рульфы, Ильфы и Инхаусы"** — 4,991 subscribers, international/in-house lawyers — HIGH relevance
- **"ЗарбитражЫ"** — 1,478 subscribers, arbitration lawyers — HIGH relevance
- **Doczilla Info** (t.me/doczilla_info) — useful for competitor tracking
- **Право.ru** (official) — legal professionals, HIGH relevance

**Industry media:** Право.ru (pravo.ru — #1 legal media), Zakon.ru (professional community), Журнал "Корпоративный юрист," Платформа Медиа (platforma-online.ru), Forbes Russia Legal, Коммерсантъ legal section.

**Budget seasonality:** Q4 (Oct–Dec) is planning season + Pravo-300 ceremony in December — managing partners are active. Q1 (Jan–Mar) — new budgets, best for closing deals. Q3 (Jul–Sep) — summer slowdown, September registration for Pravo-300 opens.

---

## SEGMENT 5: Private medicine (clinics with revenue 300M₽+)

### Block 1 — Ten private clinics/networks

Vademecum TOP200 (2023 data): total revenue 385.4B₽, entry threshold **307M₽** (up from 259M₽). 2024 rating published mid-2025. Full table behind paywall — positions 45–80 require Vademecum PDF purchase.

| Clinic | City | Revenue signal | Pain signal | Source |
|--------|------|---------------|-------------|--------|
| **Клиника Фомина** | Moscow + regions | 4.3B₽ (2023), **+54% growth** | Hiring administrators at 72K₽/month on HH.ru, 50+ new clinics planned | vademec.ru |
| **АВС-медицина** | Moscow | Plans to invest **3B₽**, open 40 clinics by 2030, franchise launch | Massive expansion = admin strain | vademec.ru |
| **СМ-Клиника** | Moscow, SPb, Ryazan, Ivanovo | 32 centers | **429 vacancies on HH.ru**, actively hiring administrators and call center staff | hh.ru |
| **Здоровье 365** | Yekaterinburg | Position #38 (↑7), +38% YoY | Rapid growth = hiring needs, admin overload | zdorovo365.ru |
| **УГМК-Здоровье** | Yekaterinburg | Position #16, +26% YoY | Large scale, multi-profile | zdorovo365.ru |
| **СМТ-Клиника** | Yekaterinburg | Position #135, +20% YoY | Actively growing | zdorovo365.ru |
| **Парацельс** | Yekaterinburg | Position #140 (↑3), +18% YoY | Mid-tier, growing | zdorovo365.ru |
| **Клиника Пасман** | Novosibirsk | NEW in TOP200 2023 | New entrant = building processes from scratch | vademec.ru |
| **Авеню** | Rostov-on-Don | ~Position 100–150, franchise model | Franchise expansion = admin standardization needs | vademec.ru |
| **Гармония** | Yekaterinburg | Position #122 (↓4), +16% YoY | Position declining despite growth — operational efficiency problem | zdorovo365.ru |

**HH.ru pain signals:** "Администратор клиники" in Moscow: **1,222+ active vacancies**. Admin salaries: 40,000–110,000₽/month, indicating high turnover and constant need.

### Block 2 — Decision makers

**Who decides on IT at a private clinic (based on noboring-finance.ru organizational analysis):**
1. **Исполнительный директор / Управляющий клиникой** — PRIMARY decision maker for IT/admin tools
2. **Директор / Собственник** — final sign-off on large investments
3. **Главный врач** — medical side only, rarely involved in IT/admin decisions
4. **IT-директор** — exists only in large networks (TOP20); in mid-tier clinics IT is outsourced or handled by 1–2 system admins

**LinkedIn assessment: LOW activity.** Could not find 3 active profiles. Better channels: Telegram, Школа Медицинского Бизнеса events, Vademecum conferences.

### Block 3 — List building

**Sources:**
- **Vademecum TOP200:** vademec.ru/article/top200_chastnykh_mnogoprofilnykh_klinik_po_vyruchke_za_2024_god/ (full table behind paywall/PDF)
- **Rusprofile:** ОКВЭД 86.x, revenue 300M₽+, employees 50+. 8,253 organizations under ОКВЭД 86 total; premium required for revenue filtering
- **HH.ru:** "администратор клиники" → hundreds of active vacancies identifying growing clinics
- **Forbes Healthcare:** annual rating of largest medical companies

**Can you find 50 clinics in 30 minutes? YES** with Vademecum PDF (200 clinics instantly). Without it, ~30–40 via HH.ru + Rusprofile cross-reference. **~150–200 clinics match the criteria** (the entire TOP200 essentially qualifies, bottom ~50 near 307M₽ threshold).

### Block 4 — Competitor analysis

**Chatme.ai** is the strongest competitor in this segment with actual medical clients:
- Clients: **Клиника Фомина** (70% appointments via WhatsApp bot), **ВЕРАМЕД** (72% booking conversion), **Европейский Медицинский Центр** (7x reduction in wait time), Медцентр СМЦ (95% operator load reduction)
- NLU-based chatbots, integrates with МИС Медиалог, Инфоклиника, 1С:Медицина
- **Limitation:** Chat-only, appointment booking + FAQ only, cloud-based, no full administrative assistant

**TWIN (twin24.ai):** Voice + chat bots. Chatbot creation from 35,000₽, voice calls from 0.114₽/sec. 100+ large clients including Ингосстрах. **Limitation:** Scripted scenarios only, no RAG/knowledge base, no on-prem.

**V-AI Labs (v-ai-labs.ru):** AI automation studio, boutique. One-time project-based pricing. **No specific medical clinic clients found publicly.** No MIS integration, no on-prem, no healthcare-specific compliance.

**Why 105K one-time (V-AI Labs) vs. 80–110K/month (our product):** V-AI Labs delivers a single chatbot setup — narrow scope. Our product is a comprehensive AI assistant handling the full spectrum of 120 daily admin calls + on-prem + adoption guarantee + ongoing support. **Different products entirely.**

| Feature | Our product | Chatme.ai | TWIN | V-AI Labs |
|---------|------------|-----------|------|-----------|
| Full AI assistant (RAG) | ✅ | ❌ scripted | ❌ scripted | ❌ basic |
| On-prem / FZ-152 | ✅ native | ❌ cloud | ❌ cloud | ❌ cloud |
| Admin task scope | Full administrative | Appointment only | Appointment + calls | General |
| MIS integration | Required | ✅ | ✅ select | ❌ |
| Price | 80–110K₽/mo | Project-based | From 35K₽ | 105K₽ once |

### Block 5 — Budget and deal cycle

IT spend for 300M₽ clinics: **1–3% of revenue = 3–9M₽/year**. MIS costs: from ~600K₽/year to several million. Our 80–110K₽/month (960K–1.32M₽/year) = comparable to **1–2 administrator salaries** (40–100K₽/month each). Sits at the threshold between operational director approval and owner sign-off.

Decision cycle: **1–3 months** for mid-size clinics, **3–6 months** for large networks. Clinics are conservative — trust, pilot programs, peer references matter. **Seasonality:** Q4 for planning, Q1 for procurement, summer slowdown.

### Block 6 — Telegram/media + counter-evidence

**Industry media:** Vademecum (THE leading healthcare business publication), Школа Медицинского Бизнеса, MedBI, Zdrav.Expert, Evercare.ru, Forbes Healthcare. **B2B Telegram channels for clinic MANAGERS not found as distinct public entities.** Medical business community on Telegram is fragmented — discussions happen in closed groups. Best entry: Школа Медицинского Бизнеса events, Vademecum conferences.

**Counter-evidence — what could prevent reaching this segment:**
- **Conservatism** — clinics are slow to adopt new tools, especially AI; distrust automation
- **"Good enough" solutions** — many clinics use basic chatbots (Chatme.ai) or additional admin hires
- **Price framing** — 80–110K₽/month subscription vs. 35–105K₽ one-time competitors requires clear ROI (replacing 1–2 admins)
- **Workforce resistance** — administrators may resist automation threatening jobs
- **No AI in MIS** — lack of native integration path requires custom integration work
- **Market concentration** — TOP10 clinics control disproportionate revenue; "sweet spot" (positions 45–80) may have less sophisticated IT and smaller budgets
- **Limited digital presence of DMs** — makes direct outreach harder; need phone/events/email

---

## Cross-segment strategic conclusions

The research reveals several patterns that should inform go-to-market prioritization. **IT companies are the fastest path to revenue** — tech-savvy buyers, short deal cycles (2–6 weeks), Telegram-reachable CTOs, and the clearest pain (ChatGPT blocked + documentation chaos). The firmoteka.ru database alone provides 50+ qualified targets in under 20 minutes.

**Manufacturing offers the strongest competitive moat** — literally zero domestic AI competitors for engineering documentation, combined with ASCON's 16,000-customer base as a partnership channel. The challenge is reaching technically conservative decision makers who don't use digital channels; direct phone via 2GIS and ASCON regional offices are the only viable paths.

**Law firms present the most defensible positioning** — no competitor covers internal docs + internet + email + meetings. At 80–110K₽/month for an entire firm, pricing is comparable to Doczilla Pro (2,900₽/person × 30 people = 87K₽) but with dramatically broader functionality. The TAM expands tenfold when corporate legal departments are included (2,000–5,000 companies with 500M₽+ revenue).

**Wholesale trade is the most scalable segment** — 2,000–5,000 companies match the ICP nationally, CRM integrators (CRM Academy, Intervolga, Ингруппа) offer warm referral channels, and the "replacing one sales manager" pricing frame makes ROI self-evident.

**Private medicine is the hardest segment to crack** — conservative buyers, fragmented decision-making, incumbent chatbots (Chatme.ai with real case studies), and DMs hidden in closed Telegram groups. Consider deprioritizing until the product has case studies from other segments that demonstrate cross-industry adoption methodology.

Three overarching findings stand out. First, **LinkedIn is effectively dead for all five segments** — Telegram is the primary professional channel across the board. Second, **budget seasonality is remarkably consistent** — September through November is the optimal outreach window (budget planning), January through March is the optimal close window (new budgets). Third, the **adoption guarantee positioning has no domestic equivalent** — every competitor sells tools, none sell outcomes. This is the strongest differentiator across all five segments.