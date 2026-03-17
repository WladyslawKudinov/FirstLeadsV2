# The complete Russian B2B cold outreach toolkit for 2024–2026

**Russia has built a self-sufficient B2B outreach ecosystem that diverges fundamentally from the Western playbook.** With LinkedIn blocked, Western SaaS tools sanctioned, and corporate email migrating to domestic providers, Russian SDR teams operate with a distinct stack: Контур.Компас for lead lists, Скорозвон for auto-dialing, Coldy.ai for cold email, and Telegram as the de facto professional networking channel. The regulatory environment tightened dramatically in 2025, with fines reaching up to 500 million ₽ for data violations and new anti-spam laws taking effect in September 2025. Despite this, cold B2B outreach remains widespread — the key is structuring it correctly.

This report maps every layer of the Russian outreach infrastructure: databases, email tools, telephony, messaging, legal framework, and performance benchmarks — everything needed to build an outreach campaign agent for the Russian market.

---

## Lead databases: a fragmented ecosystem with no single ZoomInfo equivalent

The Russian B2B data landscape rests on a unique foundation: **ЕГРЮЛ/ЕГРИП**, the state business registries maintained by the Federal Tax Service. Nearly every Russian business database enriches this government data with phone numbers, financials, and contact information. There is no single tool that combines company data, personal decision-maker contacts, and intent signals the way ZoomInfo does. Russian teams typically combine 2–3 tools.

**Контур.Компас** is the most popular lead list builder. It searches across 22+ official sources with 70+ filters (ОКВЭД industry codes, revenue, region, headcount, tax regime) and covers phone numbers for roughly **2 million active organizations**. Pricing starts at **14,900 ₽/year** with a free tier of 50 companies. Its limitation is that only ~10% of companies have named decision-maker contacts — most data is company-level (reception phones, CEO names from ЕГРЮЛ).

**DealRocket** fills this gap as the closest Russian equivalent to Apollo.io or Hunter.io. It specifically provides personal contacts of decision-makers — direct emails, phone numbers, and social media profiles — sourced from VKontakte profiles, corporate websites, and open sources. It offers a browser extension and AI-powered enrichment. DealRocket explicitly positions itself against ЕГРЮЛ-based tools by arguing that company reception numbers are "spammed to death" and useless.

**СПАРК-Интерфакс** is the premium tier at ~**25,000 ₽/month**, used by 150 of the Top-200 Forbes Russia companies, major banks, and government agencies. It provides proprietary risk scoring, ownership structure visualization, and coverage across Russia, Belarus, Kazakhstan, and other CIS countries. Overkill for most SDR teams, but essential for enterprise deals requiring deep counterparty intelligence.

**2GIS** serves as Russia's map-based business directory (Google Maps meets Yellow Pages) with **95% claimed data accuracy**. A massive ecosystem of unofficial parsers extracts company names, phones, emails, and categories by geography and industry. This remains one of the most common lead sourcing methods for SMB-focused SDR teams — parsers cost anywhere from free to ~$100.

Other notable tools include **Seldon.Basis** (mid-market alternative to СПАРК at roughly one-third the price), **Export-base.ru** (pay-per-field lead exports), **Rusprofile.ru** (free company information portal with millions of monthly visitors), **DaData** (data cleansing and enrichment API integrated into many CRMs), **СБИС/Saby** (business network with ~9.7M monthly visits), and **Trigga** (combining lead database of 3.5M contacts with built-in email outreach from **1,990 ₽/month**).

### How Russian SDRs actually find decision-maker contacts

The typical workflow follows three steps. First, identify the decision-maker's name through ЕГРЮЛ data (gives CEO/founder), HH.ru job postings (reveals organizational structure and hiring manager names), conference speaker lists, or VKontakte company group members filtered by workplace. Second, find their email through corporate website team pages, email pattern guessing (constructing name.surname@company.ru), DealRocket searches, or the old-fashioned method of calling reception and asking. Third, validate via SMTP verification (built into Trigga and Coldy.ai). Finding **direct mobile numbers** remains the hardest challenge — DealRocket is the primary tool, supplemented by social media profile scraping, conference materials, and gray-market database purchases.

A critical gap exists: **there are no Russian intent data or technographic data providers** comparable to Bombora, 6sense, or Datanyze. Russian teams substitute with surrogate signals — monitoring HH.ru vacancies (a company hiring a "CRM administrator" might be in-market for CRM software), tracking government procurement announcements on Госзакупки, and watching for company events in СПАРК alerts.

---

## Email outreach runs on homegrown platforms optimized for Russian providers

The sanctions-driven migration from Microsoft 365 and Google Workspace to domestic email providers is the defining feature of 2024–2026. **Yandex 360** and **VK WorkSpace** (formerly Mail.ru for Business) now dominate Russian corporate email. Microsoft suspended M365 for Russian corporate clients in September 2024 — Forbes Russia estimated ~90% of companies previously used Microsoft products. This means cold emails targeting Russian businesses increasingly land in Yandex and Mail.ru inboxes, not Exchange or Gmail.

**Coldy.ai** has emerged as the leading Russian cold email platform, describing itself as the "#1 cold email outreach service in Russia." It features automatic warmup specifically optimized for Yandex and Mail.ru, a built-in database of **7M+ Russian businesses**, AI personalization, and CRM integrations with AmoCRM and Bitrix24. Pricing starts at **2,900 ₽/month** (~$30). Major clients include Контур, Сбер, and Skyeng. Paradoxically, Coldy recommends Google Workspace mailboxes for sending — apparently still accessible for non-sanctioned entities and described as "most stable, rarely blocked."

**Respondo** offers chain-of-letters automation with built-in SPF/DKIM/DMARC checking, warmup scenarios, and email validation. It reports average **12–13.6% reply rates** on well-executed campaigns. Pricing starts at **1,920 ₽/month**. **Trigga** combines a 3.5M-contact database with a visual chain builder, domain warmup, and click monitoring — functioning as the closest Russian analog to Apollo.io's all-in-one approach.

Western tools like Instantly, Lemlist, and Woodpecker are known but face severe practical barriers: Russian bank cards don't work for international payments, these tools don't warm up against Russian email providers (resulting in lower deliverability to Yandex/Mail.ru inboxes), and they lack Russian-language support. They remain used primarily by teams targeting international markets.

### The critical distinction: ESPs vs. cold email tools

Russian email service providers — UniSender, DashaMail, Mailganer, Sendsay, NotiSend, RuSender — **explicitly prohibit cold email**. These are for marketing to opted-in subscribers. Cold email requires dedicated tools (Coldy, Respondo, Trigga) that emulate manual sending at ~**50 emails per inbox per day**. The standard infrastructure setup uses 3+ separate domains (not the main company domain), 2 mailboxes per domain, each sending ~50 emails daily. Six mailboxes yield ~300 emails/day or ~9,000/month. Domains cost as little as **120 ₽** for a .ru address.

Email warmup is deeply embedded in practice. All major Russian outreach platforms provide built-in warmup, and the standard protocol ramps from 20–50 emails/day over 2–3 weeks. **Holymailer** offers a specialized service providing pre-configured mailboxes with SPF/DKIM/DMARC, blacklist monitoring, and IP rotation — compatible with both Russian and Western outreach platforms. Russian SMTP relay services include Sendsay Transport, RuSender, NotiSend, and UniSender Go (positioned as a MailGun/SendGrid replacement), all with servers on Russian territory for 152-FZ compliance.

Mail.ru enforces specific spam complaint thresholds: **max 1.1%** for senders under 10K emails/month, dropping to **0.3%** for volumes above 50M. If invalid addresses exceed 5%, mailings are blocked entirely.

---

## Cold calling remains king, powered by Скорозвон and Mango Office

Russian B2B sales is fundamentally phone-centric. **51% of B2B leads are still generated through cold calls**, and direct mobile numbers of decision-makers are the most valued data point in the ecosystem. The tech stack has three layers: virtual PBX providers, dedicated auto-dialers, and speech analytics.

**Mango Office** ranks #1 in the Market.CNews 2024 comprehensive VATS rating with **60,000+ clients** and 24 data centers across 120 Russian cities. It offers 200+ PBX features including speech analytics, omnichannel contact center, call tracking, and FMC SIM cards. Basic tier starts at **685 ₽/month**. **Sipuni** holds the strongest CRM integration story, with deep native integration into AmoCRM plus 11 other systems. **Телфин** provides an omnichannel solution combining PBX, virtual mobile numbers, WhatsApp/Telegram integration within CRM, and speech analytics. **MTS Exolve** (formerly MTT) offers a CPaaS platform combining SMS, voice, and messengers. **Zadarma** provides the cheapest entry point with a free basic PBX at ~1.5 ₽/min.

**Скорозвон (Skorozvon)** is the undisputed #1 dedicated cold calling tool. Its predictive dialer enables operators to make **100–200 calls/day** versus 40–60 from a CRM+telephony setup. Key features include a "number carousel" achieving up to **98% reach rates** through automatic rotation of outgoing numbers, built-in call scripts, and a supervisor "whisper" mode for live coaching. Its AI suite now includes a voice robot processing 25,000 contacts in 6 hours (from **4 kopecks/second**), AI speech analytics, and an AI sales trainer dialog simulator. Pricing runs **2,000–2,300 ₽/month per user**.

Other auto-dialers include **Оки-Токи** (professional cloud contact center with predictive, progressive, and power modes), **Звонобот** (AI voice robot specialist), and **VoIPTime** (three outbound modes claiming 3x efficiency gains).

The AI speech analytics segment is developing rapidly. **SalesAI 2.0** represents the new "Revenue Intelligence" generation — auto-analyzing calls, filling CRM fields (BANT qualification, next steps), and providing coaching recommendations at **2 ₽/minute**. **imot.io** uses GPT-4 for call analysis at 8 ₽/minute. The shift from keyword-based analytics to contextual AI understanding is a defining 2025–2026 trend.

---

## LinkedIn survives via VPN; Telegram has become the real professional network

Despite being blocked since 2016, LinkedIn retains **7.5 million users in Russia** (April 2024 data from LinkedIn's own marketing APIs), with the 25–34 age group comprising ~70% of the base. Individuals face no prosecution for using VPNs to access blocked sites — only VPN providers bear liability. One user on Сетка.ru reported closing a **150-million-₽ deal** attributed to LinkedIn outreach. Cloud-based automation tools like Expandi ($99/month) and Dripify work from Russia through VPN, and **LinkAdd** is a Russia-adapted service that interacts with LinkedIn users without requiring login.

The practical challenges are real: unstable VPN connections, account creation triggering fraud detection, Russian bank cards not working for Premium/Sales Navigator, and the overhead of maintaining automation through VPN. LinkedIn remains essential for international contacts but is unreliable as a primary domestic channel.

**TenChat** has emerged as the most viable domestic alternative with **3+ million users**, of whom **56.9% are entrepreneurs and top managers**. Its "Бизнес.Тиндер" feature matches business contacts by 30+ parameters, and its "Zeus" AI algorithm promotes quality content while penalizing spam. TenChat verifies companies via INN and integrates tender search tools. Its weakness: no company pages, limited web functionality, and far fewer users than LinkedIn globally. **Сетка** (by HeadHunter/HH.ru), launched publicly in June 2024 with an estimated **1.5–2 billion ₽ investment**, uses AI to auto-group users by work experience and industries but remains early-stage. **Профессионалы.ру is effectively dead** — returning 403 errors since 2022.

The honest answer for 2024–2026: Russian B2B professionals use a fragmented ecosystem. LinkedIn via VPN for international contacts, **Telegram for domestic B2B networking** (professional communities, expert channels, direct messaging), TenChat for personal branding among SMB entrepreneurs, and offline events for high-value relationships.

---

## Telegram is the B2B outreach channel that doesn't exist in the West

With **91 million monthly active users** and **72% population reach**, Telegram has become Russia's second most important B2B outreach channel after email. In 2024, it overtook Instagram and VK as the **#1 platform for business promotion** — 66.9% of advertisers use it. Average daily usage runs **47 minutes per day**.

Telegram's B2B applications take four forms. **Professional communities and chats** are the primary way Russian professionals find each other — industry-specific groups exist for virtually every B2B niche, discoverable through **TGStat** and **Telemetr** analytics platforms. **Expert channels** function as the Russian equivalent of LinkedIn content marketing — one practitioner reported growing to 600 subscribers in 2 months with daily posts, generating inbound leads. **Direct messaging** works for personalized outreach when preceded by engagement in shared groups, but mass unsolicited DMs trigger aggressive bans. **Bots** handle lead qualification, auto-funnels, and appointment scheduling — tools like Chatforma, BotHelp, SaleBot, and SendPulse serve this market.

**WhatsApp** reaches **96 million monthly users** in Russia with **~90% message open rates**, but it is unsuitable for cold B2B outreach. WhatsApp Business API requires pre-approved message templates, and cold messaging results in account bans. It works for customer service and warm lead nurturing after initial contact through other channels. Authorized Russian API providers include **edna** (only official WhatsApp partner in Russia), **1msg.ru**, and **Chat2Desk**.

CRM-to-messenger integration is handled by **Wazzup** (most popular, from **1,200 ₽/month** — connects WhatsApp, Telegram, and Viber to AmoCRM/Bitrix24), **Radist.Online** (write-first capability in WhatsApp/Telegram from CRM), and **TextBack** (subscriber funnels with macros). **Viber is declining** — Roskomnadzor restricted access in December 2024, and daily usage dropped to just 3 minutes.

---

## No Russian Outreach.io exists — teams build modular stacks around CRM

Russia has **no single platform replicating Outreach.io or Salesloft**. Instead, teams assemble a modular stack using CRM as the orchestration hub with plugins for each channel.

**AmoCRM** comes closest to a sales engagement platform. Its Digital Pipelines (Цифровые воронки) automate workflows by pipeline stage, **Salesbot** auto-sends WhatsApp/Telegram messages when leads change stages, the **Почтовик** widget creates email chains with open/click tracking, and 50+ telephony integrations handle calling. **Bitrix24** offers broader functionality (CRM + tasks + projects + internal messenger + HR) with built-in telephony, AI transcription via BitrixGPT, and a marketplace of messenger integrations, but is more complex to configure for pure outbound SDR workflows.

The typical Russian multichannel SDR workflow in 2025 runs: lead sourcing from Контур.Компас → first touch via Telegram/WhatsApp message from CRM (via Wazzup/Radist) or cold call via Скорозвон → follow-up email via CRM integration or Coldy.ai → continued nurture via messenger auto-funnel → task management and analytics in CRM.

| Layer | Western model | Russian model |
|-------|--------------|---------------|
| Primary first-touch | Cold email + LinkedIn | Cold call + Telegram/WhatsApp |
| Orchestration | Outreach.io/Salesloft (all-in-one) | AmoCRM/Bitrix24 + plugins (modular) |
| Email sequences | Built into sales engagement platform | Widget/add-on (Почтовик) or Coldy.ai |
| Social selling | LinkedIn InMail | Telegram DMs, TenChat |
| Calling | Integrated dialer | Separate tool (Скорозвон) |
| AI coaching | Gong/Chorus | SalesAI 2.0, Скорозвон AI Trainer |
| Data providers | ZoomInfo, Apollo, Cognism | Контур.Компас, DealRocket, 2GIS |

---

## The legal gray zone is narrowing fast

Russian cold B2B outreach exists in a legally ambiguous space that is **tightening dramatically in 2025**. Two laws govern: **ФЗ-152** (personal data) and **ФЗ-38** (advertising). The analysis splits into two tracks.

Under ФЗ-152, generic corporate emails (info@company.ru) are generally not personal data. But individual business emails containing a person's name (ivanov@company.ru) **are** personal data requiring documented consent for processing. From September 1, 2025, consent must be a **separate standalone document** — it cannot be buried in terms of service. From July 1, 2025, all personal data of Russian citizens must be stored primarily on Russian servers before any cross-border transfer.

Under ФЗ-38, any communication promoting products/services to an undefined circle of persons is "advertising" requiring **prior consent** of the recipient — and the burden of proof falls on the sender. The law does not distinguish between B2B and B2C. However, "reference-informational and analytical materials that do not have as their primary purpose the promotion of goods on the market" are not advertising. This creates the **strategic framework**: highly personalized, problem-solving emails addressing a specific prospect's situation have a stronger case for not being classified as advertising, removing the consent requirement.

Penalties have escalated from symbolic to potentially business-threatening:

- Advertising via electronic communications without consent: **300,000–1,000,000 ₽** per violation (from April 2024)
- Data breach (100K+ records): up to **15 million ₽** (from May 2025)
- Repeated data violations: **1–3% of annual revenue** (from May 2025)
- Maximum for massive breach: up to **500 million ₽**
- Criminal liability for intentional illegal data use: up to **10 years imprisonment** (from November 2024)

The most significant upcoming change: **Law No. 41-FZ** (effective September 1, 2025) requires consent for **any mass communications** — not just advertising — via the Communications Law, broadening the scope beyond the Advertising Law. This directly impacts cold calling and mass email.

In practice, enforcement has been complaint-driven — one Russian outreach platform reports only 1 complaint per 150 million emails sent over 2 years, with FAS fines historically at ~5,000 ₽. But automated Roskomnadzor AI website audits and dramatically higher fines are changing the risk calculus. The safe approach: use corporate (not personal) contact data from public sources, craft personalized informational emails rather than promotional ones, always include opt-out mechanisms, store data on Russian servers, and register as a personal data operator.

---

## Benchmarks: what to expect from Russian B2B outreach campaigns

**Cold email performance** in Russia tracks global averages but shows higher results from specialized platforms targeting smaller, better-segmented audiences. Normal open rates run **15–30%** (above 30% is excellent; below 10% signals problems). Reply rates average **5–10%** on well-targeted campaigns, with Russian platforms like Respondo reporting **13.6%** in IT segments — significantly above the global average of 4–5%. Click-through rates hover at 3–6% for B2B. Best sending time: **8–11 AM Moscow time** on weekdays, with Wednesday showing the strongest results. Optimal format: under 200 words, 6–8 sentences, mobile-optimized, in direct but respectful business Russian.

**Cold calling metrics** reflect Russia's phone-centric culture. Dial-to-connect rates on well-prepared bases average **40–50%**. The average number of attempts to reach a decision-maker has grown from 6 in 2022 to **8.5 in 2025** — 9 out of 10 decision-makers don't answer unknown numbers. Conversion from cold call to meeting averages **2–5%**, with trained internal teams achieving 5–10% and top performers hitting 18–22% on first-call-to-meeting rates. Three call attempts yield 93% of all successful contacts; after 5 attempts, switch targets. Best calling time: **8–11 AM** in the recipient's local timezone, with Wednesday performing strongest.

Context matters: the average Russian business decision-maker receives ~**150 emails/day**, 15–20 incoming calls, and 50–70 messenger messages, with over 60% being spam. Quality and personalization are not optional — they are the only path to cutting through.

---

## Conclusion: building an outreach agent for the Russian market

The Russian B2B outreach ecosystem rewards those who understand its structural differences from Western markets. Five design principles should guide any outreach campaign agent:

**Phone-first, not email-first.** Cold calling generates 51% of Russian B2B leads. Your agent should prioritize Скорозвон integration for auto-dialing with number rotation, treating email as a supporting channel rather than the primary one.

**Telegram is your LinkedIn.** With 91M users and 72% population reach, Telegram professional communities are where decision-makers actually engage. Build community monitoring and personalized DM capabilities into your agent's workflow.

**Use Russian-native tools exclusively.** Coldy.ai for email, Контур.Компас for leads, Скорозвон for calling, AmoCRM for orchestration. Western tools face payment barriers, deliverability gaps with Yandex/Mail.ru, and compliance risks under data localization requirements.

**Personalize or perish — legally and practically.** The legal framework requires personalized, informational outreach rather than mass promotional campaigns. This aligns with performance data: hyper-targeted campaigns outperform mass approaches by 3x or more.

**Prepare for September 2025.** The new anti-spam communications law requires consent for any mass communications. Design your agent with consent management, opt-out tracking, and Russian-server data storage from the start.