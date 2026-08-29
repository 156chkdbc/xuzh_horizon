---
layout: default
title: "Horizon Summary: 2026-08-29 (EN)"
date: 2026-08-29
lang: en
---

> From 33 items, 13 important content pieces were selected

---

1. [Triton v3.8.0 Released with New Aggregate APIs and TopK Option](#item-1) ⭐️ 9.0/10
2. [OpenAI Restricts Cursor From Its Models After SpaceX Acquisition](#item-2) ⭐️ 9.0/10
3. [U.S. Sanctions Italian Hosting Collective A/I and Designates noblogs.org as Terrorist](#item-3) ⭐️ 9.0/10
4. [GLM-5.3 Released as Open-Weight, Strong Open Alternative](#item-4) ⭐️ 9.0/10
5. [CLI Tool Boots Virtual iPhone via Apple's Virtualization.framework](#item-5) ⭐️ 8.0/10
6. [Blog Post Argues GUIs Should Be Fully Keyboard-Driven](#item-6) ⭐️ 8.0/10
7. [Htmx 4.0 Has Been Released with New Features and Compatibility Improvements](#item-7) ⭐️ 8.0/10
8. [Bug rumors alone now fuel exploit discovery, says analyst](#item-8) ⭐️ 8.0/10
9. [OpenAI Python SDK Migrates to HTTPX2 to Avoid Breaking Changes](#item-9) ⭐️ 8.0/10
10. [Prompt Injection Attack Bypasses Claude Code Auto Mode 80% of the Time](#item-10) ⭐️ 8.0/10
11. [OpenAI Builds Persistent Codex Agent That Works Until Put to Sleep](#item-11) ⭐️ 8.0/10
12. [Tencent Open-Sources Hy4 Preview: 770B-Parameter MoE Model](#item-12) ⭐️ 8.0/10
13. [Z.ai launches GLM-5.3-Flash: 320B MoE, 18B active, one-tenth the price](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Triton v3.8.0 Released with New Aggregate APIs and TopK Option](https://github.com/triton-lang/triton/releases/tag/v3.8.0) ⭐️ 9.0/10

Triton v3.8.0 was released on the triton-lang GitHub repository, introducing @triton.aggregate and @gluon.aggregate as public APIs and adding a descending argument to tl.topk. The release also includes extensive compiler, NVIDIA/AMD backend, and multi-CTA/TMA improvements. Triton is a widely used GPU programming language and compiler in AI/ML, so this version's improvements will benefit kernel developers targeting both NVIDIA and AMD hardware. The public aggregate API and expanded topk support make writing complex, readable JIT kernels easier. Notable technical details include deterministic JIT cache keys, support for tl.dot_scaled in the interpreter, IEEE-rounded tl.fdiv, and fixed NaN handling for argmin/argmax/minimum/maximum/clamp. Multi-CTA support was extended to layout conversion, reductions, and TMA gather/scatter, and tma.store_wait gained a read_only argument.

github · warrendeng · Aug 28, 18:25

**Background**: Triton is a domain-specific language and compiler for writing high-performance GPU kernels, closely tied to deep learning frameworks. The new aggregate types let developers define structured data passed to kernels, similar to dataclasses. tl.topk is a common operation for finding the k largest or smallest elements along a tensor dimension; the new descending parameter lets users get the smallest values by setting it to False.

<details><summary>References</summary>
<ul>
<li><a href="https://triton-lang.org/main/python-api/generated/triton.language.topk.html">triton.language.topk — Triton documentation</a></li>
<li><a href="https://triton-lang.org/main/dialects/GluonDialect.html">‘gluon’ Dialect — Triton documentation</a></li>
<li><a href="https://github.com/triton-lang/triton/issues/8781">[Frontend] OOP + aggregate in triton/gluon #8781 - GitHub</a></li>

</ul>
</details>

**Tags**: `#triton`, `#GPU`, `#compiler`, `#release`, `#deep learning`

---

<a id="item-2"></a>
## [OpenAI Restricts Cursor From Its Models After SpaceX Acquisition](https://openai.com/index/our-decision-on-cursor-following-its-acquisition-by-spacex/) ⭐️ 9.0/10

OpenAI has decided to restrict Cursor's access to its models following SpaceX's acquisition of the AI code editor. This mirrors Anthropic's earlier ban and puts Cursor's API-reselling business model under serious pressure. The move signals escalating competition among frontier AI model providers over distribution and terms-of-service enforcement. Developers who rely on Cursor to switch between OpenAI, Anthropic, and other models may lose access to their preferred models or face higher costs. OpenAI's restriction follows Anthropic's earlier terms-of-service-based ban on xAI, which was triggered after Musk admitted to distilling competitor models. Cursor lets users mix models from multiple providers in one editor, and the restriction could destabilize that multi-model workflow and its subscription value.

hackernews · meetpateltech · Aug 29, 01:47 · [Discussion](https://news.ycombinator.com/item?id=49486172)

**Background**: Cursor is an AI-native code editor and coding agent developed by San Francisco-based Anysphere, founded in 2022. Part of its business relies on API reselling: Cursor buys access to models from providers such as OpenAI and Anthropic and bundles them into a subscription, letting developers switch between models inside the editor. Anthropic previously banned xAI for similar violations, so OpenAI's decision follows an established pattern of providers controlling where their models are used. The SpaceX acquisition puts Cursor under Elon Musk's corporate umbrella, placing it in direct competition with OpenAI.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cursor_(company)">Cursor (company) - Wikipedia</a></li>
<li><a href="https://builtin.com/articles/what-is-cursor-ai">What Is Cursor? AI Code Editor Explained | Built In</a></li>
<li><a href="https://cloudinsight.cc/en/blog/ai-api-reseller-guide">How to Choose an AI API Reseller ? 2026 Taiwan Enterprise...</a></li>

</ul>
</details>

**Discussion**: Commenters largely view OpenAI's move as an expected business maneuver, noting that Anthropic had already banned xAI. Some Cursor users are disappointed and say multi-model switching is central to their workflow, with some saying they will shift back to Anthropic-only subscriptions; others argue Cursor's API-reselling model was always fragile and that subsidized plans from model providers would eventually make it uncompetitive.

**Tags**: `#AI`, `#OpenAI`, `#Cursor`, `#Acquisition`, `#Developer Tools`

---

<a id="item-3"></a>
## [U.S. Sanctions Italian Hosting Collective A/I and Designates noblogs.org as Terrorist](https://www.inventati.org/) ⭐️ 9.0/10

In late August 2026, the U.S. State Department designated Autistici/Inventati (A/I Collective), an Italian privacy and hosting collective, as a Specially Designated Global Terrorist. The designation also covers noblogs.org, the collective's blogging platform. This is the first time the U.S. has designated an internet infrastructure provider as a global terrorist group, a move that could criminalize the operation of privacy and communication tools. It threatens to chill free speech and encryption projects worldwide, as any hosting service could potentially face similar sanctions. The State Department described A/I as an 'Italy-based extremist group' that builds digital infrastructure for 'violent Antifa cells and other far-left militants.' The designation, issued under Executive Order 13224, freezes any U.S. assets of the collective and prohibits U.S. persons from engaging in transactions with it, though the practical enforcement of sanctions against a non-profit hosting collective remains unclear.

hackernews · exiguus · Aug 28, 12:58 · [Discussion](https://news.ycombinator.com/item?id=49477854)

**Background**: Autistici/Inventati was founded in 2001 by Italian activists to provide free communication, privacy, and hosting tools for social movements. Noblogs.org is a free blogging platform run by the collective, used by a wide range of groups, including anarchists and Antifa sympathizers, but also by ordinary users. The U.S. action marks an unprecedented expansion of counterterrorism sanctions to encompass internet infrastructure, raising alarm among digital rights advocates about the future of basic online privacy tools.

<details><summary>References</summary>
<ul>
<li><a href="https://www.state.gov/releases/office-of-the-spokesperson/2026/08/designation-of-autistici-inventati-as-a-specially-designated-global-terrorist/">Designation of Autistici/Inventati as a Specially Designated ...</a></li>
<li><a href="https://www.autistici.org/who/collective">A short history of the A/I Collective - autistici.org</a></li>
<li><a href="https://noblogs.org/">noblogs . org</a></li>

</ul>
</details>

**Discussion**: Comments on the news are overwhelmingly critical, with many users calling the designation an 'unprecedented' attack on infrastructure providers. A top comment warns that if infrastructure providers can be labeled terrorists, projects like I2P, Monero, Signal, and Tox could be next, while others share historical context about A/I's activist roots and point out inaccuracies in the State Department's claims.

**Tags**: `#sanctions`, `#privacy`, `#internet freedom`, `#infrastructure`, `#surveillance`

---

<a id="item-4"></a>
## [GLM-5.3 Released as Open-Weight, Strong Open Alternative](https://huggingface.co/zai-org/GLM-5.3) ⭐️ 9.0/10

Z.ai has released GLM-5.3 as an open-weight model, building on the same base model as GLM-5.2 with substantially extended post-training to deliver improved coding and agent capabilities. The model is also available as GLM-5.3-Flash on Z.ai's platform. This release provides a compelling open-weight alternative to proprietary models, praised for its capability and token efficiency. It intensifies competition among open-weight LLMs, particularly highlighting the rapid progress of Chinese AI labs. GLM-5.3 uses the same base model as GLM-5.2, with all improvements driven by post-training rather than pretraining. It reportedly offers a good tokens-versus-accuracy ratio, with output tokens covering reasoning and tool calls, and is noted to be easier to run than some competing models like Kimi.

hackernews · jeudesprits · Aug 28, 15:20 · [Discussion](https://news.ycombinator.com/item?id=49479878)

**Background**: Open-weight models are AI models whose trained parameters are publicly released, allowing anyone to download, run, and modify them. GLM is a series of large language models developed by Z.ai (formerly Zhipu AI), a Chinese AI company. Post-training refers to additional training performed after the initial pretraining phase to align the model with desired behaviors and improve specific capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://z.ai/blog/glm-5.3">GLM-5.3: Frontier Coding with Emergent Cyber Capabilities</a></li>
<li><a href="https://docs.z.ai/guides/llm/glm-5.3">GLM-5.3 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>
<li><a href="https://www.interconnects.ai/p/glm-53-how-chinese-labs-keep-stride">GLM-5.3: How Chinese labs keep stride with the frontier</a></li>

</ul>
</details>

**Discussion**: Community reactions are broadly positive, with users praising GLM-5.3 as 'amazing' and noting it handles hard problems with intuition that DeepSeek Flash lacks. Some compare it favorably to Opus 4.8, while others point out it is slightly behind Kimi in ability but easier to run and likely cheaper from third-party providers.

**Tags**: `#AI`, `#LLM`, `#open-weights`, `#GLM`, `#machine-learning`

---

<a id="item-5"></a>
## [CLI Tool Boots Virtual iPhone via Apple's Virtualization.framework](https://github.com/Lakr233/vphone-cli) ⭐️ 8.0/10

A new open-source CLI tool called vphone-cli can boot a virtual iPhone using Apple's official Virtualization.framework. It provides a local, command-line-driven path to full iOS virtualization on Apple hardware for the first time. This matters because it offers a first-party-API-based alternative to physical iPhones for iOS testing and CI pipelines, potentially lowering costs and improving automation. It also challenges existing third-party solutions like Corellium and complements the iOS Simulator with full OS virtualization. The tool leverages Virtualization.framework, which is officially designed for macOS and Linux virtual machines, and repurposes it to boot iOS. One comment notes that during iOS setup, choosing Japan or the EU as the region introduces regulatory checks the VM cannot satisfy; the tool also depends on a macOS host, which limits its scalability.

hackernews · hentrep · Aug 28, 23:02 · [Discussion](https://news.ycombinator.com/item?id=49485267)

**Background**: Apple's Virtualization.framework provides high-level APIs for creating and managing virtual machines on Apple silicon and Intel-based Macs, typically for macOS or Linux guests. Virtualizing iOS is not an officially supported use case, but developers have been experimenting with repurposing this framework to run iOS, as documented in reverse-engineering communities and technical blogs. The iOS Simulator, by contrast, only simulates iOS apps rather than booting the full operating system, so a true virtual iPhone fills a different niche.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.apple.com/documentation/virtualization">Virtualization | Apple Developer Documentation</a></li>
<li><a href="https://www.reddit.com/r/ReverseEngineering/comments/1chcob6/virtualizing_ios_on_apple_silicon/">r/ReverseEngineering on Reddit: Virtualizing iOS on Apple Silicon</a></li>
<li><a href="https://nickb.website/blog/virtualizing-ios-on-apple-silicon">Virtualizing iOS on Apple Silicon | Nick Botticelli</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion is cautiously positive but full of practical questions: users ask whether it can test the phone's browser on localhost, how it differs from the iOS Simulator, and whether it includes a virtual baseband. Some call it a huge win for CI pipelines, while others point out that macOS host dependencies still limit scale.

**Tags**: `#iOS`, `#virtualization`, `#developer-tools`, `#Apple`, `#CI`

---

<a id="item-6"></a>
## [Blog Post Argues GUIs Should Be Fully Keyboard-Driven](https://ckardaris.com/blog/2026/08/28/keyboard-driven-guis.html) ⭐️ 8.0/10

Software engineer ckardaris published a blog post arguing that graphical user interfaces should be fully keyboard-driven, sparking a lively discussion on Hacker News with 712 points and 343 comments. The debate touches on fundamental tensions in software design: accessibility for disabled users, efficiency for power users, and the responsibility of UI frameworks to support keyboard navigation out of the box. It highlights an often-overlooked aspect of UX that affects millions of users. The original post is a personal blog entry rather than a formal proposal, and its exact technical recommendations are not included in the summary. Commenters note that older frameworks like Cocoa/AppKit made keyboard accessibility relatively easy, while modern web frameworks often fail to provide it by default.

hackernews · ckardaris · Aug 28, 15:17 · [Discussion](https://news.ycombinator.com/item?id=49479837)

**Background**: A keyboard-driven GUI is one where every action can be performed without a mouse, typically through tab navigation, shortcuts, and focus management. Keyboard accessibility is a core requirement for users with motor or vision disabilities, and also benefits power users who prefer not to switch between keyboard and mouse. Many desktop UI frameworks provide built-in support, but web apps frequently neglect this, often because developers rely on default browser behavior that is incomplete.

**Discussion**: Commenters generally agree that keyboard accessibility is important but disagree on how to achieve it. One user argues that ADA compliance and inclusion should be a priority, while another pushes back on forcing all users to learn keyboard-driven interfaces, saying power user experience is not the same as general UX. A third commenter raises the question of what 'keyboard-driven' really means, suggesting that merely assigning shortcuts is only 'keyboard-compatible' rather than truly keyboard-driven.

**Tags**: `#accessibility`, `#keyboard-driven`, `#GUI`, `#UX`, `#software engineering`

---

<a id="item-7"></a>
## [Htmx 4.0 Has Been Released with New Features and Compatibility Improvements](https://four.htmx.org/announcements/2026-08-28-htmx-4.0.0-is-released) ⭐️ 8.0/10

Htmx 4.0 was released on August 28, 2026, according to the announcement URL, introducing new features and compatibility improvements for hypermedia-driven web development. Community discussion of the release mentions a new `hx-alpine-compat` extension that smooths over compatibility issues between htmx and Alpine.js. As a major release of one of the most widely used hypermedia libraries, Htmx 4.0 reinforces the viability of hypermedia-driven applications as an alternative to complex JavaScript frameworks. It is particularly significant for developers who favor server-side rendering and minimal client-side scripting. The new `hx-alpine-compat` extension is designed to address interoperability between htmx and Alpine.js, a lightweight JavaScript library. The announcement has drawn 592 points and 145 comments on the community platform, indicating strong interest and diverse opinions.

hackernews · rmsaksida · Aug 28, 13:28 · [Discussion](https://news.ycombinator.com/item?id=49478178)

**Background**: htmx is a small, dependency-free, extendable JavaScript library that allows developers to access modern browser features directly from HTML, rather than writing JavaScript. According to Wikipedia, htmx was created as an improved version of intercooler.js that did not rely on jQuery, with version 1.0.0 released in November 2020. In hypermedia-driven development, a client transitions through application states by selecting from links and forms within the server's responses, an approach explained in the HATEOAS concept from RESTful design.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Htmx">htmx - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/HATEOAS">HATEOAS - Wikipedia</a></li>
<li><a href="https://hypermedia.systems/hypermedia-a-reintroduction/">Hypermedia: A Reintroduction</a></li>

</ul>
</details>

**Discussion**: The community discussion is largely positive but includes one contrarian view. The CEO of htmx says he really likes htmx, while another developer remarks that htmx brings him joy and the Hugs stack (Go, htmx, SQLite) keeps things simple. A .NET/Angular developer, however, found that htmx made things more difficult by forcing presentation concerns back into the backend, and another commenter points out that alpine-ajax is smaller than htmx while covering needed features.

**Tags**: `#htmx`, `#web development`, `#hypermedia`, `#javascript`, `#release`

---

<a id="item-8"></a>
## [Bug rumors alone now fuel exploit discovery, says analyst](https://anil.recoil.org/notes/rumour-is-the-exploit) ⭐️ 8.0/10

A blog post argues that mere rumors of bugs are now enough for attackers to find working exploits, a trend accelerated by LLMs scaling and democratizing vulnerability research. Real-world evidence includes rclone receiving over 40 security disclosures in the past month, versus about 20 in its first decade. This shifts the security landscape: attackers no longer need private details to start hunting, so open-source maintainers face a flood of low-quality but time-consuming reports. It also shows how AI is changing vulnerability discovery and response, with both offensive and defensive implications. The rclone maintainer reports a roughly 75% hit rate for the recent security disclosures, meaning many contain a kernel of truth. Another commenter notes that LLM-driven exploit discovery is not conceptually new but has scaled and democratized mass exploitation of low-value targets, and some builders are already using AI to detect silent bug fixes in commits.

hackernews · avsm · Aug 28, 15:58 · [Discussion](https://news.ycombinator.com/item?id=49480466)

**Background**: Traditionally, vulnerability researchers find exploits by analyzing patches, commit messages, and incidental remarks. LLMs now lower the barrier by letting anyone turn vague hints or rumors into concrete exploit PoCs. This makes exploitation faster and broader, increasing pressure on open-source maintainers who must triage a surge of reports. At the same time, AI can help defenders triage and patch, but organizational will remains a bottleneck.

**Discussion**: Maintainers express being overwhelmed, with rclone's nickcw describing a huge time sink even with AI triage. Some commenters argue the core issue is lack of organizational will to fix bugs, not AI capability, while others note that LLMs have simply scaled an old practice to mass, low-value exploitation. There are also concerns that rollout delays and supply-chain risks make rapid patching unrealistic.

**Tags**: `#security`, `#AI`, `#vulnerabilities`, `#open source`, `#LLM`

---

<a id="item-9"></a>
## [OpenAI Python SDK Migrates to HTTPX2 to Avoid Breaking Changes](https://github.com/openai/openai-python/blob/main/httpx2.md) ⭐️ 8.0/10

OpenAI's Python SDK is migrating to HTTPX2, a fork of the httpx library that preserves the existing API instead of following httpx's planned 1.0 breaking changes. Anthropic made the same switch in its Python SDK shortly afterward. This matters because OpenAI and Anthropic are among the most widely used Python SDKs, so their dependency choices affect thousands of developers. Choosing a stable fork over a moving target helps protect downstream projects from unexpected breaking changes in httpx 1.0. According to community discussion, HTTPX2 is essentially a fork of httpx that promises not to break the existing API, making it a more stable dependency. One notable behavioral change is that the SDK now uses the operating system's TLS trust store instead of certifi.

hackernews · tosh · Aug 28, 11:51 · [Discussion](https://news.ycombinator.com/item?id=49477212)

**Background**: httpx is a popular next-generation HTTP client for Python that provides sync and async APIs, and supports both HTTP/1.1 and HTTP/2. Many SDKs, including OpenAI's, depend on httpx to make API requests. Because httpx is heading toward a 1.0 release with breaking changes, some library maintainers prefer a fork like HTTPX2 that offers API stability.

<details><summary>References</summary>
<ul>
<li><a href="https://pypi.org/project/httpx/">httpx · PyPI</a></li>
<li><a href="https://www.python-httpx.org/">HTTPX</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters had mixed reactions. Simon Willison confirmed Anthropic made the same switch and explained that httpx2 promises not to break the existing API, while jklehm wondered whether niquests was evaluated as an alternative. Others asked what the upsides were, and tosh noted that the SDK now uses the operating system's TLS trust store instead of certifi.

**Tags**: `#openai`, `#httpx`, `#python`, `#http-client`, `#sdk`

---

<a id="item-10"></a>
## [Prompt Injection Attack Bypasses Claude Code Auto Mode 80% of the Time](https://simonwillison.net/2026/Aug/27/breaking-claude-code-opus-5-auto-mode/) ⭐️ 8.0/10

Security researcher Johann Rehberger demonstrated a prompt injection attack that bypasses Claude Code's auto mode approximately 80% of the time. The attack tricks the agent into extracting a zip archive containing a malicious local struct.py, which shadows Python's standard library during an import of base64 and executes attacker-controlled code. This directly challenges Anthropic's safety claims about auto mode, which is now the default mode for Claude Code. It shows that LLM-based safety classifiers can be bypassed, underscoring the need for sandboxing and stricter security practices for AI coding agents. The attack succeeded about 80% of the time, and in some runs auto mode even blocked Claude's own cleanup commands after the agent detected the compromise. Rehberger recommends running unattended coding agents in a container, VM, or OS sandbox; restricting network egress; and not exposing credentials to the agent runtime.

rss · Simon Willison · Aug 27, 22:50

**Background**: Claude Code is Anthropic's agentic coding tool that can edit files, run commands, and execute code in a developer's environment. Auto mode routes tool calls through an LLM classifier that blocks reversible, destructive, or out-of-environment actions, replacing the older --dangerously-skip-permissions flag. The attack exploits Python's import behavior, where a local file with the same name as a standard-library module shadows the real module. This illustrates a broader class of prompt injection risks for AI agents handling untrusted content.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/engineering/claude-code-auto-mode">How we built Claude Code auto mode: a safer way to skip permissions \ Anthropic</a></li>
<li><a href="https://code.claude.com/docs/en/auto-mode-config">Configure auto mode - Claude Code Docs</a></li>
<li><a href="https://bobbyhadz.com/blog/python-importerror-cannot-import-name">ImportError: cannot import name X in Python [Solved] | bobbyhadz</a></li>

</ul>
</details>

**Tags**: `#security`, `#prompt injection`, `#AI agents`, `#LLM`, `#Claude Code`

---

<a id="item-11"></a>
## [OpenAI Builds Persistent Codex Agent That Works Until Put to Sleep](https://www.wired.com/story/openai-is-developing-a-persistent-ai-agent/) ⭐️ 8.0/10

WIRED reviewed code showing OpenAI is adding a 'persistent mode' to its Codex CLI, letting the agent work continuously across sessions until the user puts it to sleep. OpenAI confirmed it is testing the feature but gave no release timeline. A persistent agent could shift AI coding tools from one-shot assistants to long-running teammates that proactively plan and execute multi-step engineering work. This could significantly boost developer productivity and accelerate the industry's move toward more autonomous AI agents. The mode includes a 'proactive' setting that lets the agent create follow-up tasks after answering requests and act across sessions based on its understanding of the user. Persistent mode is not meant to expand the agent's permissions: changes to anything outside the user's own system still require prior approval.

telegram · zaihuapd · Aug 28, 02:47

**Background**: Codex is OpenAI's AI coding agent, released in April 2025 as a terminal-based tool called Codex CLI and now also available in ChatGPT, desktop apps, and IDEs. Today's coding agents are usually reactive and stateless—they wait for a prompt and lose context when a session ends—so persistent memory and proactive task creation are considered key steps toward more autonomous agents.

<details><summary>References</summary>
<ul>
<li><a href="https://www.wired.com/story/openai-is-developing-a-persistent-ai-agent/">OpenAI Is Developing a ‘ Persistent ’ AI Agent | WIRED</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_Codex_(AI_agent)">OpenAI Codex (AI agent)</a></li>
<li><a href="https://learn.chatgpt.com/docs/codex/cli">Codex CLI | ChatGPT Learn</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#Codex`, `#AI agents`, `#software engineering`, `#AI tools`

---

<a id="item-12"></a>
## [Tencent Open-Sources Hy4 Preview: 770B-Parameter MoE Model](https://mp.weixin.qq.com/s/ymr3X878B8oa2XP15CH8TQ) ⭐️ 8.0/10

Tencent released and open-sourced Hy4 preview, a Mixture-of-Experts (MoE) model with 770B total parameters and 49B active parameters, on August 28, 2026. In blind tests across 203 engineering tasks, it scored 2.99, narrowly beating GLM-5.3 (2.92) and Kimi K3 (2.94). This release marks a major step for open-source AI, as Tencent's model competes head-to-head with top closed and open models from other Chinese labs. Developers and researchers gain access to a frontier-scale model with a 1M-token context window, potentially accelerating work in software engineering, document processing, and scientific research. The model's backbone has 78 layers: the first uses a dense FFN, while the remaining 77 layers each contain 256 routed experts plus 1 shared expert. API pricing is set at $0.834 per million input tokens and $2.501 per million output tokens, with checkpoints available on Tencent Cloud, GitHub, HuggingFace, ModelScope, AtomGit, and OpenRouter.

telegram · zaihuapd · Aug 28, 06:11

**Background**: Mixture-of-Experts (MoE) architectures make it possible to build extremely large language models while keeping inference costs low: only a subset of 'expert' parameters are activated for each token. This is why Hy4 preview can have 770B total parameters yet only 49B active per token. ModelScope is an open-source platform that provides Model-as-a-Service, making it easier for developers to deploy and use such models.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tencent.com/tencent-releases-and-open-sources-tencent-hy4-preview/">Tencent Releases and Open-Sources Tencent Hy4 preview</a></li>
<li><a href="https://github.com/Tencent-Hunyuan/Hy4-preview">Tencent-Hunyuan/Hy4-preview - GitHub</a></li>
<li><a href="https://www.ibm.com/think/topics/mixture-of-experts">What is mixture of experts? | IBM</a></li>

</ul>
</details>

**Tags**: `#AI`, `#LLM`, `#Tencent`, `#open-source`, `#model release`

---

<a id="item-13"></a>
## [Z.ai launches GLM-5.3-Flash: 320B MoE, 18B active, one-tenth the price](https://t.me/zaihuapd/43471) ⭐️ 8.0/10

Z.ai released GLM-5.3-Flash, its first native multimodal model in the GLM-5 series, with 320B total parameters and only 18B active parameters. It outperforms GLM-5.2 on several coding and agent benchmarks while priced at roughly one-tenth the cost of the previous generation, with a limited-time API input price of $0.075 per million tokens. This release signals a major push toward 'frontier performance at budget prices': GLM-5.3-Flash reportedly comes close to Claude Opus 4.8 on coding evals while costing an order of magnitude less. High-volume coding and automation workloads that previously required expensive frontier models may now be served affordably, potentially reshaping API pricing competition. The limited-time promotional pricing is $0.075 per million input tokens, $0.015 for cached input, and $0.25 for output tokens, with cache storage temporarily free. As a Mixture-of-Experts (MoE) model, only 18B of its 320B parameters are activated per token, which is the key to its efficiency; the model was previously tested anonymously as 'Ox Alpha' before the official release.

telegram · zaihuapd · Aug 28, 15:32

**Background**: Mixture-of-experts (MoE) is a neural network architecture in which only a subset of 'expert' parameters is activated for each token, reducing compute while keeping large model capacity. GLM-5.3-Flash uses this design: the 320B total parameters include shared parts and experts, but only 18B active parameters are used per token. Z.ai's GLM-5.3 series shares the same base model as GLM-5.2, with improvements driven by post-training rather than architectural changes.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://www.datacamp.com/blog/glm-5-3-flash">GLM-5.3-Flash: Features, Benchmarks, and Pricing | DataCamp</a></li>
<li><a href="https://docs.z.ai/guides/llm/glm-5.3">GLM-5.3 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>

</ul>
</details>

**Tags**: `#AI`, `#GLM`, `#multimodal`, `#LLM`, `#API pricing`

---