---
layout: default
title: "Horizon Summary: 2026-05-09 (EN)"
date: 2026-05-09
lang: en
---

> From 36 items, 12 important content pieces were selected

---

1. [AI is breaking two vulnerability cultures](#item-1) ⭐️ 9.0/10
2. [Triton v3.7.0: New Operations, Scaled BMM, and FP8 Constants](#item-2) ⭐️ 8.0/10
3. [Google reCAPTCHA breaks for de-googled Android users](#item-3) ⭐️ 8.0/10
4. [Meshtastic: Off-Grid Mesh Text Messaging](#item-4) ⭐️ 8.0/10
5. [Mojo 1.0 Beta: Python-Compatible Language with Rust-Like Performance](#item-5) ⭐️ 8.0/10
6. [Mozilla Hardens Firefox Using Claude Mythos AI](#item-6) ⭐️ 8.0/10
7. [ChatGPT Adds 'Trusted Contact' Feature for Self-Harm Detection](#item-7) ⭐️ 8.0/10
8. [OpenAI Codex Gets Chrome Extension for Browser Agent Tasks](#item-8) ⭐️ 8.0/10
9. [Cloudflare lays off 1100+ employees, cites AI-driven restructuring](#item-9) ⭐️ 8.0/10
10. [Anthropic Plans Massive Funding Round, Valuation Could Hit $1 Trillion](#item-10) ⭐️ 8.0/10
11. [US Suspects Nvidia Chips Smuggled to Alibaba via Thailand](#item-11) ⭐️ 8.0/10
12. [Apple may end TSMC's exclusive chip foundry deal, considers Intel](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [AI is breaking two vulnerability cultures](https://www.jefftk.com/p/ai-is-breaking-two-vulnerability-cultures) ⭐️ 9.0/10

AI tools like LLMs are accelerating the breakdown of distinct vulnerability disclosure cultures for open source and closed source software by enabling easier exploit generation and analysis. This forces a reevaluation of disclosure norms and embargoes, as the window for coordinated vulnerability disclosure shrinks, affecting both open source and proprietary software ecosystems. The breakdown has been building due to increased software transparency and improved reverse engineering tools, predating LLMs; community comments note that exploit generation via diffing commits was already possible.

hackernews · speckx · May 8, 17:55 · [Discussion](https://news.ycombinator.com/item?id=48066524)

**Background**: Vulnerability disclosure traditionally followed two cultures: open source, where patches are public and exploits can be reverse-engineered quickly, and closed source, where disclosure is coordinated with embargoes to allow time for fixes. Embargoes are time windows during which a vulnerability is kept secret among trusted parties. AI tools lower the barrier to exploit generation, eroding the effectiveness of embargoes and blurring the distinction between these cultures.

<details><summary>References</summary>
<ul>
<li><a href="https://dl.acm.org/doi/full/10.1145/3716822">An Empirical Study on Vulnerability Disclosure Management of ...</a></li>
<li><a href="https://openssf.org/groups/vulnerability-disclosures/">Vulnerability Disclosures – Open Source Security Foundation</a></li>
<li><a href="https://www.redhat.com/en/blog/Understanding-security-embargoes-at-Red-Hat">Understanding security embargoes at Red Hat</a></li>

</ul>
</details>

**Discussion**: Comments show mixed views: tptacek argues the crackup was predicted and driven by software transparency, not just AI; dmurray sarcastically suggests moving Linux to a closed-source model; rikafurude21 notes it's an old problem reframed; freeqaz cites Log4Shell as an example where black hats exploited public patches before coordinated disclosure.

**Tags**: `#AI`, `#security`, `#vulnerability disclosure`, `#open source`, `#cybersecurity`

---

<a id="item-2"></a>
## [Triton v3.7.0: New Operations, Scaled BMM, and FP8 Constants](https://github.com/triton-lang/triton/releases/tag/v3.7.0) ⭐️ 8.0/10

Triton v3.7.0 introduces new operations like tl.squeeze and tl.unsqueeze, scaled batched matrix multiplication (scaled BMM), and the ability to create FP8 constants directly. It also includes backend improvements for AMD/HIP and NVIDIA, along with bug fixes and performance optimizations. Triton is a widely-used GPU compiler for AI/ML, and this release enhances its expressiveness and performance, enabling more efficient custom kernel development. Scaled BMM and FP8 support are particularly important for modern deep learning workloads like transformers. The scaled BMM feature (PR #9000) allows batched matrix multiplication with scaling, beneficial for attention mechanisms. FP8 constants (PR #8882) enable direct creation of 8-bit floating point values. The release also includes breaking changes, such as a deprecation warning for make_block_ptr.

github · atalman · May 7, 22:19

**Background**: Triton is an open-source language and compiler for writing efficient GPU kernels, developed by OpenAI. It allows developers to write high-performance code in Python without needing to use low-level CUDA. Scaled BMM refers to batched matrix multiplication where the result is scaled by a factor, commonly used in scaled dot-product attention. FP8 is an 8-bit floating-point format (E4M3 and E5M2) designed to reduce memory and compute in deep learning while maintaining accuracy.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/triton/">Introducing Triton: Open-source GPU programming for neural networks | OpenAI</a></li>
<li><a href="https://github.com/triton-lang/triton">GitHub - triton-lang/triton: Development repository for the Triton language and compiler · GitHub</a></li>
<li><a href="https://developer.nvidia.com/blog/floating-point-8-an-introduction-to-efficient-lower-precision-ai-training/">Floating-Point 8: An Introduction to Efficient, Lower-Precision AI Training | NVIDIA Technical Blog</a></li>

</ul>
</details>

**Discussion**: No community comments were provided in the news item.

**Tags**: `#triton`, `#gpu`, `#compiler`, `#deep-learning`

---

<a id="item-3"></a>
## [Google reCAPTCHA breaks for de-googled Android users](https://reclaimthenet.org/google-broke-recaptcha-for-de-googled-android-users) ⭐️ 8.0/10

Google updated reCAPTCHA to a remote attestation system, causing it to fail for Android users who have removed Google Play Services, such as those running GrapheneOS or Huawei phones. This change restricts access for privacy-conscious users and non-Google devices, highlighting tensions between anti-abuse measures and user autonomy, and may push more websites to seek alternative CAPTCHA solutions. The new reCAPTCHA essentially performs remote attestation, requiring interaction with Google servers and potentially leaking hardware-bound identifiers. Community members describe it as a form of Know Your Customer (KYC) verification.

hackernews · anonymousiam · May 8, 18:45 · [Discussion](https://news.ycombinator.com/item?id=48067119)

**Background**: De-googled Android refers to devices running Android without Google's proprietary services, often achieved via custom ROMs like GrapheneOS or by disabling Google apps. Remote attestation is a security mechanism where a device proves its integrity to a remote server using hardware-backed keys, commonly used in confidential computing.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeGoogle">DeGoogle - Wikipedia</a></li>
<li><a href="https://confidentialcomputing.io/2024/10/02/what-is-remote-attestation-enhancing-data-governance-with-confidential-computing/">What Is Remote Attestation? Enhancing Data Governance with ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed concerns that reCAPTCHA is now a de facto KYC gate, with one user noting it forces users to have a SIM and Google account. Others shared alternatives like hCaptcha or self-hosted verification, while some recounted their experience switching to GrapheneOS and self-hosted services to avoid Google dependency.

**Tags**: `#privacy`, `#Android`, `#reCAPTCHA`, `#degoogling`, `#remote attestation`

---

<a id="item-4"></a>
## [Meshtastic: Off-Grid Mesh Text Messaging](https://meshtastic.org/docs/introduction/) ⭐️ 8.0/10

Meshtastic, a LoRa-based mesh text messaging system for off-grid communication, has been introduced on its official site, drawing significant community attention with 368 points and 145 comments. This technology enables decentralized, low-power, long-range communication without relying on existing infrastructure, which is crucial for emergency scenarios, outdoor activities, and IoT applications where internet access is unavailable. Meshtastic operates in license-free ISM radio bands using LoRa modulation, with limited transmit power but no restrictions on encryption. It forms a mesh network by rebroadcasting messages, and each device can connect to a single phone.

hackernews · ColinWright · May 8, 11:22 · [Discussion](https://news.ycombinator.com/item?id=48061566)

**Background**: LoRa is a proprietary spread spectrum modulation technique designed for long-range, low-power wireless communication, commonly used in IoT. A mesh network is a topology where each node relays data for others, extending coverage. Meshtastic combines these to create a decentralized off-grid messaging system, operating in the 915 MHz (US) or 868 MHz (EU) ISM bands.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Meshtastic">Meshtastic</a></li>
<li><a href="https://meshtastic.org/">Off-Grid Communication For Everyone | Meshtastic</a></li>

</ul>
</details>

**Discussion**: Many commenters expressed excitement about discovering Meshtastic, with some longtime users praising its potential and noting it encouraged them to get a HAM license. However, there were also concerns about the organization's litigiousness, with one user highlighting that the leadership has aggressively protected the 'Meshtastic' name against other projects.

**Tags**: `#mesh networking`, `#LoRa`, `#decentralized communication`, `#amateur radio`, `#open source`

---

<a id="item-5"></a>
## [Mojo 1.0 Beta: Python-Compatible Language with Rust-Like Performance](https://mojolang.org/) ⭐️ 8.0/10

Mojo 1.0 Beta has been released, introducing a Python-compatible programming language that combines high-level syntax with systems-level performance features such as ownership and comptime (compile-time computation). This release is significant because Mojo aims to bridge the gap between ease of use (Python) and raw performance (C++/Rust), potentially transforming AI and high-performance computing by allowing developers to write fast code without sacrificing productivity. It also generates high community excitement, with many hoping it becomes a viable alternative to Julia, Numba, and Triton. Mojo uses MLIR (Multi-Level Intermediate Representation) rather than directly targeting LLVM, enabling better optimization for CPUs, GPUs, and other accelerators. However, the compiler remains closed source as of October 2025, with an open source standard library; Modular has committed to open-sourcing Mojo in fall 2026.

hackernews · sbt567 · May 8, 02:49 · [Discussion](https://news.ycombinator.com/item?id=48057901)

**Background**: Mojo is a systems programming language developed by Modular Inc., designed for high-performance AI infrastructure. It builds on MLIR, a compiler framework that allows higher-level optimizations than LLVM alone. Key features include an ownership model similar to Rust for memory safety without garbage collection, and comptime (compile-time computation) for zero-cost abstractions akin to Zig. Mojo's syntax is intentionally Python-compatible to ease adoption by the large Python ecosystem, particularly in machine learning and scientific computing.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mojo_(programming_language)">Mojo (programming language)</a></li>
<li><a href="https://www.modular.com/open-source/mojo">Mojo : Powerful CPU+GPU Programming</a></li>
<li><a href="https://zig.guide/language-basics/comptime/">Comptime - zig.guide</a></li>

</ul>
</details>

**Discussion**: Community members are enthusiastic about Mojo's unique features, with one user praising its ownership model, comptime, and SIMD support, calling it 'the first language in a long time that isn't just an LLVM wrapper.' However, some express concerns about syntax differences from Python (e.g., string indexing behavior) and note that Julia already addresses many of the same use cases. Others worry about correctness issues and the language's closed-source status, though the promise of open-sourcing in 2026 is well received.

**Tags**: `#programming language`, `#performance`, `#python`, `#systems programming`, `#ML`

---

<a id="item-6"></a>
## [Mozilla Hardens Firefox Using Claude Mythos AI](https://simonwillison.net/2026/May/7/firefox-claude-mythos/#atom-everything) ⭐️ 8.0/10

Mozilla used access to the Claude Mythos preview to locate and fix hundreds of vulnerabilities in Firefox, dramatically increasing monthly security bug fixes from 20-30 to 423 in April 2026. This demonstrates a major improvement in AI-assisted security auditing, shifting from ineffective AI bug reports to highly effective vulnerability detection, potentially setting a new standard for open-source project security. The harnessed AI discovered a 20-year-old XSLT bug and a 15-year-old bug in the <legend> element, while many attempts were blocked by Firefox's existing defense-in-depth measures, which is reassuring.

rss · Simon Willison · May 7, 17:56

**Background**: Firefox is a widely-used open-source browser. Claude Mythos Preview is a highly capable AI model from Anthropic, particularly strong at software engineering and cybersecurity tasks. Traditionally, AI-generated security bug reports were often low-quality and imposed a burden on maintainers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/claude-mythos-preview-risk-report">Alignment Risk Update: Claude Mythos Preview - anthropic.com</a></li>
<li><a href="https://www.aisi.gov.uk/blog/our-evaluation-of-claude-mythos-previews-cyber-capabilities">Our evaluation of Claude Mythos Preview’s cyber capabilities</a></li>

</ul>
</details>

**Tags**: `#security`, `#AI`, `#Firefox`, `#vulnerability detection`, `#open source`

---

<a id="item-7"></a>
## [ChatGPT Adds 'Trusted Contact' Feature for Self-Harm Detection](https://www.theverge.com/ai-artificial-intelligence/925874/chatgpt-trusted-contact-emergency-self-harm-notification) ⭐️ 8.0/10

OpenAI has introduced an optional 'trusted contact' feature for adult ChatGPT users, which can notify a designated friend or family member when the system detects self-harm or suicidal language. The notification is sent after a trained team reviews the conversation and confirms a serious safety concern, without sharing the chat content. This feature addresses a critical real-world problem where AI interactions may inadvertently escalate mental health crises, following a tragic incident involving a teenager. It extends safety measures to adults and sets an industry precedent for responsible AI deployment. The feature requires both the user and the trusted contact to be adults (19+ in South Korea), and the contact must accept the invitation within one week. Notifications can be sent via email, SMS, or ChatGPT in-app notification, and Meta has implemented a similar feature for Instagram to alert parents when teens repeatedly search for self-harm topics.

telegram · zaihuapd · May 8, 02:47

**Background**: ChatGPT's new feature builds on previous safety measures for teens, which were introduced after a 16-year-old boy died by suicide following prolonged conversations with the AI chatbot. The incident raised concerns about AI's role in mental health support and the need for better safeguards. OpenAI has now extended similar protections to adult users.

**Tags**: `#safety`, `#AI ethics`, `#ChatGPT`, `#mental health`, `#OpenAI`

---

<a id="item-8"></a>
## [OpenAI Codex Gets Chrome Extension for Browser Agent Tasks](https://developers.openai.com/codex/changelog) ⭐️ 8.0/10

OpenAI has released a Chrome extension for Codex, its AI coding agent, allowing it to operate directly in the browser to perform multi-step tasks like navigation and data entry across multiple tabs in the background. This extension transforms Codex from a coding tool into a practical browser automation agent, enabling users to delegate repetitive web tasks without API integration, which could significantly boost productivity for developers and knowledge workers. Codex executes tasks by writing and running code in background tabs, automatically combining browser and plugin tools as needed. The extension is available globally except the EU and UK, with those regions to be supported later.

telegram · zaihuapd · May 8, 04:17

**Background**: Codex is an AI coding agent by OpenAI released in April 2025, capable of writing code, fixing bugs, and accelerating software engineering tasks. Browser automation for AI agents typically relies on the Chrome DevTools Protocol (CDP) to control the browser. This new extension extends Codex's capabilities to directly interact with web applications in real-time.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Codex_(AI_agent)">Codex (AI agent) - Wikipedia</a></li>
<li><a href="https://openai.com/codex/">Codex | AI Coding Partner from OpenAI</a></li>
<li><a href="https://www.allabtai.com/ai-browser-automation/">AI Browser Automation: Complete Guide for AI Agents (2026)</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#Codex`, `#Chrome扩展`, `#AI agent`, `#浏览器自动化`

---

<a id="item-9"></a>
## [Cloudflare lays off 1100+ employees, cites AI-driven restructuring](https://blog.cloudflare.com/building-for-the-future/) ⭐️ 8.0/10

On May 7, 2026, Cloudflare announced layoffs of over 1100 employees, citing a 600% increase in internal AI usage over the past three months as the primary driver for organizational restructuring. This layoff reflects a broader industry trend where rapid AI adoption is reshaping workforce structures, potentially setting a precedent for other tech companies considering similar moves. The severance package includes full base salary until end of 2026, US health insurance through year-end, equity vesting extended to August 15, 2026, and waiver of cliff vesting for employees with less than one year of service. The company emphasized a one-time, single-round layoff, communicated directly via email.

telegram · zaihuapd · May 8, 08:15

**Background**: Cloudflare is a major internet infrastructure company providing services like CDN and DDoS protection. AI agents are systems that autonomously perform tasks using tools and workflows; their rapid adoption can lead to workforce reduction as tasks are automated. Cliff vesting is a provision requiring a minimum service period before earning equity rights, commonly used in startups.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent</a></li>
<li><a href="https://www.lawinsider.com/clause/cliff-vesting">Cliff Vesting Sample Clauses | Law Insider</a></li>

</ul>
</details>

**Tags**: `#Cloudflare`, `#AI`, `#layoffs`, `#corporate restructuring`, `#tech industry`

---

<a id="item-10"></a>
## [Anthropic Plans Massive Funding Round, Valuation Could Hit $1 Trillion](https://www.ft.com/content/a40cafcc-0fa4-4e70-9e24-90d826aea56d) ⭐️ 8.0/10

Anthropic is considering raising hundreds of billions of dollars in a new funding round this summer, which could push its valuation to nearly $1 trillion, surpassing OpenAI's latest estimated valuation of around $880 billion. This would make Anthropic the most valuable AI startup, overtaking OpenAI, and signals the escalating capital intensity in the AI race as companies race to secure computing infrastructure. In February, Anthropic completed a $30 billion funding round at a $380 billion valuation; secondary market trading now implies a valuation between $1 trillion and $1.2 trillion. The new funding is intended to support significant expansion of computing capacity.

telegram · zaihuapd · May 8, 11:15

**Background**: Anthropic is a leading AI company focused on developing safe and capable AI systems, competing directly with OpenAI. The AI industry has seen massive investments in recent years, with valuations soaring as demand for advanced computing resources grows. This fundraising reflects a broader trend of AI companies raising enormous sums to build data centers and acquire GPUs.

**Tags**: `#AI`, `#融资`, `#Anthropic`, `#OpenAI`, `#估值`

---

<a id="item-11"></a>
## [US Suspects Nvidia Chips Smuggled to Alibaba via Thailand](https://www.bloomberg.com/news/articles/2026-05-08/us-said-to-suspect-nvidia-chips-smuggled-to-alibaba-via-thailand) ⭐️ 8.0/10

US prosecutors suspect Thai company OBON Corp. smuggled $2.5 billion worth of Super Micro servers containing advanced Nvidia chips to China, with Alibaba as one end customer. This case highlights ongoing US-China tensions over AI chip export controls and could lead to tighter restrictions on chip shipments to Thailand, affecting regional AI development. Alibaba denies any business relationship with Super Micro or OBON, and Siam AI's CEO claims he left OBON and that the company was not involved in smuggling.

telegram · zaihuapd · May 8, 13:23

**Background**: Since 2022, the US has restricted exports of advanced Nvidia AI chips like the A100 and H100 to China to prevent military use. Thailand has become a potential transshipment point due to looser controls. Super Micro is a major server manufacturer, and its servers often contain Nvidia GPUs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.supermicro.com/">Supermicro Data Center Server , Blade, Data Storage, AI System</a></li>
<li><a href="https://siam.ai/">SIAM AI CORPORATION CO., LTD.</a></li>

</ul>
</details>

**Tags**: `#Nvidia`, `#chip smuggling`, `#US-China trade`, `#AI`, `#export controls`

---

<a id="item-12"></a>
## [Apple may end TSMC's exclusive chip foundry deal, considers Intel](https://t.me/zaihuapd/41292) ⭐️ 8.0/10

According to the Wall Street Journal, Apple is considering ending TSMC's exclusive chip manufacturing arrangement that has been in place since 2014, and may outsource some mid-to-low-end processors to other foundries. Intel is a potential candidate, possibly using its 18A process to manufacture chips for Mac, iPad, or iPhone as early as 2027. This move could reshape the semiconductor foundry landscape by reducing Apple's reliance on a single supplier and opening a significant revenue stream for Intel's foundry business. It also highlights the growing demand pressure on TSMC from AI chipmakers like Nvidia. Intel's role would be limited to manufacturing; Apple would retain chip design. The 18A process is Intel's advanced node expected to deliver performance and power improvements, though the timeline remains tentative and subject to change.

telegram · zaihuapd · May 8, 17:18

**Background**: Apple has relied exclusively on TSMC for its custom chips (A-series and M-series) since 2014, after transitioning from Samsung. TSMC's leading-edge capacity is increasingly constrained by orders from AI companies, prompting Apple to diversify its supply chain. Intel has been expanding its foundry services and positions 18A as a competitive node for external customers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.intel.com/content/www/us/en/foundry/process/18a.html">Intel 18A | See Our Biggest Process Innovation</a></li>

</ul>
</details>

**Tags**: `#苹果`, `#芯片代工`, `#台积电`, `#英特尔`, `#供应链`

---