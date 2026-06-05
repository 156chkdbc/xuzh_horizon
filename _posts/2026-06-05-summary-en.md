---
layout: default
title: "Horizon Summary: 2026-06-05 (EN)"
date: 2026-06-05
lang: en
---

> From 31 items, 11 important content pieces were selected

---

1. [Meta ships facial recognition on smart glasses](#item-1) ⭐️ 9.0/10
2. [AI Agent Traffic Surpasses Human Traffic for First Time](#item-2) ⭐️ 9.0/10
3. [Cloudflare Acquires VoidZero, Integrates Vite Toolchain into Workers](#item-3) ⭐️ 9.0/10
4. [Anthropic releases open-source AI vulnerability discovery framework](#item-4) ⭐️ 8.0/10
5. [AI enthusiasts vs skeptics: race against time vs entropy](#item-5) ⭐️ 8.0/10
6. [Uber Caps AI Coding Tool Spending to $1,500 per Month](#item-6) ⭐️ 8.0/10
7. [WeChat Enables A2A with Phone Assistants](#item-7) ⭐️ 8.0/10
8. [DeepSeek tops US enterprise software charts on cost](#item-8) ⭐️ 8.0/10
9. [Apple's New Siri to Use Google Data Centers with Nvidia Blackwell B200 Chips](#item-9) ⭐️ 8.0/10
10. [US Bipartisan Bill Proposes Review of Chinese Robots](#item-10) ⭐️ 8.0/10
11. [US DoD ends Anthropic partnership over AI military use restrictions](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Meta ships facial recognition on smart glasses](https://www.buchodi.com/meta-glasses-facial-recognition/) ⭐️ 9.0/10

Meta has shipped facial recognition technology on its smart glasses, enabling real-time identification of people. This feature was previously prohibited by Google Glass terms and has sparked significant debate. This marks a major step in wearable tech integration with biometrics, potentially enabling accessibility for prosopagnosia but also threatening privacy and sparking legal challenges under laws like BIPA. It could set a precedent for always-on facial recognition in consumer devices. The system can identify faces and provide information to the wearer, but community comments highlight concerns about surveillance, legal risks under the Biometric Information Privacy Act, and the desire for offline, privacy-preserving alternatives for accessibility.

hackernews · buchodi · Jun 4, 19:36 · [Discussion](https://news.ycombinator.com/item?id=48403588)

**Background**: Facial recognition technology analyzes facial features to identify individuals from a database. Smart glasses are wearable computers that display information in the user's field of view. Meta's decision to include facial recognition in consumer smart glasses is controversial due to the always-on nature of the device and the potential for non-consensual identification.

**Discussion**: Commenters express mixed views: some desire offline facial recognition for prosopagnosia accessibility, others oppose surveillance and want detection of nearby facial-recognition glasses. Legal concerns under BIPA are also noted, with one commenter predicting lawsuits.

**Tags**: `#facial recognition`, `#smart glasses`, `#privacy`, `#Meta`, `#biometrics`

---

<a id="item-2"></a>
## [AI Agent Traffic Surpasses Human Traffic for First Time](https://www.tomshardware.com/tech-industry/artificial-intelligence/bots-have-now-passed-human-traffic-online-cloudflare-boss-laments-says-agentic-traffic-wasnt-expected-to-eclipse-real-people-until-next-year) ⭐️ 9.0/10

Cloudflare data reveals that AI agent traffic has exceeded human traffic for the first time, accounting for approximately 57.5% of web requests, a milestone that arrived earlier than CEO Matthew Prince's predicted 2027. This shift has major implications for web infrastructure, security, and the role of AI, as agentic AI represents a new paradigm in how the internet is used, affecting website operators, security teams, and internet governance. The data is based on page requests, not total usage time; humans still dominate in time spent. These AI agents differ from traditional crawlers by performing multi-step tasks such as price comparison and customer service.

telegram · zaihuapd · Jun 4, 16:49

**Background**: AI agents are software systems that autonomously pursue goals using tools and reasoning, often indistinguishable from human browsing. Traditional web crawlers index content for search engines, but AI agents retrieve and act on information for generative AI applications. Cloudflare's network traffic data provides a unique vantage point for monitoring such trends.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent - Wikipedia</a></li>
<li><a href="https://www.humansecurity.com/learn/blog/ai-ecosystem-agents-scrapers-crawlers/">Understanding AI Traffic: Agents, Crawlers, and Bots</a></li>

</ul>
</details>

**Tags**: `#AI`, `#network traffic`, `#Cloudflare`, `#web automation`, `#milestone`

---

<a id="item-3"></a>
## [Cloudflare Acquires VoidZero, Integrates Vite Toolchain into Workers](https://www.cloudflare.com/press/press-releases/2026/cloudflare-acquires-voidzero-to-build-the-future-of-the-ai-native-web/) ⭐️ 9.0/10

On June 4, Cloudflare announced the acquisition of VoidZero, the company behind Vite and other JavaScript tooling, and will integrate these tools into its Workers platform with a one-click deployment feature. Cloudflare also pledged a $1 million community fund and committed to keeping all projects open-source under MIT license. This acquisition signals a major push to integrate frontend tooling directly into edge computing platforms, aligning with the rise of AI-powered coding agents. Developers will benefit from a seamless path from local development to global deployment on Cloudflare's network. Vite currently has over 130 million weekly downloads, with Cloudflare's Vite plugin accounting for 13.9 million. The VoidZero team will join Cloudflare and continue to drive the open-source roadmap, including projects like Vite, Rolldown, Oxc, and Vitest.

telegram · zaihuapd · Jun 5, 00:39

**Background**: Vite is a modern frontend build tool that provides fast development server and optimized builds, created by Evan You (also creator of Vue.js). Cloudflare Workers is a serverless edge computing platform that runs JavaScript globally. By integrating Vite's toolchain, Cloudflare aims to streamline the developer experience from code to deployment on its network.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vite">Vite - Wikipedia</a></li>
<li><a href="https://rolldown.rs/">Rolldown</a></li>
<li><a href="https://oxc.rs/">The JavaScript Oxidation Compiler</a></li>

</ul>
</details>

**Discussion**: Community comments express mixed sentiments. Some recall Vue.js creator Evan You's background, while others voice concerns that the acquisition may eventually compromise the open-source nature of these projects. There is skepticism about the promise that 'nothing will change,' and some suggest that this follows a familiar pattern of open-source projects being aquihired.

**Tags**: `#Cloudflare`, `#Vite`, `#Acquisition`, `#Developer Tools`, `#Edge Computing`

---

<a id="item-4"></a>
## [Anthropic releases open-source AI vulnerability discovery framework](https://github.com/anthropics/defending-code-reference-harness) ⭐️ 8.0/10

Anthropic released an open-source framework for AI-powered vulnerability discovery on GitHub, but the repository is not actively maintained and accepts no contributions. This release signals Anthropic's commitment to transparency in AI security, but the unmaintained status may limit its practical use for the community. The framework uses agents that consume roughly 10K uncached input tokens per minute and 2K output tokens per minute, with costs estimated in the hundreds to thousands of dollars depending on the model used.

hackernews · binyu · Jun 4, 20:11 · [Discussion](https://news.ycombinator.com/item?id=48403980)

**Background**: AI-powered vulnerability discovery involves using large language models to automatically find and exploit security flaws in software. Anthropic has been exploring this area with models like Claude Opus and the unreleased Mythos, and has also established coordinated vulnerability disclosure policies.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/coordinated-vulnerability-disclosure">Coordinated vulnerability disclosure for Claude-discovered vulnerabilities \ Anthropic</a></li>
<li><a href="https://www.anthropic.com/glasswing">Project Glasswing: Securing critical software for the AI era \ Anthropic</a></li>

</ul>
</details>

**Discussion**: The community discussed that such frameworks are like 'shop jigs' that users should customize for their own needs. Concerns were raised about high running costs, and a comment noted the repository is from 'Anthropics' not 'Anthropic', causing confusion.

**Tags**: `#AI`, `#security`, `#open-source`, `#vulnerability discovery`, `#Anthropic`

---

<a id="item-5"></a>
## [AI enthusiasts vs skeptics: race against time vs entropy](https://simonwillison.net/2026/Jun/4/ai-enthusiasts-ai-skeptics/#atom-everything) ⭐️ 8.0/10

Charity Majors published an article articulating the tension between AI enthusiasts racing to leverage capability leaps and AI skeptics preserving code quality and trust, both facing existential threats. This highlights a critical organizational challenge in software teams adopting AI, where the lack of feedback loops between the two groups can lead to either missed opportunities or degraded system reliability. Majors notes that the enthusiasts are not wrong about seeing real discontinuous leaps, and skeptics are not wrong about the risks of shipping code faster than engineers can understand it, and recommends designing feedback loops to bridge the gap.

rss · Simon Willison · Jun 4, 23:55

**Tags**: `#AI`, `#software engineering`, `#technology adoption`, `#engineering culture`

---

<a id="item-6"></a>
## [Uber Caps AI Coding Tool Spending to $1,500 per Month](https://simonwillison.net/2026/Jun/3/uber-caps-usage/#atom-everything) ⭐️ 8.0/10

Uber has implemented a $1,500 monthly token spending cap per AI coding tool for all employees, after blowing through its 2026 AI budget in just four months. The limit applies to agentic coding software such as Cursor and Anthropic's Claude Code. This case highlights the real cost challenges enterprises face as AI coding agents—which consume significant tokens per task—gain adoption. The policy also provides a rare glimpse into the per-engineer value companies place on these tools, with spending caps at about 11% of median engineer compensation. The $1,500 cap applies per tool, meaning an engineer using both Cursor and Claude Code could spend up to $3,000 monthly. Uber's policy is a response to overspending on agentic coding tools, which have seen explosive token usage growth in 2026.

rss · Simon Willison · Jun 3, 12:01

**Background**: AI coding agents like Claude Code and Cursor are tools that can autonomously edit code, run commands, and interact with a developer's codebase, often consuming large numbers of API tokens per session. Token usage has become a significant cost for companies adopting these tools, especially as reasoning models and agentic workflows increase consumption. Uber's initial 2026 AI budget was set before the surge in coding agent popularity, leading to rapid overspending.

<details><summary>References</summary>
<ul>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://code.claude.com/docs/en/overview">Overview - Claude Code Docs</a></li>
<li><a href="https://digitaleconomy.stanford.edu/news/how-are-ai-agents-spending-your-tokens/">How are AI agents spending your tokens? - Stanford Digital Economy Lab</a></li>

</ul>
</details>

**Tags**: `#AI`, `#cost management`, `#Claude`, `#Uber`, `#coding agents`

---

<a id="item-7"></a>
## [WeChat Enables A2A with Phone Assistants](https://36kr.com/newsflashes/3838138218662404) ⭐️ 8.0/10

WeChat is partnering with Huawei, Xiaomi, OPPO, vivo, and Honor to launch Agent-to-Agent (A2A) capability, allowing phone voice assistants to initiate WeChat calls and send messages. Some Honor models already support this feature with their YOYO assistant. This marks a significant step in integrating WeChat with smartphone AI assistants, potentially changing how millions of users interact with the super app. It demonstrates a practical application of cross-platform AI agent communication, moving beyond standalone assistants. The A2A protocol allows phone assistants (e.g., Honor's YOYO) to directly command WeChat functions like voice/video calls and messaging. Users need to update both the assistant and WeChat to the latest versions to access the feature.

telegram · zaihuapd · Jun 4, 04:53

**Background**: Agent-to-Agent (A2A) is a communication protocol that enables different AI agents to exchange tasks and data without human intervention. Smartphone voice assistants like Siri or Google Assistant typically operate within their own ecosystems, but A2A allows them to interact with third-party apps like WeChat. This collaboration is one of the first large-scale integrations of its kind in China.

<details><summary>References</summary>
<ul>
<li><a href="https://www.caixinglobal.com/2026-06-04/tencent-opens-wechat-to-handset-makers-ai-assistants-102451051.html">Tencent Opens WeChat to Handset Makers' AI Assistants</a></li>
<li><a href="https://www.yicaiglobal.com/news/tencent-is-working-to-let-phone-ai-assistants-trigger-wechat-calls-messages">Tencent Is Working to Let Phone AI Assistants Trigger WeChat Calls ...</a></li>

</ul>
</details>

**Tags**: `#WeChat`, `#AI agent`, `#voice assistant`, `#smartphone`, `#A2A`

---

<a id="item-8"></a>
## [DeepSeek tops US enterprise software charts on cost](https://www.scmp.com/tech/tech-trends/article/3355927/more-us-firms-turn-chinas-deepseek-over-pricey-silicon-valley-ai) ⭐️ 8.0/10

DeepSeek has topped Ramp's 'Hot Software Vendor' list for June 2025, as more US companies pay directly for its AI services, sending data to servers in China. The company also announced a permanent price reduction for its flagship model V4 Pro. This signals a significant shift in the AI industry, as cost-conscious US enterprises turn to a Chinese AI provider over more expensive Silicon Valley alternatives. It highlights DeepSeek's growing competitiveness and the potential reshaping of global AI market dynamics. The Ramp report, which tracks enterprise spending, placed DeepSeek at number one. DeepSeek is reportedly raising its first round of funding at a valuation near $60 billion, with investors including Tencent and CATL.

telegram · zaihuapd · Jun 4, 10:26

**Background**: DeepSeek is a Chinese AI company founded in 2023, known for developing large language models at a fraction of the cost of US rivals. Its open-weight models and efficient training, using weaker chips due to export restrictions, have disrupted the AI industry.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek</a></li>
<li><a href="https://deepseek.com/en/">DeepSeek</a></li>

</ul>
</details>

**Tags**: `#DeepSeek`, `#AI`, `#enterprise software`, `#cost`, `#China`

---

<a id="item-9"></a>
## [Apple's New Siri to Use Google Data Centers with Nvidia Blackwell B200 Chips](https://www.macrumors.com/2026/06/04/apple-siri-rely-on-google-nvidia-chips/) ⭐️ 8.0/10

Apple plans to have its upcoming Siri, launching in September 2026, use Google data centers and Nvidia Blackwell B200 chips for cloud-based AI processing, abandoning its usual self-developed hardware approach. This marks a major strategic shift for Apple, as it traditionally relies on its own components. It signals Apple's urgency to improve Siri's AI capabilities amid competition, and could reshape cloud AI infrastructure partnerships. Apple's decision reportedly stems from its own servers being too slow to run Google's Gemini models. The Nvidia chips will also encrypt user data for privacy.

telegram · zaihuapd · Jun 4, 11:37

**Background**: Apple Intelligence, launched in 2024, has had lukewarm reception and is not yet available in mainland China. Nvidia's Blackwell B200 is a high-performance GPU for AI workloads, while Google's Gemini is a multimodal LLM. Apple has historically designed its own chips for core functions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Blackwell_(microarchitecture)">Blackwell (microarchitecture) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apple_Intelligence">Apple Intelligence</a></li>
<li><a href="https://www.nvidia.com/en-us/data-center/dgx-b200/">DGX B200: The Foundation for Your AI Factory | NVIDIA</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#Siri`, `#Nvidia`, `#Google`, `#AI`

---

<a id="item-10"></a>
## [US Bipartisan Bill Proposes Review of Chinese Robots](http://chinaselectcommittee.house.gov/media/press-releases/moolenaar-obernolte-mcclellan-introduce-legislation-to-ban-dangerous-chinese-robots) ⭐️ 8.0/10

The US House Select Committee on China introduced the GUARD Act, a bipartisan bill requiring national security review of humanoid and quadruped robots from adversarial nations like China, with potential market restrictions. This bill could significantly alter the US robotics market by limiting access to advanced Chinese robotics, impacting companies like Unitree Robotics that are filing for IPOs, and reflects growing US-China tech decoupling. The bill mandates a one-year review by national security agencies; if incomplete, the FCC automatically adds robots to a 'covered list' restricting market entry. Critics note supporters' ties to US robotics firms and lack of public evidence for security claims.

telegram · zaihuapd · Jun 4, 13:16

**Background**: Quadruped robots imitate four-legged animals and are used in inspection, military, and logistics, while humanoid robots are designed for human environments. The GUARD Act targets such robots from China and other adversaries amid rising US-China technology tensions. The bill also coincides with Unitree Robotics' IPO review in China.

<details><summary>References</summary>
<ul>
<li><a href="https://www.eff.org/deeplinks/2026/05/congress-narrowed-guard-act-serious-problems-remain">Congress Narrowed the GUARD Act , But Serious Problems Remain</a></li>
<li><a href="https://en.wikipedia.org/wiki/Quadruped_(Robotics)">Quadruped (Robotics)</a></li>

</ul>
</details>

**Tags**: `#robotics`, `#regulation`, `#US-China trade`, `#AI`, `#policy`

---

<a id="item-11"></a>
## [US DoD ends Anthropic partnership over AI military use restrictions](https://t.me/zaihuapd/41777) ⭐️ 8.0/10

The US Department of Defense is considering ending its partnership with Anthropic due to disagreements over using Claude AI for military purposes, including weapons development and battlefield operations. Anthropic insists on prohibiting use of Claude for mass surveillance and fully autonomous weapons. This highlights the growing tension between AI safety commitments and military demands, setting a precedent for how major AI companies engage with defense agencies. The outcome could influence future defense contracts and AI ethics policies across the industry. The DoD has adopted a policy requiring 'any lawful use' language in contracts, which conflicts with Anthropic's restrictions. OpenAI and Google have reportedly agreed to relax similar limits, while Anthropic remains firm.

telegram · zaihuapd · Jun 5, 01:27

**Background**: Anthropic, founded by former OpenAI employees, prioritizes AI safety through its 'Constitutional AI' approach. Claude is a large language model designed to be helpful, harmless, and honest. The US military has been increasingly integrating AI, but ethical concerns about autonomous weapons have led to calls for regulation. The DoD's 'any lawful use' policy aims to ensure AI tools are available for all military operations without restrictions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_(language_model)">Claude (language model ) - Wikipedia</a></li>
<li><a href="https://www.brennancenter.org/our-work/research-reports/militarys-use-ai-explained">The Military’s Use of AI, Explained | Brennan Center for Justice</a></li>
<li><a href="https://www.reuters.com/business/ai-contract-restrictions-could-threaten-military-missions-us-official-says-2026-03-03/">AI contract restrictions could threaten military missions, US official says | Reuters</a></li>

</ul>
</details>

**Tags**: `#AI ethics`, `#military AI`, `#Anthropic`, `#Claude`, `#defense policy`

---