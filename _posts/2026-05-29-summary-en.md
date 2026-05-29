---
layout: default
title: "Horizon Summary: 2026-05-29 (EN)"
date: 2026-05-29
lang: en
---

> From 35 items, 8 important content pieces were selected

---

1. [US DOJ Demands Reddit and X Provide Data on ICE Critics](#item-1) ⭐️ 9.0/10
2. [GitHub bans security researcher over zero-day Windows exploits](#item-2) ⭐️ 8.0/10
3. [Postgres Sufficient for Durable Workflows, Says DBOS Blog](#item-3) ⭐️ 8.0/10
4. [Curated List of LLM-Generated Text 'Smells' Surfaces Online](#item-4) ⭐️ 8.0/10
5. [Anthropic Raises $65B Series H at $965B Valuation](#item-5) ⭐️ 8.0/10
6. [Qualcomm and ByteDance Partner for Custom AI ASICs](#item-6) ⭐️ 8.0/10
7. [NVIDIA CEO: Taiwan is AI Revolution Center, $150B Annual Plan](#item-7) ⭐️ 8.0/10
8. [BYD mass-produces 4nm 'Xuanji A3' smart driving chip](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [US DOJ Demands Reddit and X Provide Data on ICE Critics](https://www.bloomberg.com/news/articles/2026-05-28/trump-s-doj-ramps-up-probes-of-anonymous-ice-critics-with-x-reddit-subpoenas) ⭐️ 9.0/10

The US Department of Justice has issued grand jury subpoenas to Reddit and X, demanding the real-world identities of at least two anonymous accounts that criticized ICE enforcement actions. The affected users have retained lawyers and are legally challenging the subpoenas. This escalation from administrative to grand jury subpoenas signals a more aggressive government approach to investigating online critics, potentially chilling protected speech under the First Amendment. It raises serious concerns about user privacy, free expression, and the reach of government surveillance on digital platforms. The subpoenas are based on an ongoing criminal investigation, but users have not been told what specific crime they are suspected of. A judge is currently reviewing a motion to quash the subpoenas.

telegram · zaihuapd · May 28, 14:22

**Background**: The US Department of Justice has authority to investigate federal crimes and can compel platforms to disclose user data via subpoenas. Grand jury subpoenas are more coercive than administrative subpoenas and typically indicate a criminal probe. While tech companies frequently receive government data requests, targeting anonymous accounts of political critics with such escalated measures is relatively rare and legally contentious.

**Tags**: `#free speech`, `#government surveillance`, `#privacy`, `#digital rights`, `#US law`

---

<a id="item-2"></a>
## [GitHub bans security researcher over zero-day Windows exploits](https://www.tomshardware.com/tech-industry/cyber-security/microsofts-github-bans-security-researcher-who-posted-zero-day-windows-exploits-because-company-ruined-their-life-expert-claims-action-is-vindictive-and-promises-further-retaliation) ⭐️ 8.0/10

GitHub banned a security researcher for posting zero-day Windows exploits, and the researcher claims Microsoft ruined their life and vows further retaliation. This incident highlights tensions between bug bounty programs, platform policies, and researcher ethics, potentially affecting how zero-day disclosures are handled and the trust between researchers and major tech companies. The researcher was also banned from GitLab, and the community speculates that rules about hosting exploits may have been broken, though Microsoft has not publicly commented.

hackernews · possibilistic · May 28, 21:45 · [Discussion](https://news.ycombinator.com/item?id=48315968)

**Background**: A zero-day vulnerability is a security flaw unknown to the software vendor, which can be exploited before a patch exists. Bug bounty programs encourage ethical hackers to report such flaws privately in exchange for rewards, but posting exploits publicly can lead to bans and legal issues.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zero-day_vulnerability">Zero-day vulnerability - Wikipedia</a></li>
<li><a href="https://bugbustersunited.com/bug-bounty-ethics-101-legal-and-ethical/">Bug Bounty Ethics 101: Legal and Ethical Best Practices | BugBustersUnited</a></li>

</ul>
</details>

**Discussion**: Commenters express concern that Microsoft's actions may be vindictive and counterproductive, pushing researchers to sell exploits elsewhere. Some question why both GitHub and GitLab banned the user, suggesting rules were likely violated. Others note that bug bounty programs typically incentivize payouts, making this an unusual case.

**Tags**: `#security`, `#zero-day`, `#GitHub`, `#Microsoft`, `#bug bounty`

---

<a id="item-3"></a>
## [Postgres Sufficient for Durable Workflows, Says DBOS Blog](https://www.dbos.dev/blog/postgres-is-all-you-need-for-durable-execution) ⭐️ 8.0/10

A blog post from DBOS argues that PostgreSQL alone is sufficient for building durable workflow execution systems, challenging the need for external workflow engines like Temporal or Restate. This discussion matters because it highlights a growing trend of leveraging the database itself for reliability, reducing infrastructure complexity and operational overhead for developers building distributed systems. The blog specifically references DBOS, a Postgres-native durable execution framework, and compares it to alternatives. Key Postgres features like advisory locks and LISTEN/NOTIFY enable workflow coordination without external dependencies.

hackernews · KraftyOne · May 28, 18:41 · [Discussion](https://news.ycombinator.com/item?id=48313530)

**Background**: Durable workflows ensure that a sequence of steps (e.g., order processing) completes reliably even if failures occur, by persisting state and retrying. Traditionally, this requires dedicated engines like Temporal. Postgres offers built-in primitives such as advisory locks for concurrency control and LISTEN/NOTIFY for real-time notifications, which can be combined to build workflow orchestration directly in the database.

<details><summary>References</summary>
<ul>
<li><a href="https://www.dbos.dev/blog/postgres-is-all-you-need-for-durable-execution">Postgres-backed Durable Workflow Execution | DBOS</a></li>
<li><a href="https://appmaster.io/blog/postgresql-advisory-locks-double-processing">PostgreSQL advisory locks for concurrency-safe workflows</a></li>
<li><a href="https://medium.com/@kaushalsinh73/10-reactive-postgres-tricks-with-listen-notify-00543968b566">10 Reactive Postgres Tricks With LISTEN / NOTIFY | Medium</a></li>

</ul>
</details>

**Discussion**: Commenters shared practical experiences: some use DBOS for workflows requiring atomic messaging tied to Postgres transactions, while others prefer Restate for performance or Cloudflare Workflows for cheap non-critical tasks. Users also compared DBOS to Temporal, noting payload size limits with the latter and praising Postgres-based approaches for simplicity.

**Tags**: `#postgres`, `#durable-workflows`, `#distributed-systems`, `#workflow-engines`

---

<a id="item-4"></a>
## [Curated List of LLM-Generated Text 'Smells' Surfaces Online](https://shvbsle.in/various-llm-smells/) ⭐️ 8.0/10

A blog post titled 'Various LLM Smells' compiles a curated list of linguistic and stylistic patterns that strongly indicate AI-generated text, sparking a community discussion on detection and usage. As LLMs become ubiquitous, being able to detect AI-generated writing is crucial for maintaining authenticity in content, education, and journalism, and this list provides practical, actionable markers for readers and writers. The list includes specific phrases like 'the honest caveat:' and 'load bearing' used metaphorically, as well as structural patterns like contrastive negation ('It's not X, it's Y'), which are common in LLM output but not typical in human writing.

hackernews · speckx · May 28, 19:02 · [Discussion](https://news.ycombinator.com/item?id=48313810)

**Background**: Large language models (LLMs) like GPT-4 generate text by predicting the next word based on vast training data. Their output often exhibits subtle stylistic habits, or 'smells,' that can be identified by attentive readers. This phenomenon is analogous to Wikipedia's 'Signs of AI writing' page, which documents similar patterns.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Large_language_model">Large language model - Wikipedia</a></li>
<li><a href="https://blog.frohrer.com/how-to-detect-llm-writing-in-text/">Detecting LLM writing in Text | Fred Rohrer's Blog</a></li>

</ul>
</details>

**Discussion**: Comments highlight that LLM writing may appear 'significantly better' to those without domain expertise, and caution against directly incorporating AI-generated phrases. Some users point out that certain structural patterns, like contrastive negation, are strong tells. Others suggest using LLMs for editing rather than generation to preserve personal style.

**Tags**: `#LLM`, `#AI detection`, `#writing`, `#analysis`, `#Hacker News`

---

<a id="item-5"></a>
## [Anthropic Raises $65B Series H at $965B Valuation](https://www.anthropic.com/news/series-h) ⭐️ 8.0/10

Anthropic announced a $65 billion Series H funding round, bringing its post-money valuation to $965 billion. The company also reported that its annualized run-rate revenue exceeded $47 billion earlier this month. This massive funding round underscores the enormous capital requirements and market expectations for leading AI companies. The high valuation relative to reported revenue raises questions about sustainability and future IPO prospects. The $47 billion run-rate revenue figure is self-reported and represents annualized revenue based on recent monthly performance, not GAAP revenue. The funding comes just months after the Series G round in February 2026.

hackernews · meetpateltech · May 28, 18:09 · [Discussion](https://news.ycombinator.com/item?id=48313048)

**Background**: Run-rate revenue estimates annual revenue by extrapolating a recent period's revenue (e.g., one month) to a full year; it is commonly used by fast-growing startups but can be misleading if growth is not linear. Venture capital funding rounds are classified alphabetically (Series A, B, C, etc.), and later-stage rounds like Series H indicate a company that has raised many rounds before considering an IPO.

**Discussion**: Community comments expressed skepticism about the valuation, with some questioning how many more funding rounds are needed before investors see returns. Others debated the meaning and reliability of run-rate revenue versus actual revenue, and noted that without an IPO, companies face less scrutiny on their financial claims.

**Tags**: `#Anthropic`, `#funding`, `#AI`, `#valuation`, `#venture capital`

---

<a id="item-6"></a>
## [Qualcomm and ByteDance Partner for Custom AI ASICs](https://t.me/zaihuapd/41616) ⭐️ 8.0/10

Qualcomm has reportedly reached a deal with ByteDance to produce custom AI ASICs, with ByteDance ordering millions of chips for its AI workloads. This partnership could significantly impact the AI hardware landscape, combining Qualcomm's chip design expertise with ByteDance's massive AI service demands. It reflects a growing trend of hyperscalers pursuing custom silicon to optimize performance and cost. The deal is unconfirmed by both companies, with Qualcomm's representative declining to comment and ByteDance's spokesperson not responding. Qualcomm had previously announced in late April that it would deliver its first ASIC to a hyperscale cloud provider this year, which aligns with this report.

telegram · zaihuapd · May 28, 07:09

**Background**: An ASIC (Application-Specific Integrated Circuit) is a chip customized for a specific task, offering superior performance and power efficiency compared to general-purpose CPUs or GPUs. In AI, ASICs can accelerate model inference and training more efficiently. Major tech companies increasingly design custom ASICs to reduce costs and improve performance for their specific workloads.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Application-specific_integrated_circuit">Application-specific integrated circuit - Wikipedia</a></li>
<li><a href="https://www.arm.com/glossary/asic">What is ASIC? - ASIC Cost</a></li>

</ul>
</details>

**Tags**: `#Qualcomm`, `#ByteDance`, `#AI`, `#ASIC`, `#hardware`

---

<a id="item-7"></a>
## [NVIDIA CEO: Taiwan is AI Revolution Center, $150B Annual Plan](https://arstechnica.com/tech-policy/2026/05/nvidia-ceo-wants-taiwan-to-be-center-of-ai-revolution-not-us/) ⭐️ 8.0/10

NVIDIA CEO Jensen Huang declared Taiwan as the center of the AI revolution and announced plans to invest approximately $150 billion annually in Taiwan, covering AI chip production, system manufacturing, and supply chain collaboration. A new Taipei headquarters is set to break ground this year and open by 2030, accommodating 4,000 employees. This massive investment significantly deepens NVIDIA's supply chain reliance on Taiwan, reinforcing the island's strategic role in AI hardware production. It also has geopolitical implications, as it underscores Taiwan's centrality to the global AI industry amid ongoing US-China tensions. The annual investment of $150 billion is a substantial increase from the previous $10–15 billion per year a few years ago. The new Taipei HQ will house 4,000 employees and is expected to be operational by 2030.

telegram · zaihuapd · May 28, 07:33

**Background**: Taiwan is home to TSMC, the world's leading semiconductor foundry, and a dense ecosystem of electronics manufacturers like Hon Hai (Foxconn), Wistron, and Quanta. NVIDIA relies on TSMC for its most advanced AI chips and on Taiwanese ODMs for system assembly. Huang's statement reinforces Taiwan's position as a critical node in the global AI supply chain.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Wistron_Corporation">Wistron Corporation</a></li>
<li><a href="https://en.wikipedia.org/wiki/Quanta_Computer">Quanta Computer</a></li>
<li><a href="https://en.wikipedia.org/wiki/Semiconductor_industry_in_Taiwan">Semiconductor industry in Taiwan - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#NVIDIA`, `#AI`, `#Supply Chain`, `#Taiwan`, `#Investment`

---

<a id="item-8"></a>
## [BYD mass-produces 4nm 'Xuanji A3' smart driving chip](https://finance.sina.com.cn/roll/2026-05-28/doc-inhznenn1371824.shtml) ⭐️ 8.0/10

On May 28, 2026, at the 'Dare to Act' intelligent strategy conference, BYD chairman Wang Chuanfu announced the mass production of the 4nm 'Xuanji A3' smart driving chip. The chip supports L3 and L4 autonomous driving, and three chips together deliver over 2100 TOPS of computing power. This milestone demonstrates BYD's deep vertical integration in autonomous driving hardware, potentially reducing reliance on external suppliers and accelerating the adoption of high-level autonomous driving in mass-market EVs. The 4nm process node is competitive with leading chipmakers, signaling China's growing capabilities in automotive semiconductors. The chip incorporates BYD's self-developed algorithms to achieve a 100% improvement in computing power utilization. BYD also revealed that it has developed over 2,000 chip products and operates five wafer fabrication plants.

telegram · zaihuapd · May 28, 13:01

**Background**: Autonomous driving is classified into levels from 0 to 5, with L3 meaning conditional automation where the driver can take their eyes off the road but must be ready to intervene, and L4 meaning high automation where the vehicle can handle all driving in specific conditions without driver attention. TOPS (trillions of operations per second) is a key metric for AI chip performance; 2100 TOPS enables complex real-time perception and decision-making for autonomous driving.

<details><summary>References</summary>
<ul>
<li><a href="https://torc.ai/understanding-the-levels-of-autonomy-3-4-5/">What Are The Levels of Autonomy? L3-L4 - Torc Robotics</a></li>
<li><a href="https://www.windowscentral.com/hardware/laptops/what-is-tops">What is TOPS and why is it important for AI? | Windows Central</a></li>

</ul>
</details>

**Tags**: `#BYD`, `#autonomous driving`, `#4nm chip`, `#EV`, `#semiconductor`

---