---
layout: default
title: "Horizon Summary: 2026-07-15 (EN)"
date: 2026-07-15
lang: en
---

> From 33 items, 15 important content pieces were selected

---

1. [2026 Fields Medalists Leaked via ICM Website Code](#item-1) ⭐️ 9.0/10
2. [Amap Launches World Model Workshop with 'Portal'](#item-2) ⭐️ 9.0/10
3. [Bonsai 27B: First 27B Model That Runs on a Phone](#item-3) ⭐️ 8.0/10
4. [AI Agents Threaten Software Composability, Essay Warns](#item-4) ⭐️ 8.0/10
5. [Cursor 0day Vulnerability Prompts Full Disclosure](#item-5) ⭐️ 8.0/10
6. [Are we offloading too much thinking to AI?](#item-6) ⭐️ 8.0/10
7. [Lobste.rs Migrates from MariaDB to SQLite, Cuts Costs](#item-7) ⭐️ 8.0/10
8. [Armin Ronacher: AI Agents May Erode Shared Software Understanding](#item-8) ⭐️ 8.0/10
9. [Cloudflare Launches Precursor: Continuous Behavioral Bot Detection](#item-9) ⭐️ 8.0/10
10. [DeepSeek Raises Over $7.4B in First Round with Novel Control Structure](#item-10) ⭐️ 8.0/10
11. [Telegram's t.me Domain Frozen by Registry](#item-11) ⭐️ 8.0/10
12. [DeepMind CEO Urges US-led Global AI Watchdog](#item-12) ⭐️ 8.0/10
13. [DeepSeek seeks $71B valuation in new round, develops AI chips](#item-13) ⭐️ 8.0/10
14. [White House to Convene Power Companies on AI Electricity Costs](#item-14) ⭐️ 8.0/10
15. [US Approves Nvidia H200 Sales to ~10 Chinese Firms](#item-15) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [2026 Fields Medalists Leaked via ICM Website Code](https://www.reddit.com/r/math/comments/1urv4id/fields_medal_26_predictionsdiscussion/) ⭐️ 9.0/10

A hidden schedule in the frontend code of the ICM website may have revealed the 2026 Fields Medalists: Yu Deng, John Pardon, Jacob Tsimerman, and Hong Wang. This leak, if genuine, would preempt one of mathematics' most prestigious announcements, intensifying scrutiny on ICM's security and highlighting the community's intense interest in the selection. The names were found in code marked 'HIDDEN' by a user scraping the ICM site; Polymarket prediction odds for this outcome reached 95%.

telegram · zaihuapd · Jul 14, 05:51

**Background**: The Fields Medal, awarded every four years, recognizes outstanding mathematical achievements for researchers under 40. Hong Wang recently gained prominence for resolving the three-dimensional Kakeya conjecture, a major problem in harmonic analysis. Polymarket is a cryptocurrency-based prediction market where users bet on future events.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kakeya_conjecture">Kakeya conjecture</a></li>
<li><a href="https://arxiv.org/abs/2512.09842">The Kakeya Conjecture: where does it come from and why is it important?</a></li>
<li><a href="https://en.wikipedia.org/wiki/Polymarket">Polymarket</a></li>

</ul>
</details>

**Tags**: `#Fields Medal`, `#mathematics`, `#leak`, `#ICM`, `#academia`

---

<a id="item-2"></a>
## [Amap Launches World Model Workshop with 'Portal'](https://www.ithome.com/0/976/538.htm) ⭐️ 9.0/10

Amap (Alibaba) released ABot-WorldStudio, a world model workshop that generates interactive 3D worlds from text or images, featuring a 'time-space portal' for seamless traversal between worlds. The underlying ABot-World series models are fully open-sourced. This release is significant because it achieves unlimited inference duration without quality degradation, far exceeding the typical ~1 minute limit of competitors. By unifying interactive video generation with 3DGS scene output, it has broad implications for embodied AI simulation, game development, and virtual production. ABot-WorldStudio runs locally on a single RTX 5090 GPU and has been tested for over one hour continuously without crashes or quality loss. It natively outputs 3DGS assets with real geometric structure and photorealistic fidelity.

telegram · zaihuapd · Jul 14, 12:22

**Background**: A world model in AI is a system that learns an internal representation of an environment to simulate dynamics and predict outcomes. 3D Gaussian Splatting (3DGS) is a rasterization technique for real-time rendering of photorealistic 3D scenes from sparse 2D images, revitalized in 2023. Embodied AI integrates AI into physical systems for real-world interaction, such as robotics and autonomous vehicles.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/3D_Gaussian_splatting">3D Gaussian splatting</a></li>
<li><a href="https://en.wikipedia.org/wiki/World_model_(artificial_intelligence)">World model (artificial intelligence)</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/embodied-ai/">Embodied AI: What Is It and How to Build It?</a></li>

</ul>
</details>

**Tags**: `#world model`, `#3DGS`, `#AI generation`, `#open source`, `#embodied AI`

---

<a id="item-3"></a>
## [Bonsai 27B: First 27B Model That Runs on a Phone](https://prismml.com/news/bonsai-27b) ⭐️ 8.0/10

PrismML announced Bonsai 27B, a 27-billion-parameter multimodal model based on Qwen3.6 27B, quantized to 1-bit or ternary weights to fit into 4GB of memory for on-device inference. The 1-bit version runs on phones, marking the first time a 27B-class model is deployable on mobile devices. This breakthrough in extreme quantization demonstrates that large language models can be run locally on consumer hardware, enabling privacy-preserving AI without cloud dependency. It challenges the assumption that sub-4-bit quantization severely degrades performance, as Bonsai 27B retains up to 94.6% of FP16 accuracy. Bonsai 27B uses 1-bit and ternary weights across all language components, with a separate 4-bit vision tower. The ternary variant takes 5.9GB and retains 94.6% of FP16 performance on benchmarks, while the 1-bit version takes 3.9GB and retains 89.5%.

hackernews · xenova · Jul 14, 17:50 · [Discussion](https://news.ycombinator.com/item?id=48910545)

**Background**: Quantization reduces the precision of neural network weights (e.g., from 16-bit floating point to 1-bit binary) to shrink model size and speed up inference, enabling deployment on devices with limited memory like smartphones. Traditional sub-4-bit quantization often causes significant accuracy loss, but new techniques like those used by PrismML aim to minimize degradation while achieving extreme compression. On-device AI eliminates latency and privacy concerns associated with cloud-based models, making powerful AI accessible without an internet connection.

<details><summary>References</summary>
<ul>
<li><a href="https://prismml.com/news/bonsai-27b">PrismML — Announcing Bonsai 27B: The First 27B-Class Model to ...</a></li>
<li><a href="https://www.marktechpost.com/2026/07/14/prismml-releases-bonsai-27b-1-bit-and-ternary-builds-of-qwen3-6-27b-that-run-on-laptops-and-phones/">PrismML Releases Bonsai 27B: 1-bit and Ternary Builds of ...</a></li>
<li><a href="https://docs.prismml.com/models/bonsai-27b">Bonsai 27B - Bonsai - docs.prismml.com</a></li>

</ul>
</details>

**Discussion**: Commenters compared Bonsai 27B to Gemma 4 12B QAT, questioning how much intelligence is lost at extremely low bitwidths. Some users reported difficulty running the models in LM Studio, while others expressed skepticism about the model's real-world performance (e.g., a recipe demo with incorrect macronutrient calculations).

**Tags**: `#AI`, `#quantization`, `#on-device AI`, `#model compression`, `#machine learning`

---

<a id="item-4"></a>
## [AI Agents Threaten Software Composability, Essay Warns](https://lucumr.pocoo.org/2026/7/13/the-tower-keeps-rising/) ⭐️ 8.0/10

Armin Ronacher's essay 'The Tower Keeps Rising' warns that over-reliance on AI coding agents erodes software composability and architectural control, echoing the Lisp Curse. As AI coding tools become widespread, developers may lose the ability to build maintainable, composable systems, threatening long-term software quality and team collaboration. The essay draws a parallel to the Lisp Curse, where extreme language power leads to isolated work and fragmented libraries. Ronacher argues that AI agents amplify this effect by allowing individuals to code faster but with less architectural coherence.

hackernews · cdrnsf · Jul 14, 16:57 · [Discussion](https://news.ycombinator.com/item?id=48909785)

**Background**: The Lisp Curse describes how Lisp's power enables solo developers to build custom solutions easily, discouraging collaboration and resulting in a poorer ecosystem. AI coding agents are software tools that autonomously write, modify, and debug code across multiple files, often lacking deep architectural understanding.

<details><summary>References</summary>
<ul>
<li><a href="https://www.freshcodeit.com/blog/myths-of-lisp-curse">What is the Curse of Lisp: Challenges and Opportunities</a></li>
<li><a href="https://agentic.ai/best/coding-agents">20 Best AI Coding Agents in 2026 — Agentic.ai</a></li>

</ul>
</details>

**Discussion**: Commenters note that using agents naively breaks composability, akin to poor Tetris play. One suggests manually fixing small annoyances to maintain architectural control, while another likens the situation to the Bipolar Lisp Programmer phenomenon.

**Tags**: `#software engineering`, `#AI agents`, `#composability`, `#programming philosophy`

---

<a id="item-5"></a>
## [Cursor 0day Vulnerability Prompts Full Disclosure](https://mindgard.ai/blog/cursor-0day-when-full-disclosure-becomes-the-only-protection-left) ⭐️ 8.0/10

A researcher disclosed a year-long unpatched vulnerability in Cursor, an AI-powered code editor, that allows arbitrary executables to run without user confirmation. The disclosure came after multiple reports to the vendor went unresolved for over six months. This vulnerability underscores the security risks in AI coding tools that execute code implicitly, and it reignites debate over responsible disclosure versus full disclosure when vendors fail to respond. Users of Cursor face potential compromise from malicious files in their workspace. The exploit leverages a Windows quirk where the current directory is searched before system PATH for executables; an attacker must place a malicious git.exe in the project folder. Cursor then executes it without any user prompt, unlike typical ACL behavior.

hackernews · Synthetic7346 · Jul 14, 17:58 · [Discussion](https://news.ycombinator.com/item?id=48910676)

**Background**: A zero-day vulnerability is a security flaw unknown to the vendor that lacks a patch, exposing users to potential attacks. Full disclosure is a practice where researchers publicly release vulnerability details after the vendor fails to address it in a timely manner. Cursor is an AI-powered code editor forked from Visual Studio Code, widely used for its intelligent coding assistance. The vulnerability reported here involves Cursor's integration with Git, where it searches for git.exe in the current working directory before consulting the system PATH.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zero-day_vulnerability">Zero-day vulnerability - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)">Full disclosure (computer security) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cursor_(code_editor)">Cursor (code editor)</a></li>

</ul>
</details>

**Discussion**: Commenters are divided: some argue the vulnerability is minor because it requires the attacker to already have placed a malicious executable, while others emphasize the lack of user prompt as dangerous. There is broad agreement that Cursor's vendor response was inadequate, with reports closed as 'informative' initially despite the issue persisting for months.

**Tags**: `#security`, `#vulnerability`, `#cursor`, `#disclosure`, `#code-editor`

---

<a id="item-6"></a>
## [Are we offloading too much thinking to AI?](https://www.artfish.ai/p/offloading-thinking-to-ai) ⭐️ 8.0/10

A high-scoring article on ArtFish sparks debate about whether over-reliance on AI for cognitive tasks is harmful, with 384 points and 387 comments engaging the technical community. As AI tools like LLMs become ubiquitous in knowledge work, this debate highlights the risk of eroding critical thinking and deep understanding, which could impact productivity and innovation. The discussion includes real-world examples, such as a junior developer unable to explain an AI-generated computation, and a commenter arguing that deep technical understanding remains valuable for effective AI use.

hackernews · yenniejun111 · Jul 14, 15:18 · [Discussion](https://news.ycombinator.com/item?id=48908178)

**Background**: Cognitive offloading is the practice of using external tools to reduce mental effort, from calculators to GPS. With advanced AI like LLMs, this has extended to reasoning and decision-making, raising concerns about skill atrophy and dependence.

**Discussion**: Community comments are largely critical of over-reliance, with users sharing anecdotes of juniors lacking fundamental understanding and worrying that AI use is replacing genuine learning. Some defend AI as a productivity tool, but the dominant sentiment is cautionary.

**Tags**: `#AI ethics`, `#critical thinking`, `#software engineering`, `#knowledge work`, `#AI dependence`

---

<a id="item-7"></a>
## [Lobste.rs Migrates from MariaDB to SQLite, Cuts Costs](https://simonwillison.net/2026/Jul/14/lobsters-sqlite/#atom-everything) ⭐️ 8.0/10

The community news site Lobsters completed its migration from MariaDB to SQLite over the weekend, resulting in lower CPU and memory usage, a snappier site, and halved VPS costs. This real-world migration provides a compelling case study for using SQLite in production web applications, demonstrating significant performance improvements and cost savings, and challenging the default choice of client-server databases for moderate-traffic sites. The Lobsters Rails application now runs on a single VPS with a primary SQLite database of about 3.8GB, plus separate cache (1.1GB), queue (218MB), and rack_attack (555MB) databases. The migration PR added 735 lines and removed 593 lines across 30 commits.

rss · Simon Willison · Jul 14, 19:44

**Background**: SQLite is a lightweight, embedded relational database engine that stores data in a single file, unlike client-server databases like MariaDB which require separate server processes. It is widely used in mobile and desktop apps but less common for web applications. MariaDB is a popular open-source relational database forked from MySQL.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/SQLite">SQLite</a></li>
<li><a href="https://en.wikipedia.org/wiki/MariaDB">MariaDB</a></li>

</ul>
</details>

**Discussion**: The Lobsters thread reported positive results, with the original poster noting CPU and memory usage down, site snappier, and plans to halve costs by removing the MariaDB VPS. Additional details on database sizes and architecture were shared.

**Tags**: `#SQLite`, `#Rails`, `#database migration`, `#performance`, `#web development`

---

<a id="item-8"></a>
## [Armin Ronacher: AI Agents May Erode Shared Software Understanding](https://simonwillison.net/2026/Jul/14/armin-ronacher/#atom-everything) ⭐️ 8.0/10

Armin Ronacher published an essay arguing that the shared language of a software project—the common understanding of concepts, boundaries, invariants, and ownership—is maintained by friction in processes like code review and cross-team coordination, and that AI agents could disrupt this synchronization. This perspective is significant because it highlights a subtle, often overlooked cost of AI-assisted programming: while agents increase individual productivity, they may reduce the cross-team awareness and shared mental models that keep large projects coherent. It challenges the assumption that faster code generation is always beneficial. Ronacher's core claim is that 'friction synchronizes people'—the deliberate slowness of reading others' code, asking questions, and coordinating is not all waste; it is how understanding spreads and consensus is preserved. AI agents that bypass these steps risk fragmenting the team's shared knowledge.

rss · Simon Willison · Jul 14, 18:04

**Background**: In large software projects, the team's shared understanding is often implicit, embedded in code reviews, discussions, and the experience of explaining changes. This 'shared language' goes beyond programming languages and documentation. Friction—like the effort required to modify a component owned by another team—forces developers to communicate and align, ensuring the system evolves coherently. AI agents that independently generate and modify code might bypass this friction, potentially undermining the collective understanding.

**Tags**: `#software engineering`, `#shared understanding`, `#AI agents`, `#code review`, `#software design`

---

<a id="item-9"></a>
## [Cloudflare Launches Precursor: Continuous Behavioral Bot Detection](https://blog.cloudflare.com/introducing-precursor/) ⭐️ 8.0/10

Cloudflare has launched Precursor, a client-side session-based verification engine that continuously monitors behavioral signals such as mouse movement, keyboard cadence, and scrolling to distinguish humans from AI bots. Precursor shifts bot detection from single-point challenges to continuous verification, making it harder for automated agents to evade detection while providing a frictionless user experience. This could become a new standard in web security for sites vulnerable to AI-driven scraping and fraud. Precursor uses dynamically injected JavaScript to collect signals throughout the entire browsing session and assembles them into a session-based analysis dashboard. It is available as a free beta for enterprise Bot Management customers, with general availability planned later this year.

telegram · zaihuapd · Jul 14, 09:44

**Background**: Traditional CAPTCHAs and even Cloudflare's Turnstile only verify users at specific entry points like login or checkout. Precursor extends verification across the entire session by analyzing human-typical micro-behaviors—such as natural mouse arc trajectories and cognitive pauses—that are difficult for AI to replicate accurately. This approach is complementary to Turnstile, covering the user journey beyond the initial challenge.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.cloudflare.com/introducing-precursor/">Introducing Precursor: detecting agentic behavior with continuous client-side signals</a></li>
<li><a href="https://developers.cloudflare.com/cloudflare-challenges/precursor/">Precursor · Cloudflare challenges docs</a></li>
<li><a href="https://tech.slashdot.org/story/26/07/13/1645252/cloudflare-precursor-watches-your-mouse-and-keyboard-to-decide-if-you-are-human">Cloudflare Precursor Watches Your Mouse and Keyboard To Decide If You Are Human - Slashdot</a></li>

</ul>
</details>

**Tags**: `#Cloudflare`, `#反机器人`, `#行为验证`, `#网络安全`, `#AI检测`

---

<a id="item-10"></a>
## [DeepSeek Raises Over $7.4B in First Round with Novel Control Structure](https://t.me/zaihuapd/42557) ⭐️ 8.0/10

DeepSeek raised over 500 billion yuan (approximately $7.4 billion) in its first-round funding, valuing the company at over $50 billion. The funding uses an unconventional limited partnership structure where investors put money into a vehicle managed by founder Liang Wenfeng, with a five-year lock-up and no voting rights. This monumental funding round underscores DeepSeek's rapid ascent as a major AI player and highlights a governance innovation that allows the founder to retain control despite massive external investment. It may set a precedent for other high-growth tech startups seeking to balance capital infusion with founder autonomy. Founder Liang Wenfeng personally invested 200 billion yuan in this round. Tencent and CATL are reportedly considering investments of 100 billion yuan and 50 billion yuan respectively, making them the largest external investors. The structure requires investors to accept a five-year lock-up and no voting rights.

telegram · zaihuapd · Jul 14, 11:06

**Background**: In a limited partnership structure, a general partner (GP) manages the fund and makes decisions, while limited partners (LPs) contribute capital but have no management control. This allows founders to raise funds without diluting voting power. By channeling investments through a limited partnership controlled by the founder, DeepSeek ensures Liang Wenfeng retains decision-making authority despite raising a large sum. Such structures are common in venture capital but relatively novel for direct startup funding rounds.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sohu.com/a/968465639_122554521">有限合伙架构：长期主义企业的控制权护航利器_股权_杰诚_公司</a></li>
<li><a href="https://k.sina.cn/article_7879922977_1d5ae152106801fx3y.html">DeepSeek创始人梁文锋具体采用了何种交易结构来保持控制权？|合伙企业...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Funding`, `#DeepSeek`, `#Governance`, `#Startup`

---

<a id="item-11"></a>
## [Telegram's t.me Domain Frozen by Registry](https://t.me/zaihuapd/42559) ⭐️ 8.0/10

Telegram's short link domain t.me has been placed under serverHold status by the registry as of July 13, 2025, effectively suspending DNS resolution and potentially disrupting short URL services. The domain, registered via GoDaddy with validity until 2035, now carries multiple EPP status codes including serverHold, prohibiting deletion, transfer, renewal, and updates. This incident impacts millions of Telegram users worldwide who rely on t.me links for sharing channels, groups, and bot access. The lack of an official explanation from Telegram or the registry introduces uncertainty and highlights vulnerabilities in domain-based infrastructure for widely-used platforms. The serverHold status is a registry-level suspension that removes the domain from the zone file, preventing DNS resolution. Additional status codes like clientDeleteProhibited and clientTransferProhibited are also applied, further restricting domain management. The exact reason for the freeze remains unknown; possible causes include legal action, abuse reports, or regulatory compliance issues.

telegram · zaihuapd · Jul 14, 12:48

**Background**: Domain names are managed by registries (which operate the top-level domain database) and registrars (which sell domains to end users). A serverHold status is set by the registry, typically for legal or abuse reasons, and is more severe than a clientHold set by the registrar. Telegram's t.me domain acts as a URL shortener for its platform, allowing users to share links like t.me/username. The freeze could break existing short links and prevent new ones from resolving.

<details><summary>References</summary>
<ul>
<li><a href="https://www.namecheap.com/support/knowledgebase/article.aspx/10717/46/why-was-my-domain-suspended-with-a-serverhold-or-clienthold-status/">Why was my domain suspended with a serverHold or clientHold ...</a></li>
<li><a href="https://www.godaddy.com/help/what-is-the-difference-between-a-registry-registrar-and-registrant-8039">What is the difference between a registry, registrar and ...</a></li>
<li><a href="https://www.icann.org/resources/pages/epp-status-codes-2014-06-16-en">EPP Status Codes | What Do They Mean, and Why Should I Know?</a></li>

</ul>
</details>

**Tags**: `#telegram`, `#domain`, `#dns`, `#outage`, `#registry`

---

<a id="item-12"></a>
## [DeepMind CEO Urges US-led Global AI Watchdog](https://www.theverge.com/tech/965270/google-deepmind-demis-hassabis-global-ai-watchdog) ⭐️ 8.0/10

Demis Hassabis, CEO of Google DeepMind, has called for a US-led global AI regulatory body that would evaluate frontier AI models before their deployment, aiming to launch by the end of 2025. This proposal from a leading AI figure could significantly shape international AI governance, potentially establishing a precedent for pre-deployment safety assessments and coordinated industry pauses when risks are too high. The proposed watchdog would consist of independent experts and open-source community representatives, and could mandate a coordinated industry-wide halt if a model poses excessive risk. Hassabis has been in discussions with the Trump administration, other AI labs, and European officials.

telegram · zaihuapd · Jul 14, 14:29

**Background**: Frontier AI models are highly capable foundation models that could possess dangerous capabilities sufficient to pose severe risks to public safety. As these models become more advanced, there is growing concern about their potential misuse or unintended consequences, prompting calls for proactive regulation before deployment.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/frontier-ai-regulation/">Frontier AI regulation: Managing emerging risks to public ...</a></li>
<li><a href="https://www.governance.ai/analysis/frontier-ai-regulation">Frontier AI Regulation | GovAI - Governance</a></li>

</ul>
</details>

**Tags**: `#AI regulation`, `#DeepMind`, `#Demis Hassabis`, `#global governance`, `#AI safety`

---

<a id="item-13"></a>
## [DeepSeek seeks $71B valuation in new round, develops AI chips](https://t.me/zaihuapd/42564) ⭐️ 8.0/10

Chinese AI startup DeepSeek has initiated preliminary talks with investors for a new funding round at a pre-money valuation of approximately $71 billion, just one month after closing its first round at $52 billion. Additionally, Reuters reported earlier this month that DeepSeek is developing its own AI chips to reduce reliance on Nvidia and Huawei. This rapid valuation surge—from $52B to $71B in a month—underscores the intense investor demand for leading Chinese AI startups, even amid geopolitical tensions. Developing proprietary AI chips signals DeepSeek's strategic push to control its supply chain and compete more independently with Western AI giants. The new round is reportedly at a pre-money valuation of $71 billion, following a $7 billion raise at a $52 billion valuation in late May 2026. The custom chip development is still early-stage and aims to lessen dependence on Nvidia and Huawei hardware.

telegram · zaihuapd · Jul 14, 15:15

**Background**: DeepSeek is a Chinese AI startup that gained global attention in early 2025 after its AI assistant topped app charts and caused U.S. tech stocks to dip, rivaling models from OpenAI. The company has since released upgraded models and expanded into African markets. Developing custom AI chips is a common strategy among major AI firms to optimize performance and reduce costs, though it requires significant investment and time.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek - Wikipedia</a></li>
<li><a href="https://www.usnews.com/news/top-news/articles/2026-07-07/exclusive-chinas-deepseek-developing-its-own-ai-chip-sources-say">Exclusive-China's DeepSeek Developing Its Own AI Chip ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#DeepSeek`, `#funding`, `#AI chips`, `#startup`

---

<a id="item-14"></a>
## [White House to Convene Power Companies on AI Electricity Costs](https://t.me/zaihuapd/42566) ⭐️ 8.0/10

The White House plans to convene power companies and data center developers in the coming weeks to secure voluntary commitments that AI-driven electricity demand increases will not be passed on to residential and business consumers. This initiative could set a precedent for how AI infrastructure costs are distributed, protecting consumers from rate hikes while supporting the rapid expansion of AI data centers. It involves major tech players and state governors, signaling a coordinated policy approach. Earlier this year, companies like Google, Meta, and OpenAI signed similar commitments at the White House, agreeing to bear the costs of power generation and grid upgrades for AI projects. The new phase aims to also include power utilities, data center operators, and state governors.

telegram · zaihuapd · Jul 14, 16:00

**Background**: AI data centers consume enormous amounts of electricity, straining grids and raising fears of higher energy bills for ordinary customers. The White House intervention aims to prevent cost shifting and encourage sustainable infrastructure investments.

**Tags**: `#AI`, `#Energy`, `#Policy`, `#Data Centers`, `#US Government`

---

<a id="item-15"></a>
## [US Approves Nvidia H200 Sales to ~10 Chinese Firms](https://t.me/zaihuapd/42567) ⭐️ 8.0/10

The U.S. Commerce Department has approved about 10 Chinese companies, including Alibaba and Tencent, to purchase Nvidia's H200 AI chips, but deliveries have not yet begun as Chinese guidance cautions buyers. This decision signals a potential easing of US chip export controls and could significantly boost Nvidia's revenue, while giving Chinese tech giants access to cutting-edge AI hardware amid intensifying US-China tech competition. Buyers include Alibaba, Tencent, ByteDance, and JD.com, with distributors like Lenovo and Foxconn also licensed; each customer can purchase up to 75,000 chips. Nvidia CEO Jensen Huang's visit to China is seen as a move to facilitate the deals.

telegram · zaihuapd · Jul 15, 00:14

**Background**: The H200 Tensor Core GPU is Nvidia's high-end AI accelerator, built on the Hopper architecture with enhanced memory (141GB HBM3e) and bandwidth (4.8 TB/s), offering up to 45% faster LLM inference than the H100. Prior restrictions limited China's access to advanced AI chips, spurring development of domestic alternatives. The approval comes amid ongoing US-China trade tensions and a push for AI self-sufficiency in China.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/data-center/h200/">H200 GPU | NVIDIA</a></li>
<li><a href="https://www.cnbc.com/2026/07/14/nvidia-h200-ai-chips-china.html">Commerce official says Nvidia H200 AI chips have been shipped ...</a></li>
<li><a href="https://introl.com/blog/h100-vs-h200-vs-b200-choosing-the-right-nvidia-gpus-for-your-ai-workload">H100 vs H200 vs B200: NVIDIA GPU Comparison | Introl Blog</a></li>

</ul>
</details>

**Tags**: `#AI hardware`, `#US-China trade`, `#H200`, `#Nvidia`, `#semiconductor`

---