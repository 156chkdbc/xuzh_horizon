---
layout: default
title: "Horizon Summary: 2026-07-17 (EN)"
date: 2026-07-17
lang: en
---

> From 37 items, 15 important content pieces were selected

---

1. [Firefox Compiled to WebAssembly Runs Inside Another Browser](#item-1) ⭐️ 9.0/10
2. [Kimi K3: 2.8 Trillion Parameter Open-Weight Model](#item-2) ⭐️ 9.0/10
3. [Inkling: 975B Open-Weights MoE Multimodal Model Released](#item-3) ⭐️ 9.0/10
4. [Linus Torvalds Declares Linux Not Anti-AI](#item-4) ⭐️ 9.0/10
5. [Claude web_fetch tool vulnerability enables data exfiltration via nested links](#item-5) ⭐️ 9.0/10
6. [LM Studio launches Bionic, an AI agent for open models](#item-6) ⭐️ 8.0/10
7. [Interactive Linear Algebra Book Enhances Learning with Immersive Figures](#item-7) ⭐️ 8.0/10
8. [Roc Compiler Rewrite from Rust to Zig Reaches Feature Parity](#item-8) ⭐️ 8.0/10
9. [GOES-19 Weather Satellite Enters Safe Hold](#item-9) ⭐️ 8.0/10
10. [GPT-5.6 Codex Bug Can Delete Files Without Sandboxing](#item-10) ⭐️ 8.0/10
11. [xAI's Grok CLI privacy scandal leads to open-sourcing](#item-11) ⭐️ 8.0/10
12. [US ITC Launches 337 DRAM Probe; Samsung, Google, Nvidia Named](#item-12) ⭐️ 8.0/10
13. [Japan to Buy 27,500 Nvidia Rubin Chips for Robot AI](#item-13) ⭐️ 8.0/10
14. [TSMC invests additional $100B in Arizona, Q2 profit up 77% to record](#item-14) ⭐️ 8.0/10
15. [Truth Social to Sell Fast Access to Trump Posts to Wall Street](#item-15) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Firefox Compiled to WebAssembly Runs Inside Another Browser](https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/#atom-everything) ⭐️ 9.0/10

Puter has compiled the full Firefox browser to WebAssembly, allowing it to run inside another browser window. The demo, which loaded a 233MB gecko.wasm file, uses a WebSocket proxy (Wisp protocol) to handle network traffic. This demonstrates a paradigm shift in cross-platform browser execution, showing that a full-featured browser can be sandboxed and run within any modern browser. It could enable new use cases for isolated browsing, testing, and legacy compatibility without native installation. The project used an estimated $25,000 worth of Claude Opus and Fable tokens, but cost less due to a subscription plan. Traffic is routed through Puter's servers via the Wisp protocol, and the team claims end-to-end encryption is supported.

rss · Simon Willison · Jul 16, 23:34

**Background**: WebAssembly (WASM) is a binary instruction format that allows code written in languages like C++ to run in web browsers at near-native speed. Compiling an entire browser like Firefox to WASM is extremely challenging because browsers are complex systems that manage network, graphics, and memory. Puter is a cloud-based desktop environment that runs in a browser, making it a natural platform for hosting such a demo.

<details><summary>References</summary>
<ul>
<li><a href="https://puter.com/">Puter</a></li>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/wisp-protocol: Wisp is a low-overhead, easy to implement protocol for proxying multiple TCP/UDP sockets over a single websocket. · GitHub</a></li>

</ul>
</details>

**Tags**: `#WebAssembly`, `#Firefox`, `#Browser`, `#Compilation`, `#Cross-platform`

---

<a id="item-2"></a>
## [Kimi K3: 2.8 Trillion Parameter Open-Weight Model](https://simonwillison.net/2026/Jul/16/kimi-k3/#atom-everything) ⭐️ 9.0/10

Moonshot AI announced Kimi K3, a 2.8 trillion parameter open-weight model that outperforms GPT-5.5 and Claude Opus 4.8 on several benchmarks. It is available via API and website, with open weights promised by July 27, 2026. This marks a significant milestone for open-weight AI, as Kimi K3 is the largest open-weight model at 2.8 trillion parameters, challenging proprietary leaders. It shows Chinese AI labs are pushing the frontier of open models, potentially making high-performance AI more accessible. The model uses 1 million token context, priced at $3/M input and $15/M output tokens, making it the most expensive Chinese open-weight model. It also tops the Arena.ai Frontend Code leaderboard, surpassing Claude Fable 5.

rss · Simon Willison · Jul 16, 20:19

**Background**: Open-weight models allow users to download and run the model parameters on their own infrastructure, but do not necessarily include training data or code. While dense models have billions of parameters, Kimi K3 likely uses a mixture-of-experts architecture to keep inference costs manageable despite its 2.8T total parameters. The '3 trillion parameter class' refers to models around the 3T mark, with DeepSeek-V4 Pro at 1.6T being the previous largest open-weight model.

<details><summary>References</summary>
<ul>
<li><a href="https://d-central.tech/mining-glossary/open-weight-model/">Open - Weight Model Meaning | Bitcoin Mining Glossary</a></li>
<li><a href="https://macaron.im/blog/deepseek-v4-moe-1-trillion">DeepSeek-V4 MoE: The 1- Trillion Parameter Breakthrough - Macaron</a></li>
<li><a href="https://www.buildfastwithai.com/blogs/qwen3-max-preview-trillion-parameter">Qwen 3 -Max-Preview: Alibaba’s Trillion - Parameter Breakthrough with...</a></li>

</ul>
</details>

**Discussion**: Commenters note the high cost ($0.94 per task) compared to other open-weight models, and discuss whether Chinese labs are commoditizing AI intelligence. Some express skepticism about the open-weight label and the economic viability of such large models.

**Tags**: `#AI`, `#large language models`, `#open-source`, `#model release`, `#benchmarks`

---

<a id="item-3"></a>
## [Inkling: 975B Open-Weights MoE Multimodal Model Released](https://simonwillison.net/2026/Jul/16/inkling/#atom-everything) ⭐️ 9.0/10

Thinking Machines Lab, led by Mira Murati, released Inkling, a 975 billion parameter Mixture-of-Experts multimodal model with 41B active parameters, under the Apache-2.0 license. It is trained on 45 trillion tokens of text, images, audio, and video. This release strengthens the US open-weights ecosystem, providing a competitive alternative to models from China and NVIDIA/Gemma. It offers a strong base for fine-tuning, potentially democratizing access to advanced multimodal AI. The model card is notably short, with minimal training data documentation. Inkling is not a frontier model but intended as a strong base model for customization via their Tinker training platform; a smaller 276B (12B active) variant called Inkling-Small is promised later.

rss · Simon Willison · Jul 16, 15:35

**Background**: Mixture-of-Experts (MoE) architecture uses multiple specialized subnetworks ('experts') with a routing mechanism to activate only a subset per input, enabling larger total parameters with efficient inference. Open-weights models release trained parameters publicly, allowing download, fine-tuning, and deployment, but often with usage restrictions unlike fully open-source.

<details><summary>References</summary>
<ul>
<li><a href="https://datanorth.ai/blog/what-is-mixture-of-experts-moe-and-why-does-it-matter">What is mixture of experts (MoE) and why does it matter?</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>

</ul>
</details>

**Tags**: `#open-weights`, `#multimodal`, `#Mixture-of-Experts`, `#AI model`, `#Thinking Machines Lab`

---

<a id="item-4"></a>
## [Linus Torvalds Declares Linux Not Anti-AI](https://simonwillison.net/2026/Jul/16/linus-torvalds/#atom-everything) ⭐️ 9.0/10

Linus Torvalds, the creator and top maintainer of the Linux kernel, explicitly stated on the Linux Media Mailing List that the Linux project is not anti-AI, considering AI a useful tool and telling dissenters they can fork the project or walk away. This statement from the highest authority in the Linux kernel sets a clear direction for the entire open-source ecosystem, potentially encouraging broader adoption of AI tools in development and reducing resistance within the community. Torvalds acknowledged that AI's usefulness was not clear a year ago but is now unquestionable, though he noted economic questions remain. His remarks were made in response to unspecified opposition to AI use in the kernel.

rss · Simon Willison · Jul 16, 13:26

**Background**: Linus Torvalds is the creator and longtime maintainer of the Linux kernel, which powers servers, embedded systems, and Android devices. His statements carry immense weight in the open-source community. The debate around AI in open-source projects has been contentious, with some developers opposing AI-generated code due to quality, licensing, and ethical concerns.

**Tags**: `#Linux`, `#AI`, `#Open Source`, `#Kernel Development`, `#Linus Torvalds`

---

<a id="item-5"></a>
## [Claude web_fetch tool vulnerability enables data exfiltration via nested links](https://simonwillison.net/2026/Jul/15/claude-web-fetch-exfiltration/#atom-everything) ⭐️ 9.0/10

A security researcher discovered that Anthropic's Claude web_fetch tool could be tricked into exfiltrating sensitive user data by following nested links from a malicious website, bypassing intended restrictions. This vulnerability demonstrates a critical flaw in AI agent design where safeguards against data exfiltration can be circumvented through social engineering combined with technical loopholes, highlighting ongoing risks in LLM-powered tools. The attacker created a honeypot page that displayed a fake Cloudflare authentication prompt, tricking the AI into navigating through alphabetical subpages to construct a user profile URL that exfiltrated name, city, and employer. Anthropic had already internally identified the issue and closed the loophole by preventing web_fetch from following links within fetched content.

rss · Simon Willison · Jul 15, 14:21

**Background**: Claude's web_fetch tool was designed with restrictions: it can only visit exact URLs provided by the user or returned from its web_search tool, preventing direct exfiltration attacks. However, it could follow links embedded in fetched pages. This vulnerability is an example of the 'lethal trifecta' attack pattern where an AI agent has access to private data, processes untrusted content, and can communicate externally, enabling prompt injection to steal information.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/">The lethal trifecta for AI agents: private data, untrusted content, and external communication</a></li>
<li><a href="https://simonwillison.net/2025/Sep/10/claude-web-fetch-tool/">Claude API: Web fetch tool</a></li>

</ul>
</details>

**Tags**: `#AI security`, `#data exfiltration`, `#Claude`, `#prompt injection`, `#LLM vulnerabilities`

---

<a id="item-6"></a>
## [LM Studio launches Bionic, an AI agent for open models](https://lmstudio.ai/blog/introducing-lm-studio-bionic) ⭐️ 8.0/10

LM Studio has launched Bionic, an agentic workflow tool that allows users to run AI agents with local and hosted open-source models. It supports coding and document creation with features like automatic checkpointing. This release brings agentic AI capabilities to local and open-source models, making advanced workflows accessible to a broader audience without relying solely on cloud APIs. It positions LM Studio as a key platform for privacy-conscious enterprises and developers wanting to control costs and data. Bionic supports models like Qwen3.6 35B and offers a Code project for coding and a Work project with automatic checkpointing for each agent change. The founder also offered free credits to try it with models like GLM 5.2 and Kimi K2.6.

hackernews · minimaxir · Jul 16, 20:18 · [Discussion](https://news.ycombinator.com/item?id=48939662)

**Background**: LM Studio is a popular beginner-friendly tool for running local large language models (LLMs) on personal computers without requiring command-line expertise. Agentic workflows involve AI agents that autonomously plan and execute tasks with minimal human intervention, often using external tools and APIs.

<details><summary>References</summary>
<ul>
<li><a href="https://lmstudio.ai/download">Download LM Studio - Mac, Linux, Windows</a></li>
<li><a href="https://www.ibm.com/think/topics/agentic-workflows">What are Agentic Workflows? | IBM</a></li>

</ul>
</details>

**Discussion**: Early users gave positive first impressions, with one noting smooth performance using Qwen3.6 35B and a familiar UI similar to Codex. The founder engaged directly, offering free credits for specific models. Some expressed concerns about a business model shift toward cloud services, while others questioned the differentiation from existing agent harnesses.

**Tags**: `#LM Studio`, `#AI agent`, `#local LLMs`, `#open-source models`, `#coding assistant`

---

<a id="item-7"></a>
## [Interactive Linear Algebra Book Enhances Learning with Immersive Figures](https://immersivemath.com/ila/) ⭐️ 8.0/10

A free online linear algebra book, published in 2015, features interactive 3D figures that allow readers to manipulate and explore mathematical concepts directly in the browser. This book demonstrates how interactivity can make abstract mathematical concepts more intuitive, potentially improving learning outcomes and inspiring similar approaches in other STEM fields. The book covers standard linear algebra topics such as vectors, matrices, eigenvalues, and linear transformations, with each interactive figure accompanied by explanatory text and tooltips.

hackernews · srean · Jul 16, 15:32 · [Discussion](https://news.ycombinator.com/item?id=48935951)

**Background**: Linear algebra is a foundational branch of mathematics used in computer graphics, machine learning, and engineering. Traditional textbooks present static diagrams, but interactive visualizations allow students to rotate, zoom, and change parameters, enhancing spatial understanding.

**Discussion**: The community highly praises the book, with users expressing nostalgia for such resources during their own studies and suggesting extensions to statistics, probability, and robotics. Some commenters note that advances in AI and LLMs make creating similar interactive content easier, potentially leading to a new wave of educational tools.

**Tags**: `#linear algebra`, `#education`, `#interactive`, `#math`, `#visualization`

---

<a id="item-8"></a>
## [Roc Compiler Rewrite from Rust to Zig Reaches Feature Parity](https://rtfeldman.com/rust-to-zig) ⭐️ 8.0/10

The Roc compiler team announced that their 1.5-year rewrite of the compiler from Rust to Zig has achieved feature parity with the original Rust-based compiler, involving around 300,000 lines of code. This milestone demonstrates the viability of migrating a large-scale systems project from Rust to Zig, highlighting Zig's strengths in faster compilation, simpler cross-compilation, and more flexible unsafe code handling for compiler development. The post explains that compilers often need memory-unsafe operations for features like hot binary patching, which influenced the switch. Zig's ReleaseSafe mode provides runtime checks for use-after-free errors, though some commenters questioned its effectiveness.

hackernews · jorangreef · Jul 16, 11:39 · [Discussion](https://news.ycombinator.com/item?id=48933149)

**Background**: Roc is a functional programming language designed for speed and friendliness. Its compiler was originally written in Rust, but the team decided to rewrite it in Zig to take advantage of Zig's fast compilation times, excellent cross-compilation support, and more straightforward approach to unsafe code. The rewrite took 1.5 years and recently reached feature parity with the original compiler.

<details><summary>References</summary>
<ul>
<li><a href="https://www.roc-lang.org/">The Roc Programming Language</a></li>
<li><a href="https://github.com/roc-lang/roc">GitHub - roc-lang/roc: A fast, friendly, functional language. The Roc Programming Language roc/docs/mini-tutorial-new-compiler.md at main · roc-lang/roc ROCm Software - AMD The Complete Roc Guide: From Zero to Expert - kodikra How Our Rust-to-Zig Rewrite is Going</a></li>

</ul>
</details>

**Discussion**: steveklabnik challenged the claim that compilers inherently require memory-unsafe operations, arguing only specific features like binary patching need unsafe code. landr0id questioned Zig's runtime use-after-free detection, while onlyrealcuzzo praised Zig's incremental builds but expressed safety concerns.

**Tags**: `#Rust`, `#Zig`, `#compilers`, `#memory safety`, `#systems programming`

---

<a id="item-9"></a>
## [GOES-19 Weather Satellite Enters Safe Hold](https://www.spaceweather.gov/news/goes-19-safe-hold) ⭐️ 8.0/10

The GOES-19 weather satellite entered safe hold mode on July 15, 2026, but engineers have already restored DCS and SAR services and are working to resume ABI imaging by 1900Z. GOES-19 is the primary satellite for tracking Atlantic hurricanes and Gulf Coast weather; its outage, even brief, can impact real-time forecasting and public safety during hurricane season. The recovery order is ABI, GLM, SUVI, and CCOR instruments, with image navigation possibly degraded for the first hour after restoration. The satellite returned to service in under 24 hours.

hackernews · yabones · Jul 16, 13:30 · [Discussion](https://news.ycombinator.com/item?id=48934286)

**Background**: Safe hold (or safe mode) is a spacecraft operating state where non-essential systems are shut down and only critical functions like thermal control and communication remain active. GOES-19 is the fourth and final satellite in NOAA's GOES-R series, providing continuous weather monitoring from geostationary orbit.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Safe_mode_in_spacecraft">Safe mode in spacecraft - Wikipedia</a></li>
<li><a href="https://www.nola.com/news/hurricane/weather-satellite-goes-19-out/article_75a9d7be-1e36-4bf1-b55f-26ff9a369157.html">GOES 19 satellite used to track Gulf hurricanes is offline | Hurricane Center | nola.com</a></li>

</ul>
</details>

**Discussion**: A former GOES engineer noted that anomalies are common across the GOES fleet, citing past issues like GOES-17's heat pipe anomaly and GOES-13's fuel tank problem. Commenters also indicated that restoration was progressing quickly and that the outage highlighted reliance on satellite data for forecasting.

**Tags**: `#weather satellite`, `#GOES-19`, `#safe hold mode`, `#NOAA`, `#hurricane tracking`

---

<a id="item-10"></a>
## [GPT-5.6 Codex Bug Can Delete Files Without Sandboxing](https://simonwillison.net/2026/Jul/16/bad-codex-bug/#atom-everything) ⭐️ 8.0/10

A bug in OpenAI's GPT-5.6 Codex agent can accidentally delete files when full access mode is enabled without sandboxing or auto-review, caused by the model erroneously deleting the $HOME directory after attempting to override the $HOME environment variable. This bug poses a significant data loss risk for developers using Codex in production environments, highlighting the critical need for sandboxing and review safeguards when deploying AI coding agents autonomously. The bug occurs specifically when Codex runs with full access mode, no sandboxing, no auto-review, and the model attempts to set a temporary directory via $HOME override but mistakenly deletes $HOME instead.

rss · Simon Willison · Jul 16, 17:45

**Background**: OpenAI Codex is an AI coding agent for software engineering tasks like writing code and fixing bugs, released in April 2025 as Codex CLI. It can be used with varying levels of system access; 'full access mode' without sandboxing gives the agent unrestricted file system permissions, which can lead to destructive actions if the model errs.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_Codex_(AI_agent)">OpenAI Codex (AI agent) - Wikipedia</a></li>
<li><a href="https://www.docker.com/products/docker-sandboxes/">Sandboxes for Coding Agents - Docker</a></li>

</ul>
</details>

**Tags**: `#codex`, `#coding-agents`, `#generative-ai`, `#ai-safety`, `#security`

---

<a id="item-11"></a>
## [xAI's Grok CLI privacy scandal leads to open-sourcing](https://simonwillison.net/2026/Jul/15/grok-build/#atom-everything) ⭐️ 8.0/10

xAI's Grok CLI tool was found to upload entire user directories to the cloud, including SSH keys and password databases. In response, xAI deleted all previously uploaded user data, disabled the feature, and released the Grok Build codebase under an Apache 2.0 license. This incident severely damages trust in AI coding tools, especially those integrated into developer environments. The reactive open-sourcing may help rebuild confidence, but it underscores critical privacy risks in cloud-based AI agents that have access to local files. The Grok Build codebase contains 844,530 lines of Rust code (only 3% vendored) and was released in a single commit, so no development history is visible. It includes a self-contained Mermaid diagram terminal renderer and tool implementations inspired by Codex and OpenCode.

rss · Simon Willison · Jul 15, 23:59

**Background**: The Grok CLI is an AI-powered coding agent that runs in the terminal, similar to tools like GitHub Copilot. By default, it uploaded the current directory contents to xAI's servers, which led to users inadvertently exposing sensitive files. The community backlash prompted xAI to take immediate action.

<details><summary>References</summary>
<ul>
<li><a href="https://x.ai/cli">Grok Build | SpaceXAI</a></li>
<li><a href="https://lalatenduswain.medium.com/automate-your-terminal-with-grok-cli-a-developers-guide-to-xai-s-ai-powered-tool-eb8e2b0460bf">Automate Your Terminal with Grok CLI : A Developer’s Guide... | Medium</a></li>

</ul>
</details>

**Discussion**: User reports on social media described finding SSH keys, password databases, and personal documents being uploaded. The overall sentiment is outrage over the privacy violation, with many criticizing the lack of consent and transparency. Some appreciate the open-sourcing but remain skeptical about future trust.

**Tags**: `#privacy`, `#security`, `#open-source`, `#xAI`, `#CLI`

---

<a id="item-12"></a>
## [US ITC Launches 337 DRAM Probe; Samsung, Google, Nvidia Named](https://www.cls.cn/detail/2428105) ⭐️ 8.0/10

The U.S. International Trade Commission (ITC) voted on July 15 to initiate Section 337 investigation No. 337-TA-1511 targeting certain DRAM devices, downstream products, and components, based on a patent infringement complaint filed by Netlist. Respondents include Samsung Electronics, Google, Nvidia, Broadcom, and Super Micro Computer. The investigation covers DDR5 DIMMs and High Bandwidth Memory (HBM) used in AI servers and data centers, potentially disrupting supply chains for major tech companies. If the ITC rules in favor of Netlist, imports of the infringing products could be blocked, affecting cloud services and AI computing costs. The complaint specifically mentions DDR5 DIMM modules, HBM stacks, and servers, computing, and storage systems incorporating these memories. The investigation is in its early stages; a final determination may take 12-18 months, and immediate price impacts on consumer electronics are unlikely.

telegram · zaihuapd · Jul 16, 08:34

**Background**: Section 337 of the Tariff Act of 1930 empowers the USITC to investigate unfair trade practices, including patent infringement, in imported goods. If a violation is found, the ITC can issue exclusion orders barring entry of the products into the U.S. DDR5 DIMMs are the latest generation of dual in-line memory modules, while HBM is a 3D-stacked DRAM architecture offering extremely high bandwidth for AI and HPC workloads. Netlist is a memory technology company that has previously litigated patent cases against major DRAM manufacturers.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DDR5_SDRAM">DDR5 SDRAM - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://www.mti-worldwide.com/current-events-worldwide-logistics-blog/usitc-institutes-section-337-investigation-of-certain-vaporizer-devices-cartridges-used-therewith-and-components-thereof">USITC Institutes section 337 investigation of certain...</a></li>

</ul>
</details>

**Tags**: `#DRAM`, `#专利调查`, `#供应链`, `#半导体`, `#美国ITC`

---

<a id="item-13"></a>
## [Japan to Buy 27,500 Nvidia Rubin Chips for Robot AI](https://www.bloomberg.com/news/articles/2026-07-16/japan-to-buy-nvidia-rubin-chips-to-build-sovereign-ai-for-robots) ⭐️ 8.0/10

Japan announced a plan to purchase 27,500 Nvidia Rubin chips to build a large-scale data center, led by newly formed company Noetra, for developing sovereign AI models tailored to robotics, with a government subsidy of 387.3 billion yen (about $2.4 billion). This project aims to reduce Japan's dependence on foreign AI technology and capture over 30% of the global robot market by 2040, making it a significant move in the geopolitical competition for AI sovereignty. Noetra aims to release the first AI model by March of next year and a robot-specific version within a few years. The consortium includes SoftBank, Toyota-backed Preferred Networks, and NEC.

telegram · zaihuapd · Jul 16, 10:59

**Background**: Nvidia Rubin is a next-generation GPU microarchitecture named after astrophysicist Vera Rubin, announced in 2024. 'Sovereign AI' refers to national efforts to develop independent AI capabilities, including infrastructure, data, and models, to reduce reliance on foreign providers.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Rubin_(microarchitecture)">Rubin (microarchitecture) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Sovereign_AI">Sovereign AI</a></li>

</ul>
</details>

**Tags**: `#nvidia`, `#rubin`, `#robotics`, `#sovereign AI`, `#japan`

---

<a id="item-14"></a>
## [TSMC invests additional $100B in Arizona, Q2 profit up 77% to record](https://www.reuters.com/world/asia-pacific/tsmcs-second-quarter-profit-seen-hitting-record-ai-boom-2026-07-15/) ⭐️ 8.0/10

TSMC announced an additional $100 billion investment in Arizona for new fabs, bringing total US investment to $165 billion, and reported a Q2 net profit surge of 77% to a record NT$706.6 billion (approximately $22 billion), driven by AI demand. This underscores TSMC's strategic expansion to diversify manufacturing beyond Taiwan and its central role in the AI boom, with record profits signaling sustained strong demand from AI chips. TSMC raised its 2026 capital expenditure forecast to $60-64 billion and expects full-year dollar revenue to grow slightly over 40%. In Arizona, there are currently eight fabs under construction or planned, with potential for four more.

telegram · zaihuapd · Jul 16, 12:29

**Background**: TSMC is the world's largest contract chipmaker, crucial for producing advanced chips for companies like Apple and Nvidia. The firm has been expanding in the US, partly due to geopolitical tensions with China. The AI boom has dramatically increased demand for its cutting-edge semiconductor manufacturing services.

**Tags**: `#TSMC`, `#semiconductor`, `#AI`, `#investment`, `#profit`

---

<a id="item-15"></a>
## [Truth Social to Sell Fast Access to Trump Posts to Wall Street](https://www.cnn.com/2026/07/16/business/truth-social-data-wall-street) ⭐️ 8.0/10

Trump Media & Technology Group (TMTG) announced on July 16, 2026, that it will launch Truth API from August 1, providing institutional clients with millisecond-speed access to real-time posts from the top 10 accounts on Truth Social, including Donald Trump's. The service is explicitly marketed to high-frequency algorithmic traders seeking an information edge in financial markets. This move raises significant ethical and market integrity concerns, as it monetizes presidential social media posts for direct financial gain by high-speed traders, potentially allowing them to front-run market reactions to Trump's policy announcements. It also blurs the lines between public communication and private business interests, especially given Trump's history of using Truth Social to promote stocks he invested in. The API provides data in milliseconds, targeting high-frequency algorithmic trading strategies that rely on speed. TMTG has not disclosed specific pricing. Trump's Truth Social account has become a primary channel for announcing policy decisions on tariffs, Iran, and the Strait of Hormuz, which have previously caused sharp volatility in stock and oil markets.

telegram · zaihuapd · Jul 17, 01:02

**Background**: Algorithmic trading uses computer programs to execute trades automatically based on pre-defined rules, often leveraging speed and data to outperform humans. High-frequency trading (HFT) is a subset that requires extremely low latency to profit from tiny price movements. Truth Social was launched after Trump's ban from mainstream platforms, and it has become his primary social media outlet, with his posts frequently moving markets. The sale of real-time data directly to traders represents a novel and controversial revenue stream for a social platform tied to a political figure.

<details><summary>References</summary>
<ul>
<li><a href="https://marketchameleon.com/articles/b/2026/7/16/trump-media-launches-truth-api-institutional-market-impact">Trump Media Unveils Truth API: Real-Time Access to ...</a></li>
<li><a href="https://www.cnbc.com/2026/07/16/trump-truth-social-wall-street-traders-api.html">Truth Social launches service to give Wall Street traders an ...</a></li>

</ul>
</details>

**Tags**: `#Truth Social`, `#data API`, `#algorithmic trading`, `#finance`, `#ethics`

---