---
layout: default
title: "Horizon Summary: 2026-06-19 (EN)"
date: 2026-06-19
lang: en
---

> From 37 items, 13 important content pieces were selected

---

1. [10K GitHub Repos Found Distributing Trojan Malware](#item-1) ⭐️ 9.0/10
2. [Noam Shazeer Joins OpenAI](#item-2) ⭐️ 9.0/10
3. [GLM-5.2: Powerful Open-Weights LLM Released by Z.ai](#item-3) ⭐️ 9.0/10
4. [Ubiquiti Unveils Enterprise ZFS-Based NAS](#item-4) ⭐️ 8.0/10
5. [Cornell's Advanced Compilers Course Now Free Online Self-Guided](#item-5) ⭐️ 8.0/10
6. [Hospitals repurposing drugs at 90% lower cost](#item-6) ⭐️ 8.0/10
7. [GDPR forced consent fine: €1.8M for Elkjop loyalty club](#item-7) ⭐️ 8.0/10
8. [Modos Color E-Paper Monitor Hits 60Hz Refresh Rate](#item-8) ⭐️ 8.0/10
9. [Datasette Apps: Sandboxed Custom HTML Apps with SQL Access](#item-9) ⭐️ 8.0/10
10. [Charity Majors: AI Upends Code Economics](#item-10) ⭐️ 8.0/10
11. [Apple and Intel Reach Preliminary Chip Manufacturing Deal](#item-11) ⭐️ 8.0/10
12. [Xiaomi Open-Sources Miloco 2.0 AI Smart Home Solution](#item-12) ⭐️ 8.0/10
13. [China Proposes Regulations for Blockchain-Based Digital Identity Interoperability](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [10K GitHub Repos Found Distributing Trojan Malware](https://orchidfiles.com/github-repositories-distributing-malware/) ⭐️ 9.0/10

A researcher discovered over 10,000 GitHub repositories that distribute Trojan malware by manipulating commits, such as deleting and pushing new commits every few hours. This massive-scale attack poses a serious threat to open-source supply chain security, as automated agents may unknowingly clone infected repositories as dependencies, potentially leading to widespread infections. The malicious repositories are often clones of legitimate projects with Trojans injected, and they are not targeting humans but automated agents that search for dependencies. The frequent commit manipulation helps them appear in search results.

hackernews · theorchid · Jun 18, 11:45 · [Discussion](https://news.ycombinator.com/item?id=48583928)

**Background**: A supply chain attack exploits the trust relationships between software components, where attackers compromise a dependency to infect downstream users. GitHub is a popular platform for hosting open-source code, but its permissive nature can be abused. Commit manipulation, including techniques like commit stomping, allows attackers to alter repository history and evade detection.

<details><summary>References</summary>
<ul>
<li><a href="https://cybersecuritynews.com/commit-stomping/">Commit Stomping - An Offensive Technique Let Hackers Manipulate ...</a></li>
<li><a href="https://cybersecuritynews.com/23000-github-repositories-targeted/">23,000 GitHub Repositories Targeted In Supply Chain Attack</a></li>

</ul>
</details>

**Discussion**: Commenters discussed reasons for the attack strategy: targeting agents rather than humans, and manipulating commit times to appear at the top of 'Last Updated' searches. One user reported similar victimization, finding their name attached to unknown malware-distributing projects.

**Tags**: `#security`, `#malware`, `#GitHub`, `#supply chain`, `#Trojan`

---

<a id="item-2"></a>
## [Noam Shazeer Joins OpenAI](https://twitter.com/NoamShazeer/status/2067400851438932297) ⭐️ 9.0/10

Noam Shazeer, a co-author of the seminal 'Attention Is All You Need' paper and co-founder of Character.AI, has left Google to join OpenAI, as announced via his tweet and confirmed by Reuters. This move comes shortly after his return to Google in 2024 as a Gemini co-lead. Shazeer's move is significant because he is a key architect of the transformer architecture, which underpins most modern large language models. His joining OpenAI could accelerate their research and development efforts, intensifying competition in the AI industry. Shazeer returned to Google in 2024 through a licensing and talent deal with Character.AI reportedly valued at around $2.7 billion, where he became a co-lead for the Gemini project. His departure to OpenAI is unexpected and marks a notable shift in talent between leading AI companies.

hackernews · lukasgross · Jun 18, 00:26 · [Discussion](https://news.ycombinator.com/item?id=48578913)

**Background**: Noam Shazeer is a renowned computer scientist who joined Google in 2000 and contributed to early projects like spell-checking and AdSense. He was one of the eight co-authors of the 2017 paper 'Attention Is All You Need', which introduced the transformer architecture that revolutionized AI by enabling efficient parallel processing. Transformers are the foundation of large language models such as GPT-4 and Google's Gemini.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Noam_Shazeer">Noam Shazeer</a></li>
<li><a href="https://en.wikipedia.org/wiki/Transformer_architecture">Transformer architecture</a></li>

</ul>
</details>

**Discussion**: Commenters expressed surprise at Shazeer's swift departure from Google after his return, with some recalling his legendary status at Google and his deep technical contributions. The discussion also highlighted the broader talent war between Google and OpenAI, and speculated on the potential impact on the development of next-generation AI models.

**Tags**: `#OpenAI`, `#Noam Shazeer`, `#AI industry`, `#transformers`, `#personnel move`

---

<a id="item-3"></a>
## [GLM-5.2: Powerful Open-Weights LLM Released by Z.ai](https://simonwillison.net/2026/Jun/17/glm-52/#atom-everything) ⭐️ 9.0/10

Z.ai released GLM-5.2, a 753B parameter Mixture-of-Experts text-only LLM with a 1 million token context window, under the MIT license. GLM-5.2 achieves top scores on the Artificial Analysis Intelligence Index, surpassing other open-weights models like MiniMax-M3 and DeepSeek V4 Pro, and ranks second on Code Arena WebDev, demonstrating exceptional performance despite being text-only. The model uses 43k output tokens per task on average, which is higher than comparable models, indicating higher token consumption. It is available via OpenRouter at $1.40/million input tokens and $4.40/million output tokens, significantly cheaper than GPT-5.5 and Claude Opus.

rss · Simon Willison · Jun 17, 23:58

**Background**: Mixture of Experts (MoE) is an architecture that activates only a subset of parameters per token, enabling large model capacity with efficient computation. The context window is the maximum amount of text an LLM can consider at once; GLM-5.2's 1M token window is a significant increase from its predecessor's 200k.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/google-cloud/how-mixture-of-experts-llms-work-58b3ba8e0349">How Mixture-of-Experts LLMs Work - Medium</a></li>
<li><a href="https://en.wikipedia.org/wiki/Context_window">Context window - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#open-weights`, `#LLM`, `#AI`, `#natural language processing`, `#MIT license`

---

<a id="item-4"></a>
## [Ubiquiti Unveils Enterprise ZFS-Based NAS](https://blog.ui.com/article/introducing-enterprise-nas) ⭐️ 8.0/10

Ubiquiti announced a new enterprise NAS product built on the ZFS file system, marking its entry into the network-attached storage market. The device features dual 25 Gigabit SFP28 ports and redundant power supplies. This is significant because Ubiquiti, a major networking vendor, is entering the NAS space with ZFS, a file system known for data integrity and advanced features. It could challenge existing NAS providers like QNAP and Synology, especially for users who prefer a no-subscription model. The NAS is priced at $3999, targeting enterprise users. Community discussions highlight concerns about Ubiquiti's past security and software quality issues, as well as potential performance bottlenecks with spinning hard drives despite the high-speed network interfaces.

hackernews · ksec · Jun 18, 14:24 · [Discussion](https://news.ycombinator.com/item?id=48585866)

**Background**: ZFS is an advanced file system that combines volume management and data protection features, such as checksums for data integrity, snapshots, and replication. Unlike traditional file systems, ZFS can span multiple drives in a pool and protect against bit rot and corruption. Ubiquiti is known for its networking hardware but has faced criticism for software reliability and security incidents.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ZFS">ZFS - Wikipedia</a></li>
<li><a href="https://itsfoss.com/what-is-zfs/">What is ZFS? Why are People Crazy About it?</a></li>

</ul>
</details>

**Discussion**: The community shows mixed sentiment: some praise ZFS and the no-subscription model, while others express concerns about Ubiquiti's past security lapses and software quality. There is also technical skepticism about saturating 25 Gbps links with spinning drives.

**Tags**: `#Ubiquiti`, `#NAS`, `#ZFS`, `#Enterprise Storage`, `#Hardware`

---

<a id="item-5"></a>
## [Cornell's Advanced Compilers Course Now Free Online Self-Guided](https://www.cs.cornell.edu/courses/cs6120/2025fa/self-guided/) ⭐️ 8.0/10

Cornell University's CS 6120: Advanced Compilers, a PhD-level course taught by Adrian Sampson, is now available as a free self-guided online resource, including lecture videos and assignments. This course provides accessible, high-quality advanced compiler education to a global audience, filling a gap for self-learners interested in systems and programming language implementation. The course covers both classic topics like data flow and SSA form, and research-flavored topics such as JIT compilation, parallelization, and garbage collection. It includes a blog and GitHub repository for hands-on work.

hackernews · ibobev · Jun 18, 11:04 · [Discussion](https://news.ycombinator.com/item?id=48583606)

**Background**: Advanced compilers courses traditionally require a CS background and are often only taught at universities. This self-guided version removes barriers, offering lecture videos and assignments similar to the in-person offering.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cs.cornell.edu/courses/cs6120/2020fa/self-guided/">CS 6120: Advanced Compilers: The Self-Guided Online Course</a></li>
<li><a href="https://github.com/sampsyo/cs6120">GitHub - sampsyo/cs6120: advanced compilers</a></li>

</ul>
</details>

**Discussion**: Comments on Hacker News note that the dynamic compilers section focuses on trace compilation, which some consider a dead end, but praise the overall course quality. There is debate over whether the content is truly 'advanced' or suitable for a first compilers course.

**Tags**: `#compilers`, `#online-course`, `#advanced-compilers`, `#education`, `#systems`

---

<a id="item-6"></a>
## [Hospitals repurposing drugs at 90% lower cost](https://www.kcl.ac.uk/news/hospitals-and-universities-repurposing-drugs-at-90-lower-cost) ⭐️ 8.0/10

Hospitals and universities are repurposing existing drugs for new therapeutic uses, achieving up to 90% cost reduction compared to patented alternatives. For example, the cancer drug bevacizumab (Avastin) is used off-label for macular degeneration at $50 per dose versus $1,500 for the approved drug Lucentis. This practice challenges pharmaceutical pricing models and expands access to affordable treatments, especially for rare or neglected diseases. It highlights systemic issues in drug pricing and could shift incentives toward evidence-based repurposing rather than developing expensive new drugs. Drug repurposing benefits from reduced clinical trial steps and known safety profiles, but it lacks a clear regulatory pathway for new indications without manufacturer consent. Community comments note that esketamine (Spravato) is a patented modification of off-patent ketamine, yet evidence suggests it is less effective than the original.

hackernews · giuliomagnifico · Jun 18, 10:33 · [Discussion](https://news.ycombinator.com/item?id=48583386)

**Background**: Drug repurposing (also called drug repositioning) identifies new uses for existing FDA-approved drugs, potentially reducing time and cost to reach market. It relies on known safety and pharmacokinetic data, and is often investigated for rare diseases where new drug development is uneconomical.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Drug_repurposing">Drug repurposing</a></li>
<li><a href="https://www.fda.gov/drugs/resources-drugs/drug-repurposing">Drug Repurposing | FDA</a></li>

</ul>
</details>

**Discussion**: Commenters provided concrete examples and personal experiences: one noted the Avastin/Lucentis cost disparity and molecular similarity; another highlighted the nonprofit Cures Within Reach for Huntington's disease. A third criticized Spravato as a less effective patented version of ketamine, illustrating broken incentives in US healthcare.

**Tags**: `#drug repurposing`, `#healthcare costs`, `#pharmaceuticals`, `#public health`

---

<a id="item-7"></a>
## [GDPR forced consent fine: €1.8M for Elkjop loyalty club](https://www.thatprivacyguy.com/blog/elkjop-forced-consent-fine/) ⭐️ 8.0/10

The Norwegian data protection authority Datatilsynet fined electronics retailer Elkjop NOK 20 million (€1.8M) for requiring customers to consent to marketing as a condition of joining its loyalty club, violating GDPR's requirement of freely given consent. This enforcement clarifies that GDPR prohibits conditioning service membership on consent to marketing, setting a precedent for loyalty programs across the EEA. It also demonstrates that individual complaints can drive significant regulatory action, empowering privacy advocates. The fine came five years after a privacy advocate warned Elkjop that its practice was unlawful. Elkjop explicitly stated in writing that receiving marketing was a condition of membership, which constituted forced consent. The official decision is available in English from Datatilsynet.

hackernews · speckx · Jun 18, 18:31 · [Discussion](https://news.ycombinator.com/item?id=48589501)

**Background**: Under GDPR Article 4(11), consent must be freely given, specific, informed, and unambiguous. Article 7(4) prohibits conditioning service access on consent to non-essential processing. The EDPB guidelines emphasize that bundling consent with service terms invalidates consent, as individuals cannot truly choose.

<details><summary>References</summary>
<ul>
<li><a href="https://www.thatprivacyguy.com/blog/elkjop-forced-consent-fine/">I told them forced consent was unlawful. Five years later it ...</a></li>
<li><a href="https://www.edpb.europa.eu/sites/default/files/files/file1/edpb_guidelines_202005_consent_en.pdf">PDF Guidelines 05/2020 on consent under Regulation 2016/679 Version 1 - Europa</a></li>

</ul>
</details>

**Discussion**: Commenters largely praised the outcome, with some noting the irony that the complainant sued the entity that won the case for him. One commenter provided links to the official decision in Norwegian and an English machine translation. Another expressed hope that more individuals will exercise their privacy rights.

**Tags**: `#GDPR`, `#privacy`, `#data protection`, `#forced consent`, `#fine`

---

<a id="item-8"></a>
## [Modos Color E-Paper Monitor Hits 60Hz Refresh Rate](https://spectrum.ieee.org/modos-e-paper-monitor) ⭐️ 8.0/10

A two-person startup, Modos, is developing a 13.3-inch color e-paper monitor with a native resolution of 3200x2400 and a 60Hz refresh rate, which is a significant leap for e-paper displays that traditionally have low refresh rates. This development could make e-paper displays viable for general-purpose computing, including video playback and interactive tasks, due to the high refresh rate and resolution, potentially reducing eye strain and power consumption compared to LCDs. The monitor, named Modos Flow, supports touch input and is being funded through a crowdfunding campaign. The 60Hz refresh rate raises questions about the longevity of the electrophoretic display panel, as higher refresh rates may accelerate wear.

hackernews · Vinnl · Jun 18, 11:41 · [Discussion](https://news.ycombinator.com/item?id=48583897)

**Background**: E-paper displays, such as those based on E Ink technology, use electrophoretic particles to reflect ambient light, offering low power consumption and readability in bright sunlight. However, they typically suffer from slow refresh rates (often below 20Hz) and limited color reproduction, restricting their use to applications like e-readers and digital signage. Modos' monitor aims to overcome these limitations by achieving a 60Hz refresh rate and high resolution, potentially opening up new use cases.

<details><summary>References</summary>
<ul>
<li><a href="https://news.samsung.com/us/story-behind-samsung-color-e-paper-digital-signage-solution-displays-2-5-million-colors-without-continuous-power/">The Story Behind Samsung Color E-Paper: The Digital Signage Solution ...</a></li>
<li><a href="https://news.samsung.com/global/interview-i-thought-it-was-real-paper-the-story-behind-samsung-color-e-paper-the-digital-signage-solution-that-displays-2-5-million-colors-without-continuous-power">[Interview] 'I Thought It Was Real Paper' — The Story Behind Samsung ...</a></li>

</ul>
</details>

**Discussion**: Community members expressed excitement about the development, with some noting a useful YouTube video from the creator. One commenter raised concerns about the impact of 60Hz refresh rate on panel longevity, while another highlighted the potential for outdoor-capable, low-power devices. Overall sentiment is positive, with praise for the specifications and hope for broader adoption.

**Tags**: `#e-paper`, `#displays`, `#startups`, `#hardware`, `#innovation`

---

<a id="item-9"></a>
## [Datasette Apps: Sandboxed Custom HTML Apps with SQL Access](https://simonwillison.net/2026/Jun/18/datasette-apps/#atom-everything) ⭐️ 8.0/10

Simon Willison launched the datasette-apps plugin for Datasette, allowing users to host custom HTML+JavaScript applications inside sandboxed iframes with read/write SQL access to the underlying database. This plugin significantly extends Datasette's capabilities from a data exploration tool to a platform for building interactive SQL-backed web apps, benefiting data journalists, researchers, and developers who want to create custom interfaces without leaving the Datasette ecosystem. Apps run in a constrained iframe with sandbox="allow-scripts allow-forms" and an injected CSP header that blocks outbound HTTP requests, preventing data exfiltration. Write queries are only allowed if configured via stored queries.

rss · Simon Willison · Jun 18, 23:58

**Background**: Datasette is an open-source tool that turns SQLite databases into interactive web pages with a JSON API. It is widely used for data publishing and exploration. The datasette-apps plugin originated as a feature for Datasette Agent but was spun off as a standalone plugin because the sandboxed pattern proved broadly useful.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jun/18/datasette-apps/">Datasette Apps: Host custom HTML applications inside Datasette</a></li>
<li><a href="https://datasette.io/plugins">Datasette Plugins</a></li>
<li><a href="https://docs.datasette.io/en/stable/plugins.html">Plugins - Datasette documentation</a></li>

</ul>
</details>

**Tags**: `#Datasette`, `#plugin`, `#data visualization`, `#SQL`, `#JavaScript`

---

<a id="item-10"></a>
## [Charity Majors: AI Upends Code Economics](https://simonwillison.net/2026/Jun/17/charity-majors/#atom-everything) ⭐️ 8.0/10

Charity Majors observes that in 2025, the economics of code production shifted dramatically: generating code became effectively free and instant, instead of hard, time-consuming, and expensive. This paradigm shift means code is now disposable and regenerable, forcing a rethinking of software engineering practices and the value of code craftsmanship. The quote is from her Substack article 'AI demands more engineering discipline. Not less,' highlighting that despite cheap code generation, engineering discipline becomes more important.

rss · Simon Willison · Jun 17, 17:12

**Background**: Traditionally, code was expensive to write and maintain, so engineers treated it as a valuable asset to be reused and curated. AI-powered code generation tools have flipped this, making it cheaper to regenerate than to maintain old code.

**Tags**: `#ai-assisted-programming`, `#software-engineering`, `#generative-ai`, `#economics-of-code`

---

<a id="item-11"></a>
## [Apple and Intel Reach Preliminary Chip Manufacturing Deal](https://t.me/zaihuapd/42031) ⭐️ 8.0/10

Apple and Intel have reached a preliminary agreement for Intel to manufacture chips for some Apple devices, with the deal finalized after over a year of negotiations and with heavy involvement from the US government. This agreement diversifies Apple's chip supply away from sole reliance on TSMC and boosts Intel's foundry business, with significant implications for semiconductor supply chain geopolitics and US manufacturing goals. It is not yet specified which Apple products—iPhone, iPad, or Mac—will use Intel-made chips. Intel now counts Apple alongside Nvidia and SpaceX as foundry customers.

telegram · zaihuapd · Jun 18, 09:19

**Background**: In the semiconductor industry, chip foundries are factories that manufacture integrated circuits. Traditionally, Intel was an integrated device manufacturer (IDM) that designed and manufactured its own chips, while Apple relied on foundries like TSMC. Intel launched Intel Foundry Services to manufacture chips for external customers, aiming to compete with TSMC and Samsung.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chip_foundry">Chip foundry</a></li>
<li><a href="https://en.wikipedia.org/wiki/Intel_Foundry_Services">Intel Foundry Services</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#Intel`, `#chip manufacturing`, `#semiconductor`, `#foundry`

---

<a id="item-12"></a>
## [Xiaomi Open-Sources Miloco 2.0 AI Smart Home Solution](https://github.com/XiaoMi/xiaomi-miloco) ⭐️ 8.0/10

Xiaomi has released Miloco 2.0 as an open-source AI-driven smart home platform, which uses MiMo large model running as an OpenClaw plugin to proactively control devices based on audio and video inputs from Mi Home cameras. This move makes powerful AI-driven home automation accessible to developers and enthusiasts, potentially advancing open-source smart home ecosystems by integrating large language models for proactive reasoning and control. Miloco 2.0 requires macOS or Linux (Windows via WSL), at least 4 GB RAM and 256 GB storage, plus a Xiaomi account and MiMo API key. The cloud dependency for perception and agent leads to ongoing API fees, and the project is limited to non-commercial use.

telegram · zaihuapd · Jun 18, 12:23

**Background**: Miloco is Xiaomi's open-source smart home platform that leverages AI to automate home environments. The MiMo large model is Xiaomi's in-house large language model, offering various pricing tiers. OpenClaw is an open-source AI agent framework that supports plugins like Miloco. By combining these, Miloco 2.0 can interpret camera feeds and proactively adjust smart devices.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/XiaoMi/xiaomi-miloco">Xiaomi Miloco - GitHub</a></li>
<li><a href="https://xiaomiforall.com/xiaomi-miloco-2-0-smart-home-ai/">Xiaomi Miloco 2.0: The AI Revolution for Your Smart Home</a></li>
<li><a href="https://open-claw.bot/docs/tools/plugins/">OpenClaw Plugins : Extend Your AI Agent | OpenClaw</a></li>

</ul>
</details>

**Tags**: `#open source`, `#smart home`, `#AI`, `#Xiaomi`, `#large language model`

---

<a id="item-13"></a>
## [China Proposes Regulations for Blockchain-Based Digital Identity Interoperability](https://www.cac.gov.cn/2026-06/18/c_1783525605384124.htm) ⭐️ 8.0/10

On June 18, 2026, China's Cyberspace Administration released a draft regulation seeking public comment on promoting distributed digital identity interoperability and mutual recognition based on blockchain technology. This regulation could establish a national framework for decentralized identity management, enhancing data security and user control while enabling cross-sector identity verification across finance, transportation, customs, taxation, and digital currency systems. The draft specifies that distributed digital identities consist of identifiers, keys, verifiable credentials, and verifiable declarations. It also mandates that users under 14 require parental consent for identity issuance.

telegram · zaihuapd · Jun 19, 01:39

**Background**: Distributed digital identity (DID) is a decentralized identity model that allows users to control their own identity data without relying on a central authority. Using blockchain, DIDs enable secure, verifiable credentials that can be used across different platforms. Traditional centralized identity systems often suffer from privacy risks and cross-domain trust issues.

<details><summary>References</summary>
<ul>
<li><a href="https://www.news.cn/politics/20260618/780f2dbba382444385e6b59d0cd53dd4/c.html">国家互联网信息办公室关于《促进分布式数字身份互通互认应用规定（征求意见稿）》公开征求意见的通知-新华网</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/506783361">Dpki的崛起之路——分布式数字身份 (Did) - 知乎</a></li>
<li><a href="https://www.secrss.com/articles/84215">分布式数字身份技术概述 - 安全内参 | 决策者的网络安全知识库</a></li>

</ul>
</details>

**Tags**: `#distributed digital identity`, `#blockchain`, `#regulation`, `#China`, `#data security`

---