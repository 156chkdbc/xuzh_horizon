---
layout: default
title: "Horizon Summary: 2026-07-09 (EN)"
date: 2026-07-09
lang: en
---

> From 38 items, 14 important content pieces were selected

---

1. [TypeScript 7 Announced with Rust-Based Rewrite](#item-1) ⭐️ 9.0/10
2. [Cloudflare Meerkat: First Production Async Consensus](#item-2) ⭐️ 9.0/10
3. [Bun Rewritten from Zig to Rust Using AI Agents](#item-3) ⭐️ 9.0/10
4. [Critical Android Vulnerability Chain Enables Remote Root on All Versions](#item-4) ⭐️ 9.0/10
5. [John Deere FTC Settlement Advances Right to Repair](#item-5) ⭐️ 8.0/10
6. [OpenAI on removing noise from coding benchmarks](#item-6) ⭐️ 8.0/10
7. [Mistral Unveils Robostral Navigate for Map-Less Robot Navigation](#item-7) ⭐️ 8.0/10
8. [Microsoft releases Flint, a visualization language for AI agents](#item-8) ⭐️ 8.0/10
9. [xAI Unveils Grok 4.5: Cost-Efficient but Controversial](#item-9) ⭐️ 8.0/10
10. [OpenAI Unveils GPT-Live Voice Mode with GPT-5.5 Delegation](#item-10) ⭐️ 8.0/10
11. [sqlite-utils 4.0 Released with Schema Migrations](#item-11) ⭐️ 8.0/10
12. [Huawei 5G Flagship Returns Overseas with 1100 Mbps Speed](#item-12) ⭐️ 8.0/10
13. [Cloudflare and OpenAI Pilot Global Network Data for AI Search](#item-13) ⭐️ 8.0/10
14. [Smartphone app identification via EM signals achieves 99.07% accuracy](#item-14) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [TypeScript 7 Announced with Rust-Based Rewrite](https://devblogs.microsoft.com/typescript/announcing-typescript-7-0/) ⭐️ 9.0/10

Microsoft announced TypeScript 7.0, a major release featuring a completely new architecture based on a Rust rewrite, delivering up to 11.9x faster build times compared to TypeScript 6. This performance leap addresses a long-standing issue of TypeScript compilation speed, making it significantly more efficient for large codebases like VS Code, Sentry, and Playwright, and could encourage wider adoption of typed JavaScript. Benchmarks show speedups ranging from 7.7x to 11.9x across various codebases; the rewrite in Rust replaces the previous TypeScript-based compiler, achieving gains through native performance and parallelization.

hackernews · DanRosenwasser · Jul 8, 16:06 · [Discussion](https://news.ycombinator.com/item?id=48833715)

**Background**: TypeScript is a typed superset of JavaScript that compiles to plain JavaScript. Its compiler (tsc) has historically been written in TypeScript itself, leading to performance bottlenecks on large projects. A Rust rewrite had been speculated for years, with community projects like STC attempting it, but Microsoft's official effort now brings dramatic improvements.

<details><summary>References</summary>
<ul>
<li><a href="https://www.totaltypescript.com/rewriting-typescript-in-rust">Rewriting TypeScript in Rust? You'd have to be... | Total TypeScript</a></li>
<li><a href="https://medium.com/nerd-for-tech/curious-why-microsoft-did-not-use-rust-to-rewrite-the-typescript-compiler-16f1611bfd1d">Curious why Microsoft did not use Rust to rewrite the TypeScript Compiler? | by Olenin Slava | Nerd For Tech | Medium</a></li>

</ul>
</details>

**Discussion**: The community expressed excitement and congratulations, with many noting the impressive engineering feat of maintaining two codebases. Some users highlighted the continued support for JSDoc type syntax and the impact on developer experience.

**Tags**: `#TypeScript`, `#performance`, `#programming languages`, `#compiler`, `#Microsoft`

---

<a id="item-2"></a>
## [Cloudflare Meerkat: First Production Async Consensus](https://blog.cloudflare.com/meerkat-introduction/) ⭐️ 9.0/10

Cloudflare has introduced Meerkat, the first production implementation of the QuePaxa asynchronous consensus algorithm, designed for globally distributed systems. This is a groundbreaking step as it brings asynchronous consensus, which is resilient to network delays and timeouts, from theory to real-world deployment, potentially improving reliability for distributed systems operating under adverse network conditions. Meerkat is leaderless and does not rely on timeouts, unlike traditional consensus algorithms like Paxos and Raft. However, it requires global consensus for every read operation, which may introduce additional latency.

hackernews · bobnamob · Jul 8, 13:18 · [Discussion](https://news.ycombinator.com/item?id=48831565)

**Background**: Consensus algorithms are critical for distributed systems to agree on a value despite failures. Traditional algorithms like Paxos and Raft are partially synchronous, relying on timeouts for liveness, which can cause issues in unstable networks. Asynchronous consensus algorithms, like QuePaxa, do not depend on timeouts, making them more robust, but they are harder to implement efficiently.

<details><summary>References</summary>
<ul>
<li><a href="https://bford.info/pub/os/quepaxa/">QuePaxa: Escaping the Tyranny of Timeouts in Consensus – Bryan Ford's Home Page</a></li>
<li><a href="https://en.wikipedia.org/wiki/Consensus_(computer_science)">Consensus (computer science) - Wikipedia</a></li>
<li><a href="https://github.com/dedis/quepaxa">GitHub - dedis/quepaxa: This is the code repository for QuePaxa project (formerly Raxos or QSCOD) · GitHub</a></li>

</ul>
</details>

**Discussion**: Community comments express both excitement and skepticism. Some appreciate the novelty of a production asynchronous consensus implementation, while others question its performance compared to leaderless protocols and note that reads require consensus, potentially limiting use cases. There is also debate about whether the comparison to Raft is fair, as Raft is specifically leader-based.

**Tags**: `#distributed systems`, `#consensus algorithms`, `#asynchronous consensus`, `#QuePaxa`, `#Cloudflare`

---

<a id="item-3"></a>
## [Bun Rewritten from Zig to Rust Using AI Agents](https://simonwillison.net/2026/Jul/8/rewriting-bun-in-rust/#atom-everything) ⭐️ 9.0/10

Jarred Sumner announced that Bun has been rewritten from Zig to Rust using AI coding agents, resulting in improved stability, 5% performance gain, and 20% smaller binary size. This demonstrates that large-scale rewrites traditionally considered too risky are now feasible with AI assistance, and it validates Rust's memory safety benefits for performance-critical runtimes like Bun. The rewrite cost approximately $165,000 in API tokens (5.9 billion uncached input tokens, 690 million output tokens) and was done in 11 days by one engineer using Claude Code and Fable, with a TypeScript test suite acting as a conformance suite.

rss · Simon Willison · Jul 8, 23:57

**Background**: Bun is a fast JavaScript runtime and toolchain written originally in Zig. Zig is a low-level language that offers manual memory management, while Rust provides memory safety through its ownership model. Mixing garbage-collected JavaScript with manual memory management in Zig led to use-after-free and double-free bugs that motivated the rewrite. The rewrite leveraged agentic engineering, where AI agents autonomously perform coding tasks guided by a test suite, a methodology that has gained traction in 2026.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/guides/agentic-engineering-patterns/what-is-agentic-engineering/">What is agentic engineering? - Agentic Engineering Patterns - Simon Willison's Weblog</a></li>
<li><a href="https://www.langchain.com/blog/agentic-engineering-redefining-software-engineering">Agentic Engineering: How Swarms of AI Agents Are Redefining Software Engineering</a></li>
<li><a href="https://en.wikipedia.org/wiki/Garbage_collection_(computer_science)">Garbage collection (computer science) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Comments highlight that the rewrite is a strong endorsement for Rust's memory safety and shows the cost-effectiveness of AI-assisted rewrites compared to hiring engineers. Some discuss that it's not good for Zig that a naive rewrite improved stability and performance, and others note the power of a strong test suite in enabling LLM-based code generation.

**Tags**: `#Bun`, `#Rust`, `#Zig`, `#JavaScript runtime`, `#software engineering`

---

<a id="item-4"></a>
## [Critical Android Vulnerability Chain Enables Remote Root on All Versions](https://www.coolapk.com/feed/72700258?s=ZGQ2MTVlZjYxMDYyNTM3ZzZhNGUzOThjega1640) ⭐️ 9.0/10

Security firm Nebula disclosed a remote root exploit chain affecting all Android versions, including Android 17, by combining a Firefox browser vulnerability with a 15-year-old Linux kernel flaw (CVE-2026-43499, GhostLock). A proof-of-concept has been published on GitHub, and vendors have been notified. This vulnerability chain allows attackers to gain persistent root access on any Android device simply by tricking a user into clicking a malicious link, posing a massive threat to billions of users. It underscores the critical need for timely patching and the risks of legacy kernel bugs in mobile platforms. The exploit uses a Firefox browser vulnerability (up to version 151.0.2) to achieve code execution, then leverages GhostLock (CVE-2026-43499) for kernel-level privilege escalation to root. The attack completes within one minute and grants full device control via ADB; the Linux kernel has already released a fix, but Android patches are pending.

telegram · zaihuapd · Jul 8, 13:01

**Background**: Android Debug Bridge (ADB) is a command-line tool that allows developers to communicate with Android devices for debugging and control. A 'remote root' exploit allows an attacker to gain superuser (root) privileges without physical access to the device. GhostLock (CVE-2026-43499) is a 15-year-old use-after-free vulnerability in the Linux kernel's real-time mutex (rt-mutex) code, introduced in 2011 and affecting most Linux distributions since then.

<details><summary>References</summary>
<ul>
<li><a href="https://threat-modeling.com/cve-2026-43499-ghostlock-linux-kernel-root-container-escape/">CVE-2026-43499 "GhostLock": 15-Year-Old Linux Kernel Flaw Gives Local Users Root Access and Container Escape — Public PoC Released - Threat-Modeling.com</a></li>
<li><a href="https://thehackernews.com/2026/07/15-year-old-ghostlock-flaw-enables-root.html">15-Year-Old GhostLock Flaw Enables Root and Container Escape on Most Linux Distros</a></li>
<li><a href="https://developer.android.com/tools/adb">Android Debug Bridge (adb) | Android Studio | Android Developers</a></li>

</ul>
</details>

**Tags**: `#Android`, `#security`, `#vulnerability`, `#Linux kernel`, `#remote root`

---

<a id="item-5"></a>
## [John Deere FTC Settlement Advances Right to Repair](https://apnews.com/article/john-deere-right-to-repair-agriculture-equipment-cb7514ffedb95c130a976af661f2bc02) ⭐️ 8.0/10

John Deere has settled with the Federal Trade Commission (FTC) and five states, agreeing to allow owners and independent repair shops to fix their own equipment. This settlement is a landmark win for the right-to-repair movement, potentially reducing monopoly on repairs and lowering costs for farmers and consumers. As part of the settlement, John Deere will pay $1 million collectively to the five states and be subject to compliance oversight for 10 years.

hackernews · djoldman · Jul 8, 23:37 · [Discussion](https://news.ycombinator.com/item?id=48838876)

**Background**: The right-to-repair movement advocates for consumers' ability to repair their own purchased products, which manufacturers often restrict via proprietary tools and software locks. John Deere has been a major target due to its practice of limiting access to repair manuals and parts.

**Discussion**: Commenters applaud activists like Louis Rossmann and note the fine is relatively small compared to John Deere's profits, questioning the enforcement's deterrent effect. Some express frustration that such basic freedoms require litigation, while others point out hypocrisy in the tech industry's defense of similar practices.

**Tags**: `#right-to-repair`, `#FTC`, `#John Deere`, `#consumer rights`, `#hardware`

---

<a id="item-6"></a>
## [OpenAI on removing noise from coding benchmarks](https://openai.com/index/separating-signal-from-noise-coding-evaluations/) ⭐️ 8.0/10

OpenAI published an analysis showing that many coding benchmark tasks contain flaws like misleading prompts or inadvertently testing instruction-following, and they manually cleaned over 800 tasks in SWE-bench to improve signal accuracy. This work highlights the fragility of current AI coding evaluations and pushes the field toward more rigorous, meaningful benchmarks, which is critical for accurately measuring model capabilities and avoiding inflated results. The analysis found that approximately 20% of tasks in SWE-bench had issues such as misleading prompts, tests that pass without correct code, or hidden pretraining data contamination; OpenAI used models themselves to help surface these problems.

hackernews · sk4rekr0w · Jul 8, 21:03 · [Discussion](https://news.ycombinator.com/item?id=48837396)

**Background**: Coding evaluation benchmarks like SWE-bench are used to assess how well AI models can solve real-world software engineering tasks. However, many benchmarks suffer from 'noise' such as ambiguous prompts or flawed test cases, which can lead to misleading performance scores. OpenAI's article demonstrates that as models improve, they can also help detect these flaws, enabling more reliable evaluations.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/separating-signal-from-noise-coding-evaluations/">Separating signal from noise in coding evaluations | OpenAI</a></li>

</ul>
</details>

**Discussion**: Community comments raised concerns about benchmark gaming, efficiency metrics, and task ambiguity. One user proposed a new benchmark measuring cost-effectiveness ($100 of API spend), while another noted that the small task count (under 800) makes human review feasible, criticizing original authors for not checking. There was also a suggestion that misleading prompts inadvertently test the model's ability to handle noise, which could be a benchmark itself.

**Tags**: `#AI`, `#Benchmarks`, `#Coding Evaluations`, `#OpenAI`, `#Software Engineering`

---

<a id="item-7"></a>
## [Mistral Unveils Robostral Navigate for Map-Less Robot Navigation](https://mistral.ai/news/robostral-navigate/) ⭐️ 8.0/10

Mistral AI has announced Robostral Navigate, an 8B-parameter model that enables robots to navigate complex indoor environments using only a single RGB camera, without requiring a pre-built map. The model follows natural language instructions like 'leave the lobby and enter the supply room.' This advancement significantly simplifies robot deployment in dynamic or unstructured environments, as it eliminates the need for costly mapping infrastructure. It opens up possibilities for hobbyist and commercial robotics, potentially accelerating adoption in warehouses, homes, and farms. Robostral Navigate is hardware-agnostic, designed to work with any robot platform, and currently appears to be a research demonstration rather than an openly available model. The system relies on a vision-based approach, similar to prior work like Stanford's PIGEON but indoors.

hackernews · ottomengis · Jul 8, 14:09 · [Discussion](https://news.ycombinator.com/item?id=48832212)

**Background**: Traditional robot navigation often requires a pre-built map (SLAM) or external beacons, failing when the robot is 'kidnapped' (i.e., moved to an unknown location without localization). Map-less navigation, in contrast, allows a robot to understand its surroundings from raw camera input and follow commands without prior knowledge of the space. This approach has been demonstrated outdoors but remains challenging indoors due to visual ambiguity.

<details><summary>References</summary>
<ul>
<li><a href="https://mistral.ai/news/robostral-navigate/">Robostral Navigate: single-camera AI navigation | Mistral AI</a></li>
<li><a href="https://news.ycombinator.com/item?id=48832212">Mistral's Robostral Navigate: a state of the art robotics navigation model</a></li>
<li><a href="https://www.reddit.com/r/AIGuild/comments/1ur9vyz/mistral_launched_robostral_navigate_an_8b_model/">Mistral launched Robostral Navigate, an 8B model for robot navigation</a></li>

</ul>
</details>

**Discussion**: The community is excited about the map-less capability, noting it solves the 'kidnapped robot' problem. Commenters express interest in hobbyist applications, but lament that the model is not openly available. Some draw parallels to Stanford's PIGEON and discuss potential privacy implications of such technology.

**Tags**: `#robotics`, `#navigation`, `#Mistral AI`, `#AI`, `#map-less navigation`

---

<a id="item-8"></a>
## [Microsoft releases Flint, a visualization language for AI agents](https://microsoft.github.io/flint-chart/#/) ⭐️ 8.0/10

Microsoft has released Flint, an open-source visualization intermediate language designed to improve the reliability and quality of charts generated by AI agents. Flint introduces a semantic-type-based specification and a layout optimization engine that produces high-quality charts from simple, high-level inputs. Flint addresses the fundamental trade-off between reliability and quality in AI-generated visualizations, making it easier for agents to produce publication-ready charts consistently. This could accelerate the adoption of AI agents in data analysis and reporting, providing a deterministic layer that improves output reliability. Flint is already powering Microsoft's Data Formulator project and is available as an open-source MCP (Model Context Protocol) server that can be plugged into agent applications. The language abstracts away low-level visual decisions like scales, axes, and layout, delegating them to a compiler-based optimization engine.

hackernews · chenglong-hn · Jul 8, 17:46 · [Discussion](https://news.ycombinator.com/item?id=48834924)

**Background**: Current visualization languages force AI agents to either use simple but low-quality specifications or complex, verbose ones that hurt reliability. Flint acts as an intermediate representation (IR) similar to a compiler IR, allowing agents to express high-level intent while the engine handles the visual details. This pattern of combining LLM generation with a deterministic compiler layer is emerging as a best practice in agentic systems.

**Discussion**: Commenters noted Flint follows an emerging pattern of combining LLMs with a deterministic compiler layer. Some questioned how Flint differs from Vega, a well-known visualization DSL, while others expressed skepticism about LLMs needing simpler specs, arguing they handle verbose code well but struggle with spatial composition. Overall, the discussion was substantive, with both praise and technical critique.

**Tags**: `#visualization`, `#AI agents`, `#Microsoft`, `#data visualization`, `#programming languages`

---

<a id="item-9"></a>
## [xAI Unveils Grok 4.5: Cost-Efficient but Controversial](https://x.ai/news/grok-4-5) ⭐️ 8.0/10

xAI has announced the release of Grok 4.5, a large language model that offers competitive performance at a significantly lower cost than competing models like GPT-4.5 and Opus 4.8, with pricing at $2 per million input tokens and $6 per million output tokens. The release of Grok 4.5 could intensify price competition in the AI model market, making advanced AI more accessible to businesses and developers. However, the model faces significant trust issues due to reported political bias and ethical concerns, which may limit its adoption in enterprise settings. According to community benchmarks, Grok 4.5 achieves roughly the performance level of Opus 4.7 while offering 4x better reasoning efficiency. The model was trained using trillions of tokens of Cursor data, capturing real-world developer interactions and software workflows.

hackernews · BoumTAC · Jul 8, 18:00 · [Discussion](https://news.ycombinator.com/item?id=48835111)

**Background**: Grok is a series of large language models developed by xAI, a company founded by Elon Musk. Grok 4.5 is the latest version, positioned as a cost-efficient alternative to models from OpenAI, Anthropic, and others. xAI has faced criticism over its handling of content moderation and political neutrality, which has fueled skepticism about the model's reliability.

**Discussion**: Commenters expressed strong distrust towards xAI, citing concerns about political bias and ethical practices, particularly regarding CSAM. Some praised the model's cost efficiency and benchmark performance, comparing it favorably to competitors. Others questioned the economic viability of training such costly models given the current market profitability challenges.

**Tags**: `#AI`, `#machine learning`, `#Grok`, `#xAI`, `#model release`

---

<a id="item-10"></a>
## [OpenAI Unveils GPT-Live Voice Mode with GPT-5.5 Delegation](https://openai.com/index/introducing-gpt-live/) ⭐️ 8.0/10

OpenAI has announced GPT-Live, a real-time voice mode that can delegate complex reasoning tasks to GPT-5.5 in the background, providing significantly improved response quality over previous voice models. This integration merges natural voice interaction with cutting-edge reasoning, making AI conversations more useful and lifelike, potentially increasing voice AI adoption while also sparking debate about human interaction replacement. The initial release is called GPT-Live-1. A bug was reported where the model would interrupt and laugh at unintended moments, and the feature currently lacks tool or connector integration, limiting its productivity use cases.

hackernews · logickkk1 · Jul 8, 17:03 · [Discussion](https://news.ycombinator.com/item?id=48834405)

**Background**: Previous AI voice modes were limited to older, less capable models due to latency constraints of real-time speech. GPT-Live overcomes this by delegating heavy reasoning to GPT-5.5 while maintaining low-latency voice flow, enabling more sophisticated conversations.

**Discussion**: Community reactions are mixed: some users praise the quality and naturalness (simonw reports an hour-long productive walk), while others express ethical concerns about replacing human relationships (jonstaab, overgard). A common request is for tool integration (artdigital), and an OpenAI employee (athyuttamre) clarifies the version as GPT-Live-1.

**Tags**: `#OpenAI`, `#voice mode`, `#AI product launch`, `#ethical concerns`, `#GPT-5`

---

<a id="item-11"></a>
## [sqlite-utils 4.0 Released with Schema Migrations](https://simonwillison.net/2026/Jul/7/sqlite-utils/#atom-everything) ⭐️ 8.0/10

sqlite-utils 4.0 has been released, introducing database schema migration support for the first time. This new feature makes sqlite-utils a more complete tool for managing SQLite databases, allowing users to evolve their database schemas programmatically. The migration system likely allows applying incremental changes to database schemas, similar to other migration frameworks.

rss · Simon Willison · Jul 7, 15:42

**Background**: sqlite-utils is a Python library and command-line tool for creating and manipulating SQLite databases. It is commonly used for data analysis and ETL workflows. The addition of schema migrations fills a long-standing gap in its feature set.

<details><summary>References</summary>
<ul>
<li><a href="https://sqlite-utils.datasette.io/">sqlite-utils</a></li>
<li><a href="https://github.com/simonw/sqlite-utils">simonw/sqlite-utils: Python CLI utility and library for ... - GitHub</a></li>

</ul>
</details>

**Tags**: `#sqlite`, `#python`, `#database`, `#migrations`

---

<a id="item-12"></a>
## [Huawei 5G Flagship Returns Overseas with 1100 Mbps Speed](https://finance.sina.com.cn/tech/roll/2026-07-08/doc-inihapna8035781.shtml) ⭐️ 8.0/10

Huawei's Pura 90 Pro Max international version has been tested to achieve peak 5G download speeds exceeding 1100 Mbps, confirming the return of Huawei 5G flagship smartphones to overseas markets after seven years of US sanctions. This milestone demonstrates Huawei's ability to overcome technology restrictions and re-enter the global 5G smartphone market, potentially intensifying competition in the premium segment and affecting supply chain dynamics. The international version natively supports 5G, with the status bar displaying the 5G logo, and achieves over 1100 Mbps peak download speeds in real-world tests. Earlier this year, Huawei's flagship devices upgraded to HarmonyOS 6.0.0.125, implementing 5A communication technology as a foundation for this international launch.

telegram · zaihuapd · Jul 8, 12:17

**Background**: Since 2019, US sanctions prevented Huawei from selling 5G smartphones globally. In 2023, the Mate 60 series broke through some technology restrictions, and with the HarmonyOS 6.0.0.125 update, Huawei introduced 5A communication technology. The Pura 90 Pro Max now brings 5G capabilities to international markets, marking a significant turnaround.

<details><summary>References</summary>
<ul>
<li><a href="https://betawiki.net/wiki/HarmonyOS_6">HarmonyOS 6 - BetaWiki</a></li>
<li><a href="https://www.reddit.com/r/Huawei/comments/1q8v34v/celia_keyboard_hits_the_primetime_letsgoooo_hos/">Celia Keyboard Hits the Prime-Time, Letsgoooo! (HOS 6.0.0.125) - Reddit</a></li>

</ul>
</details>

**Tags**: `#Huawei`, `#5G`, `#smartphones`, `#telecommunications`, `#sanctions`

---

<a id="item-13"></a>
## [Cloudflare and OpenAI Pilot Global Network Data for AI Search](https://36kr.com/newsflashes/3886946347694593) ⭐️ 8.0/10

Cloudflare and OpenAI announced a pilot research project on July 8 to use real-time website insights from Cloudflare's global network to help AI search engines more efficiently discover and index web content. This collaboration could significantly improve the accuracy and timeliness of AI answers by incorporating real-time web signals such as content freshness and traffic quality, setting a new standard for AI search indexing. The pilot leverages Cloudflare's visibility into actual page changes and traffic patterns to optimize crawling efficiency, but it is still experimental with no production deployment announced.

telegram · zaihuapd · Jul 8, 15:27

**Background**: AI search engines rely on web crawling to index content, but traditional crawling can be inefficient and miss updates. Cloudflare's global network processes a large portion of web traffic, providing unique real-time data on site changes and popularity. This data could help AI systems prioritize fresh, high-quality pages.

**Tags**: `#Cloudflare`, `#OpenAI`, `#AI Search`, `#Web Indexing`, `#Data Optimization`

---

<a id="item-14"></a>
## [Smartphone app identification via EM signals achieves 99.07% accuracy](https://www.scmp.com/news/china/science/article/3359688/chinese-researchers-find-peephole-any-smartphone-its-leaked-radio-signal) ⭐️ 8.0/10

Researchers developed a non-contact technique to analyze low-frequency electromagnetic signals leaked from smartphones, enabling identification of running apps and actions with up to 99.07% accuracy. The method works even when the device is offline, in airplane mode, encrypted, or locked. This side-channel attack poses significant privacy and security risks as it can infer app usage patterns without any direct access to the device. It highlights the vulnerability of electromagnetic emissions as an information leak vector. Tests were conducted on iPhone 15 Pro, Xiaomi 15 Pro, and OPPO Reno 13, covering apps like Douyin, WeChat video calls, Baidu Maps, SMS, browser, camera, and cloud storage. The highest accuracy reached 99.07%.

telegram · zaihuapd · Jul 8, 16:05

**Background**: Smartphones emit low-frequency electromagnetic signals during operation as a byproduct of internal circuit activity. While often unintended, these signals can be captured remotely by specialized equipment and analyzed to infer user activity. This technique, known as a side-channel attack, exploits physical emissions to extract information that would otherwise be protected by software security measures.

**Tags**: `#security`, `#side-channel`, `#smartphone`, `#privacy`, `#forensics`

---