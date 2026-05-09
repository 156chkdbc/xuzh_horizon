---
layout: default
title: "Horizon Summary: 2026-05-09 (EN)"
date: 2026-05-09
lang: en
---

> From 37 items, 13 important content pieces were selected

---

1. [Mozilla uses Claude Mythos to find hundreds of Firefox bugs](#item-1) ⭐️ 9.0/10
2. [Triton 3.7.0: New Tensor Ops and FP8 Support](#item-2) ⭐️ 8.0/10
3. [Google's reCAPTCHA now performs remote attestation, blocking de-googled Android users](#item-3) ⭐️ 8.0/10
4. [AI Disrupts Two Vulnerability Disclosure Cultures](#item-4) ⭐️ 8.0/10
5. [Meta Ends End-to-End Encryption for Instagram DMs](#item-5) ⭐️ 8.0/10
6. [Mojo 1.0 Beta Released: Python-compatible with Rust ownership and Zig comptime](#item-6) ⭐️ 8.0/10
7. [Luke Curley Criticizes WebRTC's Packet Dropping for LLM Prompts](#item-7) ⭐️ 8.0/10
8. [Canvas LMS Hacked by ShinyHunters Disrupts US School Finals](#item-8) ⭐️ 8.0/10
9. [Cloudflare lays off 1100+, cites 600% AI usage surge as cause](#item-9) ⭐️ 8.0/10
10. [Anthropic seeks hundreds of billions in funding, valuation nears $1 trillion](#item-10) ⭐️ 8.0/10
11. [US suspects Nvidia chips smuggled to China via Thailand; Alibaba named as end customer](#item-11) ⭐️ 8.0/10
12. [DeepSeek Seeks $45B Valuation with State-Backed Funding](#item-12) ⭐️ 8.0/10
13. [Apple May End TSMC's Chip Exclusivity, Consider Intel for Some Chips](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Mozilla uses Claude Mythos to find hundreds of Firefox bugs](https://simonwillison.net/2026/May/7/firefox-claude-mythos/#atom-everything) ⭐️ 9.0/10

Mozilla utilized a preview of Anthropic's Claude Mythos model to locate and fix hundreds of security vulnerabilities in Firefox, with April 2026 seeing 423 security bug fixes, a dramatic increase from the typical 20-30 per month. This marks a paradigm shift in AI-assisted security, transforming LLMs from generating unusable bug reports to producing high-quality, actionable vulnerability discoveries, which could significantly reduce the cost and effort of open-source software hardening. Among the discovered bugs were a 20-year-old XSLT bug and a 15-year-old bug in the <legend> HTML element; many attempts were blocked by Firefox's defense-in-depth measures, highlighting the model's ability to find subtle flaws.

rss · Simon Willison · May 7, 17:56

**Background**: Claude Mythos is an advanced AI model by Anthropic designed for complex, multi-step cybersecurity tasks. Previously, AI-generated security reports were often incorrect and burdensome for maintainers. Mozilla combined improved models with better prompting techniques to filter noise and amplify signal, achieving a breakthrough in vulnerability detection.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_(language_model)">Claude (language model) - Wikipedia</a></li>
<li><a href="https://www.bbc.com/news/articles/crk1py1jgzko">What is Anthopic's Claude Mythos and what risks does it pose?</a></li>
<li><a href="https://www.pluralsight.com/resources/blog/ai-and-data/what-is-claude-mythos">What is Claude Mythos? | Pluralsight</a></li>

</ul>
</details>

**Tags**: `#AI`, `#security`, `#Firefox`, `#vulnerability detection`, `#LLM`

---

<a id="item-2"></a>
## [Triton 3.7.0: New Tensor Ops and FP8 Support](https://github.com/triton-lang/triton/releases/tag/v3.7.0) ⭐️ 8.0/10

Triton 3.7.0 introduces tl.squeeze and tl.unsqueeze operations, scaled batched matrix multiplication, and direct creation of FP8 constants. The release also includes backend enhancements for both AMD and NVIDIA GPUs. This release improves Triton's expressiveness for deep learning workloads, particularly for low-precision FP8 computations which are increasingly used for efficient inference. The new operations simplify writing complex GPU kernels. The scaled BMM operation enables efficient batched matrix multiplication with optional scaling. FP8 constants allow direct use of 8-bit floating-point values without conversion. Backend improvements include 2CTA mode and TMA multicast for NVIDIA and various fixes for AMD.

github · atalman · May 7, 22:19

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/parca-dev/proton">GitHub - parca-dev/ proton</a></li>
<li><a href="https://en.wikipedia.org/wiki/Minifloat">Minifloat - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Triton`, `#GPU compiler`, `#deep learning`, `#release`, `#open source`

---

<a id="item-3"></a>
## [Google's reCAPTCHA now performs remote attestation, blocking de-googled Android users](https://reclaimthenet.org/google-broke-recaptcha-for-de-googled-android-users) ⭐️ 8.0/10

Google's new reCAPTCHA effectively performs remote attestation, breaking functionality for de-googled Android users and raising serious privacy concerns. This change impacts users who have chosen to remove Google services from their Android devices, limiting their access to many websites that use reCAPTCHA. It also raises serious privacy concerns as remote attestation can tie device identity to user activity. The new reCAPTCHA uses remote attestation involving a chain of trust from a burned-in private key (EK) to an ephemeral identity key (AIK) signed by Google servers, potentially allowing Google to link device identity across sessions.

hackernews · anonymousiam · May 8, 18:45 · [Discussion](https://news.ycombinator.com/item?id=48067119)

**Background**: Remote attestation is a trusted computing technology where a device proves its integrity to a remote verifier. In this context, Google's reCAPTCHA uses it to ensure the device hasn't been tampered with. De-googled Android refers to devices stripped of Google services, often running custom ROMs. These devices lack necessary proprietary components to pass remote attestation, hence being blocked.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Remote_attestation">Remote attestation</a></li>
<li><a href="https://tech.yahoo.com/phones/articles/googling-android-simpler-think-no-193119747.html">De - Googling Android is simpler than you think—no special phone...</a></li>

</ul>
</details>

**Discussion**: Comments express frustration and concern. Users discuss technical details of remote attestation and seek alternatives to reCAPTCHA. There is sentiment that this move forces KYC and is an overreach.

**Tags**: `#reCAPTCHA`, `#Android`, `#privacy`, `#remote attestation`, `#Google`

---

<a id="item-4"></a>
## [AI Disrupts Two Vulnerability Disclosure Cultures](https://www.jefftk.com/p/ai-is-breaking-two-vulnerability-cultures) ⭐️ 8.0/10

A new analysis argues that AI is accelerating the erosion of traditional vulnerability disclosure norms by enabling faster exploit generation and widening the gap between coordinated disclosure and public exploitation. This shift could fundamentally alter how vulnerabilities are reported and patched, potentially increasing the risk of zero-day exploits and making coordinated disclosure less effective. The analysis is rooted in the Log4Shell incident and discusses how AI tools enable attackers to generate exploits faster than defenders can patch, particularly affecting open-source software with public codebases.

hackernews · speckx · May 8, 17:55 · [Discussion](https://news.ycombinator.com/item?id=48066524)

**Background**: Vulnerability disclosure traditionally follows two main cultures: coordinated disclosure, where researchers privately inform vendors and allow time for patches, and full disclosure, where details are publicly released immediately. The rise of AI and improved software transparency — through open-source adoption and advanced reverse-engineering tools — has blurred this distinction, as attackers can now quickly generate exploits from publicly available patches or commits.

**Discussion**: Commenters largely agree that AI is accelerating existing trends rather than creating a new problem, with tptacek noting the long-predicted impact of software transparency. freeqaz highlights Log4Shell as a key example of exploit generation racing against disclosure. However, rikafurude21 argues that cheaper exploit generation makes coordinated disclosure more important, not less.

**Tags**: `#AI`, `#cybersecurity`, `#vulnerability disclosure`, `#open source`, `#Log4Shell`

---

<a id="item-5"></a>
## [Meta Ends End-to-End Encryption for Instagram DMs](https://www.pcmag.com/news/meta-shuts-down-end-to-end-encryption-for-instagram-dms-messaging) ⭐️ 8.0/10

Meta has discontinued end-to-end encryption for Instagram direct messages, citing low opt-in rates. The company will now store messages unencrypted. This decision raises concerns about user privacy and signals a step backward from industry trends toward stronger encryption. Critics argue that Meta prioritizes access to user data for advertising and compliance over privacy. The encryption feature was opt-in and required users to enable it manually. Meta claims few users chose to turn it on, making the feature unsustainable.

hackernews · tcp_handshaker · May 8, 21:47 · [Discussion](https://news.ycombinator.com/item?id=48069192)

**Background**: End-to-end encryption ensures that only the sender and recipient can read messages, preventing even the service provider from accessing content. Privacy advocates often push for default encryption, as seen in apps like WhatsApp (also owned by Meta) and Signal. Meta's decision contrasts with its earlier promises to roll out encryption across its messaging platforms.

**Discussion**: Comments criticize Meta for not making encryption default, comparing it unfavorably to Signal and WhatsApp. Some argue that Meta's move reflects a broader corporate reluctance to prioritize privacy over business interests, while others express frustration over the lack of progress in protecting user data.

**Tags**: `#privacy`, `#encryption`, `#Instagram`, `#Meta`, `#tech-policy`

---

<a id="item-6"></a>
## [Mojo 1.0 Beta Released: Python-compatible with Rust ownership and Zig comptime](https://mojolang.org/) ⭐️ 8.0/10

Modular Inc. released Mojo 1.0 Beta, a programming language that combines Python syntax with Rust-like ownership and Zig-like comptime, targeting high-performance ML and systems programming. Mojo aims to bridge the gap between high-level usability and low-level performance, potentially enabling Python developers to write efficient systems code without switching languages. Its unique use of MLIR for compiler infrastructure allows it to target CPUs, GPUs, and TPUs from a single codebase. Mojo is currently closed-source with an open-source standard library, but Modular has committed to open-sourcing it in Fall 2026. It supports first-class SIMD, a rich type system, and can interoperate with Python via a foreign function interface.

hackernews · sbt567 · May 8, 02:49 · [Discussion](https://news.ycombinator.com/item?id=48057901)

**Background**: Mojo is built on MLIR (Multi-Level Intermediate Representation), a compiler framework that enables higher-level optimization passes compared to LLVM alone. This allows Mojo to efficiently target diverse hardware including GPUs and TPUs. The ownership model borrows from Rust, ensuring memory safety without garbage collection, while comptime (compile-time execution) from Zig enables powerful metaprogramming.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mojo_(programming_language)">Mojo (programming language)</a></li>
<li><a href="https://zig.guide/language-basics/comptime/">Comptime | zig .guide</a></li>

</ul>
</details>

**Discussion**: Commenters expressed excitement about Mojo's performance and features like ownership and comptime, but noted challenges for Python developers due to syntax differences and limited Python compatibility. Some users also expressed impatience for the planned open-sourcing in 2026.

**Tags**: `#programming language`, `#performance`, `#ML`, `#systems programming`, `#Mojo`

---

<a id="item-7"></a>
## [Luke Curley Criticizes WebRTC's Packet Dropping for LLM Prompts](https://simonwillison.net/2026/May/9/luke-curley/#atom-everything) ⭐️ 8.0/10

Luke Curley argues that WebRTC's design to drop audio packets for low latency harms the accuracy of LLM prompts, and notes that browsers cannot even retransmit lost packets, citing Discord's experience. This highlights a fundamental conflict between real-time communication optimizations and the accuracy requirements of AI models, which could impact the quality of voice-based AI interactions. WebRTC aggressively drops audio packets during poor network conditions to maintain low latency, but this can lead to distorted audio; Curley notes that waiting an extra 200ms would be preferable for accurate LLM prompts.

rss · Simon Willison · May 9, 01:03

**Background**: WebRTC is a standard for real-time communication in browsers, designed for low-latency scenarios like video calls. Large language models (LLMs) process voice prompts and require accurate input, making packet loss problematic.

**Tags**: `#WebRTC`, `#LLM`, `#real-time communication`, `#audio`, `#latency`

---

<a id="item-8"></a>
## [Canvas LMS Hacked by ShinyHunters Disrupts US School Finals](https://www.cnn.com/2026/05/07/us/canvas-hack-strands-college-students-finals-week) ⭐️ 8.0/10

Instructure's Canvas learning management system suffered a ransomware attack and data breach by the ShinyHunters hacking group, causing widespread disruption during US schools' finals week. The attack compromised over 300 TB of data, including student names, IDs, and email addresses, and forced some universities to reschedule exams. This incident highlights the vulnerability of critical educational infrastructure, affecting thousands of schools and millions of students during a high-stakes academic period. It underscores the urgent need for stronger cybersecurity measures in the education technology sector, especially as ransomware groups increasingly target sensitive student data. ShinyHunters claimed responsibility for two incidents against Instructure in May 2026, with the first on May 1 leaking usernames, emails, and student IDs. The second attack on May 7 involved ransomware, rendering Canvas inaccessible for many users, and allegedly affecting nearly 9,000 schools or organizations with over 300 TB of data stolen.

telegram · zaihuapd · May 8, 04:30

**Background**: Canvas is a cloud-based learning management system (LMS) developed by Instructure, widely used in K-12, higher education, and corporate training for course management, quizzes, and student engagement. ShinyHunters is a black-hat criminal hacking group formed around 2019, known for orchestrating multiple data breaches across various industries. The group often exfiltrates data and demands ransom, threatening to leak sensitive information if not paid.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Canvas_LMS">Canvas LMS</a></li>
<li><a href="https://en.wikipedia.org/wiki/ShinyHunters">ShinyHunters - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#data breach`, `#education`, `#ransomware`, `#canvas`

---

<a id="item-9"></a>
## [Cloudflare lays off 1100+, cites 600% AI usage surge as cause](https://blog.cloudflare.com/building-for-the-future/) ⭐️ 8.0/10

Cloudflare announced layoffs of over 1,100 employees globally, attributing the restructuring to a 600% increase in internal AI agent usage across departments within the past three months. This signals a major shift by a key internet infrastructure company toward AI-driven workforce restructuring, potentially influencing broader tech industry employment trends and highlighting the growing displacement of human roles by AI agents. The layoff is a one-time event, with severance including full base salary through end of 2026, U.S. health insurance coverage until year-end, extended equity vesting to August 15, 2026, and cliff waivers for those not yet vested for one year.

telegram · zaihuapd · May 8, 08:15

**Background**: AI agents are autonomous software tools that can perform tasks, make decisions, and interact with environments using data from internal systems and enterprise tools. Companies like Cloudflare are increasingly deploying AI agents across departments such as engineering, HR, finance, and marketing to automate routine work, leading to reduced need for human employees. This trend reflects a broader industry shift where AI adoption is directly impacting workforce size and structure.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/resources/articles/what-are-ai-agents">What are AI agents ? · GitHub</a></li>
<li><a href="https://www.grammarly.com/agentic-ai">What is Agentic AI ? | Agentic AI 101</a></li>

</ul>
</details>

**Tags**: `#Cloudflare`, `#layoffs`, `#AI`, `#restructuring`, `#tech industry`

---

<a id="item-10"></a>
## [Anthropic seeks hundreds of billions in funding, valuation nears $1 trillion](https://www.ft.com/content/a40cafcc-0fa4-4e70-9e24-90d826aea56d) ⭐️ 8.0/10

Anthropic is reportedly planning to raise hundreds of billions of dollars this summer to expand its computing infrastructure, potentially pushing its valuation to nearly $1 trillion and surpassing OpenAI. This funding round would mark a major milestone in the AI industry, signaling a shift in investor confidence from OpenAI to Anthropic and underscoring the escalating capital requirements for frontier AI development. On Forge Global's secondary market, Anthropic's implied valuation has already reached between $1 trillion and $1.2 trillion, above OpenAI's ~$880 billion. Just in February, Anthropic closed a $30 billion round at a $380 billion valuation.

telegram · zaihuapd · May 8, 11:15

**Background**: Anthropic, founded by former OpenAI employees, is a leading AI safety startup competing directly with OpenAI. Private secondary markets like Forge Global allow investors to trade shares of pre-IPO companies, providing a real-time indicator of a startup's perceived value. The rapid valuation surge reflects Anthropic's strong enterprise customer growth and the intense demand for AI compute resources.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/Forge_Global">Forge Global</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Anthropic`, `#funding`, `#valuation`, `#startup`

---

<a id="item-11"></a>
## [US suspects Nvidia chips smuggled to China via Thailand; Alibaba named as end customer](https://www.bloomberg.com/news/articles/2026-05-08/us-said-to-suspect-nvidia-chips-smuggled-to-alibaba-via-thailand) ⭐️ 8.0/10

US prosecutors suspect Thai company OBON Corp. smuggled $2.5 billion worth of Super Micro servers containing advanced Nvidia chips to China, with Alibaba Group identified as one of the end customers. This case highlights ongoing US-China tech tensions and could lead to stricter export controls on Thailand, potentially hindering Thailand's AI development and affecting global supply chains. OBON was involved in creating Thailand's sovereign AI cloud, Siam AI, which holds an Nvidia partner status. Alibaba denies any business relationship with Super Micro or OBON.

telegram · zaihuapd · May 8, 13:23

**Background**: The US has imposed export controls on advanced Nvidia chips to China to prevent their use in military applications. Smuggling routes through third countries like Thailand have become a concern, prompting investigations. Super Micro servers are high-performance computing systems often used in AI and data centers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.supermicro.com/">Supermicro Data Center Server , Blade, Data Storage, AI System</a></li>
<li><a href="https://siam.ai/">Siam ai corporation co., ltd.</a></li>

</ul>
</details>

**Tags**: `#export controls`, `#Nvidia`, `#smuggling`, `#Alibaba`, `#US-China relations`

---

<a id="item-12"></a>
## [DeepSeek Seeks $45B Valuation with State-Backed Funding](https://t.me/zaihuapd/41289) ⭐️ 8.0/10

DeepSeek is reportedly seeking a $45 billion valuation in its first major external funding round, with China's National Integrated Circuit Industry Investment Fund potentially leading the investment. This funding round would mark significant state-backed capital entering China's AI sector, deepening government involvement in core AI companies and signaling strong national support for DeepSeek. This is DeepSeek's first major external fundraising; the company was previously wholly funded by parent hedge fund High-Flyer. The $45 billion valuation would be one of the highest for a Chinese AI startup.

telegram · zaihuapd · May 8, 14:59

**Background**: DeepSeek was founded in July 2023 by Liang Wenfeng, co-founder of High-Flyer. It is known for developing open-weight large language models at a fraction of the cost of rivals like OpenAI, despite facing US chip export restrictions that forced it to use less powerful hardware. The company's R1 model, released in January 2025, shocked the industry with its low training cost and high performance.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek_(Company)">DeepSeek (Company)</a></li>
<li><a href="https://www.deepseek.com/en/">DeepSeek</a></li>

</ul>
</details>

**Tags**: `#AI`, `#funding`, `#DeepSeek`, `#China`, `#semiconductor`

---

<a id="item-13"></a>
## [Apple May End TSMC's Chip Exclusivity, Consider Intel for Some Chips](https://t.me/zaihuapd/41292) ⭐️ 8.0/10

Apple is reportedly considering ending TSMC's 12-year exclusive chip manufacturing deal and may use Intel's 18A process for some low-end chips as early as 2027. This move would diversify Apple's supply chain, reducing its reliance on TSMC, which is currently prioritizing AI chip demand from Nvidia. It also provides a significant boost to Intel's foundry business. Intel's involvement would be limited to manufacturing only, not chip design. Apple's decision is driven by TSMC's capacity constraints due to surging AI chip orders.

telegram · zaihuapd · May 8, 17:18

**Background**: Since 2014, Apple has relied exclusively on TSMC to manufacture its custom A-series and M-series chips. Apple designs its own chips but outsources fabrication. A shift to Intel would be a major change in the semiconductor supply chain, potentially challenging TSMC's dominance.

**Tags**: `#Apple`, `#TSMC`, `#Intel`, `#chip manufacturing`, `#supply chain`

---