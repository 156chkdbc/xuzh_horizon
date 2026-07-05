---
layout: default
title: "Horizon Summary: 2026-07-05 (EN)"
date: 2026-07-05
lang: en
---

> From 54 items, 9 important content pieces were selected

---

1. [Prompt Injection Leaks YouTube Creators' Private Videos](#item-1) ⭐️ 9.0/10
2. [Session/Cache Leakage Risk in LLM Infrastructure Reported](#item-2) ⭐️ 9.0/10
3. [GPT-5.5 Codex reasoning-token clustering degrades performance](#item-3) ⭐️ 8.0/10
4. [Anna's Archive Offers $200K Bounty for Google Books Scans](#item-4) ⭐️ 8.0/10
5. [Building a World Map with Only 500 Bytes Using Deflate and JavaScript](#item-5) ⭐️ 8.0/10
6. [Newer Claude Models Show Worse Tool Call Accuracy](#item-6) ⭐️ 8.0/10
7. [Open Source AI Gap Map Launched by Current AI](#item-7) ⭐️ 8.0/10
8. [Tencent Atuin AI beats Mythos on CyberGym at 0.1% cost](#item-8) ⭐️ 8.0/10
9. [Huawei Unveils 'Tao's Law' Proposing Time Scaling for Chips](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Prompt Injection Leaks YouTube Creators' Private Videos](https://javoriuski.com/post/youtube) ⭐️ 9.0/10

A security researcher discovered that YouTube's AI-powered comment reply feature is vulnerable to prompt injection, allowing attackers to leak metadata of creators' private and unlisted videos. This vulnerability exposes private video metadata—including titles—that should remain confidential, affecting millions of creators who rely on YouTube's AI features for engagement. It highlights the growing risk of prompt injection attacks in widely deployed AI systems. The attack works when a creator clicks a suggested AI reply prompt in YouTube Studio; the attacker's malicious comment causes the AI to include private video titles in its response. The researcher demonstrated that the injected prompt can force the model to output specific text, such as a phishing link, along with the leaked data.

hackernews · javxfps · Jul 4, 16:45 · [Discussion](https://news.ycombinator.com/item?id=48786781)

**Background**: Prompt injection is a security vulnerability where an attacker embeds instructions within user input that override an AI model's original system prompt. Large language models like those used by YouTube struggle to distinguish between trusted instructions and adversarial user-generated content. The affected feature uses AI to auto-generate comment replies for creators, but it processes user comments without adequate isolation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.mdpi.com/2078-2489/17/1/54">Prompt Injection Attacks in Large Language Models and AI Agent ... - MDPI</a></li>
<li><a href="https://arxiv.org/html/2511.15759v1">Securing AI Agents Against Prompt Injection Attacks:</a></li>

</ul>
</details>

**Discussion**: A former Google engineer explained that the slow fix may stem from the implementing engineer having already moved on, making the bug low priority. Another commenter expressed frustration that YouTube does not treat prompt injection as a bug. A user who attempted to reproduce the attack found it partially worked, with the injected text appearing in the AI's response.

**Tags**: `#security`, `#prompt injection`, `#YouTube`, `#AI`, `#vulnerability`

---

<a id="item-2"></a>
## [Session/Cache Leakage Risk in LLM Infrastructure Reported](https://github.com/anthropics/claude-code/issues/74066) ⭐️ 9.0/10

Users report potential session or cache leakage in Claude Code and other LLM services, where responses from one user's session appear to be swapped with another's, including instances involving GPT and Gemini models. A Claude Code team member stated they are investigating but currently believe it is a hallucination. If confirmed, this would indicate a serious security vulnerability in multi-tenant LLM infrastructure, potentially leaking sensitive information across user sessions. The issue highlights the need for robust session isolation and cache security in AI platforms. One user detailed incidents across multiple providers, including a postmortem where an API gateway mishandled HTTP 100 status codes, causing an off-by-one error. Academic research has identified key collision attacks on LLM semantic caching as a known vulnerability.

hackernews · chatmasta · Jul 4, 14:03 · [Discussion](https://news.ycombinator.com/item?id=48785485)

**Background**: Session leakage occurs when data from one user's interaction with an LLM is incorrectly served to another user, often due to misconfigured caching layers or shared memory in multi-tenant architectures. Semantic caching in LLMs aims to improve response times by reusing outputs for similar queries, but this locality creates collision risks. Cache poisoning and cross-session leaks are emerging security concerns in AI infrastructure.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/anthropics/claude-code/issues/74066">[Bug] Potential session/cache leakage between workspace ... - GitHub</a></li>
<li><a href="https://www.promptzone.com/priya_sharma_3cccef14/claude-workspace-leakage-risk-discussed-on-hn-3m2c">Claude Workspace Leakage Risk Discussed on HN - PromptZone</a></li>
<li><a href="https://www.giskard.ai/knowledge/cross-session-leak-when-your-ai-assistant-becomes-a-data-breach">Cross Session Leak: LLM security vulnerability & detection guide</a></li>

</ul>
</details>

**Discussion**: Community responses are divided: some users report similar cross-session anomalies with other providers like Gemini, while others suspect hallucination rather than infrastructure flaws. A Claude Code team member acknowledged the report and stated they are investigating but leaning toward hallucination. The discussion includes technical analysis of possible API gateway mishandling.

**Tags**: `#security`, `#LLM`, `#privacy`, `#session-leakage`, `#cache-collision`

---

<a id="item-3"></a>
## [GPT-5.5 Codex reasoning-token clustering degrades performance](https://github.com/openai/codex/issues/30364) ⭐️ 8.0/10

Users report that GPT-5.5 Codex exhibits reasoning-token clustering, where responses cluster at fixed token counts (e.g., 516) leading to incorrect results, while correct responses use 6000-8000 tokens. This mirrors a previous regression in Claude Code. This highlights a reproducible regression in a widely-used AI coding tool, affecting developer trust and prompting comparisons to server-side changes in closed models. It underscores the fragility of AI reasoning patterns and the importance of open-source visibility. The clustering occurs at fixed intervals spaced 518 tokens apart, and stuck responses at these thresholds strongly correlate with errors in complex tasks. Users can reproduce the issue with the Codex CLI using puzzle prompts.

hackernews · maille · Jul 4, 21:51 · [Discussion](https://news.ycombinator.com/item?id=48789428)

**Background**: GPT-5.5 Codex is OpenAI's AI coding assistant. Reasoning tokens are used by models to 'think' before responding, and adaptive thinking adjusts token count. Token clustering suggests a bug causing premature truncation of reasoning, similar to a past issue in Claude Code where adaptive-thinking shrinkage led to degraded performance.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48789428">GPT-5.5 Codex reasoning-token clustering may be leading to degraded performance | Hacker News</a></li>
<li><a href="https://lilting.ch/en/articles/claude-code-quality-regression-thinking-redaction">Claude Code adaptive thinking regression: 17,871 thinking ...</a></li>
<li><a href="https://www.anthropic.com/engineering/april-23-postmortem">An update on recent Claude Code quality reports \ Anthropic</a></li>

</ul>
</details>

**Discussion**: Users express concern over quality degradation, with some switching to Claude or local models. They note the issue is easily reproducible and draw parallels to the previous Claude Code regression. Some feel OpenAI hasn't taken the issue seriously.

**Tags**: `#openai`, `#codex`, `#ai-degradation`, `#reasoning-tokens`, `#community-feedback`

---

<a id="item-4"></a>
## [Anna's Archive Offers $200K Bounty for Google Books Scans](https://software.annas-archive.gl/AnnaArchivist/annas-archive/-/work_items/234) ⭐️ 8.0/10

Anna's Archive has announced a $200,000 bounty for a complete collection of Google Books or similar digitized book scans, aiming to expand digital access to knowledge. This bounty could significantly increase the availability of digitized books in regions with restricted access, challenging copyright norms and advancing the shadow library movement. The bounty targets a complete copy of Google Books' scan library or similar collections; Anna's Archive is known for aggregating shadow libraries like Z-Library and Sci-Hub.

hackernews · Cider9986 · Jul 4, 16:51 · [Discussion](https://news.ycombinator.com/item?id=48786838)

**Background**: Anna's Archive is an open source metasearch engine for shadow libraries, launched after Z-Library's crackdown in 2022. It aggregates metadata from multiple sources and aims to catalog all books. Shadow libraries like these often operate in legal gray areas, providing access to copyrighted works without authorization.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anna's_Archive">Anna's Archive</a></li>
<li><a href="https://grokipedia.com/page/Anna's_Archive">Anna's Archive</a></li>

</ul>
</details>

**Discussion**: Community members express gratitude for access to books in restricted regions, with one user sharing a personal success story. Another user mentions SourceLibrary.org with 16,000 rare books, and there is speculation about future bounties for internet scrapes.

**Tags**: `#digital libraries`, `#book scanning`, `#access to knowledge`, `#copyright`, `#community bounty`

---

<a id="item-5"></a>
## [Building a World Map with Only 500 Bytes Using Deflate and JavaScript](https://simonwillison.net/2026/Jul/4/building-a-world-map-with-only-500-bytes/#atom-everything) ⭐️ 8.0/10

Iwo Kadziela demonstrated a technique to generate a credible ASCII world map using only 445 bytes of data by employing deflate compression and modern JavaScript APIs including fetch, data URIs, and DecompressionStream. This showcases a clever combination of compression and web APIs to achieve visually impressive results with minimal data, inspiring new approaches to data-efficient graphics and web development. The technique uses a base64-encoded deflate-raw compressed data URI, which is fetched and decompressed through a DecompressionStream, then rendered as an ASCII preformatted map. The map is drawn using asterisks to represent landmass.

rss · Simon Willison · Jul 4, 23:09

**Background**: Deflate is a lossless data compression algorithm that combines LZ77 and Huffman coding, commonly used in PNG and ZIP files. The DecompressionStream interface is part of the Compression Streams API, enabling stream-based decompression in web browsers. Data URIs allow embedding small data directly into URLs, reducing the need for external files.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/DecompressionStream">DecompressionStream - Web APIs | MDN</a></li>
<li><a href="https://en.wikipedia.org/wiki/DEFLATE">Deflate - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#compression`, `#JavaScript`, `#ASCII art`, `#web development`, `#data URIs`

---

<a id="item-6"></a>
## [Newer Claude Models Show Worse Tool Call Accuracy](https://simonwillison.net/2026/Jul/4/better-models-worse-tools/#atom-everything) ⭐️ 8.0/10

Armin Ronacher reported that newer Anthropic Claude models (Opus 4.8 and Sonnet 5) produce malformed tool calls with invented fields when using Pi's edit tool, while older models do not exhibit this issue. This regression in tool-calling accuracy undermines the reliability of state-of-the-art LLMs for agentic workflows, forcing third-party tool harnesses like Pi to adapt or risk degraded user experience. The issue likely stems from Anthropic training newer models via reinforcement learning to better use Claude Code's built-in edit tool, causing them to invent extra fields when calling third-party edit tools like Pi's.

rss · Simon Willison · Jul 4, 22:53

**Background**: Tool calling (or function calling) allows LLMs to execute external actions by generating structured arguments that match a predefined schema. When models deviate from the schema, tool calls fail, which is especially problematic for coding agents that rely on precise edits. The contrast between Claude's search-and-replace tool and OpenAI's apply_patch mechanism highlights how model-specific training can lead to compatibility issues.

<details><summary>References</summary>
<ul>
<li><a href="https://x.com/mitsuhiko/article/2072955230862332106">Pi's Edit Tool | Armin Ronacher ⇌ (@mitsuhiko) on X</a></li>
<li><a href="https://www.anthropic.com/news/claude-opus-4-8">Introducing Claude Opus 4.8 \ Anthropic</a></li>
<li><a href="https://martinuke0.github.io/posts/2026-01-07-the-anatomy-of-tool-calling-in-llms-a-deep-dive/">The Anatomy of Tool Calling in LLMs: A Deep Dive</a></li>

</ul>
</details>

**Tags**: `#llm`, `#tool-calling`, `#anthropic`, `#regression`, `#model-quality`

---

<a id="item-7"></a>
## [Open Source AI Gap Map Launched by Current AI](https://simonwillison.net/2026/Jul/3/open-source-ai-gap-map/#atom-everything) ⭐️ 8.0/10

Current AI, a non-profit founded at the 2025 AI Action Summit, has launched the Open Source AI Gap Map v0.1, indexing 421 products and over 24,000 artifacts across the open source AI stack. This map provides a structured, publicly available overview of the open source AI ecosystem, helping identify gaps and opportunities for investment and development, which is crucial for the broader AI community and policymakers. The map categorizes 266 software tools, 85 models, 50 datasets, and 20 hardware projects from 228 organizations, with the underlying data (1,184 YAML files) released under MIT license on GitHub.

rss · Simon Willison · Jul 3, 22:04

**Background**: Open source AI encompasses not just models but also tools, datasets, and hardware. Current AI is a global partnership with $400 million committed, aiming to build a 'public option for AI'. This map is part of that effort to systematically understand and improve the open source AI stack.

<details><summary>References</summary>
<ul>
<li><a href="https://www.currentai.org/blogs/introducing-the-gap-map-v0-1">Introducing the Gap Map v0.1</a></li>
<li><a href="https://map.currentai.org/">Current AI – Open Source AI Gap Map</a></li>
<li><a href="https://simonwillison.net/2026/Jul/3/open-source-ai-gap-map/">Open Source AI Gap Map</a></li>

</ul>
</details>

**Discussion**: As the news item is from Simon Willison's blog, the discussion likely appreciates the structured data release and the use of Datasette Lite for exploration, though no specific comments are provided.

**Tags**: `#open source`, `#AI`, `#ecosystem mapping`, `#Current AI`, `#gap analysis`

---

<a id="item-8"></a>
## [Tencent Atuin AI beats Mythos on CyberGym at 0.1% cost](https://mp.weixin.qq.com/s/BzU7g-2iG7d6h4ViwMhxyg) ⭐️ 8.0/10

Tencent Xuanwu Lab's Atuin AI achieved 84.0% on the CyberGym cybersecurity benchmark, surpassing Anthropic's Claude Mythos Preview (83.1%) while consuming less than 0.1% of Mythos's budget. This demonstrates that open-source, cost-effective AI models can rival or surpass proprietary frontier models in specialized cybersecurity tasks, potentially democratizing advanced vulnerability discovery for the broader industry. Atuin AI is built on the open-source GLM-5.1 model, which can run locally, and it discovered multiple high-risk logic vulnerabilities (rating up to 9.3) in real projects like curl, OpenSSL, and Python cryptography that Mythos missed.

telegram · zaihuapd · Jul 3, 16:12

**Background**: CyberGym is a benchmark developed at UC Berkeley that evaluates AI agents in simulated cybersecurity environments, focusing on autonomous vulnerability discovery and exploitation. Claude Mythos Preview is Anthropic's powerful but unreleased model, kept private due to safety concerns over its offensive capabilities. GLM-5.1 is an open-source large language model developed by Z.AI, designed for long-horizon agentic tasks and can operate for up to 8 hours on a single task.

<details><summary>References</summary>
<ul>
<li><a href="https://llm-stats.com/benchmarks/cybergym">CyberGym Benchmark Leaderboard | LLM Stats</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Mythos_Preview">Claude Mythos Preview</a></li>
<li><a href="https://huggingface.co/zai-org/GLM-5.1">zai-org/GLM-5.1 · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Cybersecurity`, `#Benchmark`, `#Vulnerability Detection`, `#Tencent`

---

<a id="item-9"></a>
## [Huawei Unveils 'Tao's Law' Proposing Time Scaling for Chips](https://t.me/zaihuapd/42346) ⭐️ 8.0/10

At the 2026 International Symposium on Circuits and Systems in Shanghai, Huawei introduced 'Tao's Law,' which proposes replacing traditional geometric scaling with 'time scaling' to advance semiconductor technology. The company claims to have designed and mass-produced 381 chips over the past six years using this principle, and plans to release a new Kirin mobile chip with logic folding technology this autumn. This proposal represents a potential paradigm shift in semiconductor scaling as Moore's Law approaches physical limits, offering an alternative path for continued performance gains. If validated, it could reshape chip design strategies for the entire industry, particularly for companies facing advanced process node restrictions. Tao's Law focuses on reducing time constants through multi-level collaborative optimization across devices, circuits, chips, and systems. Huawei predicts that by 2031, high-end chips based on this law could achieve transistor density equivalent to a 1.4nm process node, and its Ascend AI chips are expected to incorporate logic folding around 2030.

telegram · zaihuapd · Jul 4, 04:56

**Background**: Traditional semiconductor scaling (Moore's Law) reduces transistor dimensions geometrically to pack more transistors on a chip, but this approach is hitting physical limits. 'Tao's Law' (τ Law) instead compresses signal propagation delay time through techniques like logic folding, which uses 3D stacking to fold circuit logic paths within a single die, reducing the physical distance signals must travel. This is distinct from conventional 3D packaging that stacks separate dies.

<details><summary>References</summary>
<ul>
<li><a href="https://www.peopleapp.com/column/30052254360-500007517346">“ 韬 定 律 ”，做 时 间 的朋友_人民日报</a></li>
<li><a href="https://news.pedaily.cn/202605/564396.shtml">详解 华 为 “韬定律”：对半导体行业究竟意味着什么？_ 投资界</a></li>
<li><a href="https://user.guancha.cn/main/content?id=1658342&comments-container">user.guancha.cn/main/content?id=1658342&comments-container</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#Huawei`, `#Moore's Law`, `#chip design`, `#logic folding`

---