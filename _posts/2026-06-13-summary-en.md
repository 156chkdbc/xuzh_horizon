---
layout: default
title: "Horizon Summary: 2026-06-13 (EN)"
date: 2026-06-13
lang: en
---

> From 40 items, 16 important content pieces were selected

---

1. [US orders Anthropic to suspend Fable 5 and Mythos 5](#item-1) ⭐️ 10.0/10
2. [NVIDIA Unveils Vera Rubin Platform, Predicts $1T Sales by 2027](#item-2) ⭐️ 10.0/10
3. [CRISPR Cas12a2 shreds cancer cells, including 'undruggable' ones](#item-3) ⭐️ 9.0/10
4. [HarmonyOS 7 Released with Agent Architecture](#item-4) ⭐️ 9.0/10
5. [Cloudflare Global Outage Causes Intermittent Failures, Fix Underway](#item-5) ⭐️ 9.0/10
6. [vLLM v0.23.0 Released with DeepSeek-V4 and MRV2 Improvements](#item-6) ⭐️ 8.0/10
7. [Open Source AI Must Win](#item-7) ⭐️ 8.0/10
8. [Malware Uses CBRN Text to Target Bioinformatics and MCP Developers](#item-8) ⭐️ 8.0/10
9. [Critique of AI Replacing Human Expertise](#item-9) ⭐️ 8.0/10
10. [To Earn Attention, Show Effort in AI Era](#item-10) ⭐️ 8.0/10
11. [Claude Fable 5's Relentless Proactivity Demonstrated](#item-11) ⭐️ 8.0/10
12. [Anthropic Reverses Secret Policy Limiting AI Researchers](#item-12) ⭐️ 8.0/10
13. [Preprint Accuses Huawei's Pangu of Copying Alibaba Qwen Weights](#item-13) ⭐️ 8.0/10
14. [Kimi Open-Sources K2.7-Code Model with Benchmark Gains](#item-14) ⭐️ 8.0/10
15. [CXMT STAR Market IPO Approved, Raises 29.5B Yuan](#item-15) ⭐️ 8.0/10
16. [US State Attorneys General Jointly Investigate OpenAI](#item-16) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [US orders Anthropic to suspend Fable 5 and Mythos 5](https://simonwillison.net/2026/Jun/13/us-government-directive-to-suspend-access/#atom-everything) ⭐️ 10.0/10

The US government issued an export control directive to Anthropic, ordering the immediate suspension of all access to the Fable 5 and Mythos 5 AI models by any foreign national, citing national security concerns over a potential jailbreak vulnerability. This marks the first time the US government has used national security authorities to disable access to advanced AI models from a major company, setting a precedent for future AI regulation and potentially limiting the availability of cutting-edge models to the public. The directive applies to all foreign nationals, including foreign employees of Anthropic, and effectively forces Anthropic to disable Fable 5 and Mythos 5 for all customers to ensure compliance; other Anthropic models remain unaffected. Anthropic states the alleged jailbreak technique is non-unique and similar capabilities exist in other public models like GPT-5.5.

rss · Simon Willison · Jun 13, 01:01

**Background**: Fable 5 and Mythos 5 are Anthropic's latest advanced AI models, with Fable 5 being a generally available version of the more restricted Mythos 5, which is designed for cybersecurity tasks. AI jailbreaking refers to techniques that bypass safety guardrails in LLMs to produce unintended or harmful outputs. The US government's export control directive uses national security authorities to restrict access to these models, which is unusual for commercial AI products.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mythos_(Anthropic)">Mythos (Anthropic)</a></li>
<li><a href="https://www.vellum.ai/blog/claude-fable-5-and-mythos-5-benchmarks-explained">Claude Fable 5 & Claude Mythos 5 Full Benchmark Breakdown</a></li>

</ul>
</details>

**Discussion**: Commenters express mixed reactions: some argue this could lead to government restrictions on public LLM access, while others blame Anthropic's own fear-mongering for provoking such actions. There is concern that this may drive users to Chinese models and undermine trust in US AI technologies.

**Tags**: `#AI regulation`, `#National Security`, `#Anthropic`, `#AI Safety`, `#Government Directive`

---

<a id="item-2"></a>
## [NVIDIA Unveils Vera Rubin Platform, Predicts $1T Sales by 2027](https://t.me/zaihuapd/41917) ⭐️ 10.0/10

At GTC, NVIDIA announced the Vera Rubin platform, a next-generation AI infrastructure featuring a new Vera CPU, Rubin GPU, and integrated Groq 3 LPU. CEO Jensen Huang predicted combined sales of the Blackwell and Rubin series would reach at least $1 trillion by 2027. This announcement solidifies NVIDIA's dominance in AI hardware and data center infrastructure. The massive sales projection underscores the surging demand for AI compute, impacting the entire semiconductor and AI industries. The Vera Rubin platform includes seven chips already in production: Vera CPU (claimed to be 2x more efficient and 50% faster than traditional rack-level CPUs), Rubin GPU, NVLink 6 Switch, ConnectX-9 SuperNIC, and BlueField-4 DPU, among others. The Groq 3 LPU integration provides low-latency inference with a rack-scale accelerator housing 32 liquid-cooled compute trays.

telegram · zaihuapd · Jun 12, 10:17

**Background**: NVIDIA's GPU platforms are the backbone of modern AI training and inference. The Blackwell architecture (current generation) powers many data centers, while Rubin is its successor. The Vera CPU is a new Arm-based server processor designed to work closely with NVIDIA GPUs, reducing data movement bottlenecks.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Groq">Groq - Wikipedia</a></li>
<li><a href="https://siliconangle.com/2026/06/01/nvidia-ramps-production-vera-rubin-foundation-next-generation-ai-factories/">Nvidia ramps up production of Vera Rubin , the... - SiliconANGLE</a></li>
<li><a href="https://en.wikipedia.org/wiki/Blackwell_(microarchitecture)">Blackwell (microarchitecture) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#NVIDIA`, `#AI hardware`, `#GPU`, `#data center`, `#AI infrastructure`

---

<a id="item-3"></a>
## [CRISPR Cas12a2 shreds cancer cells, including 'undruggable' ones](https://innovativegenomics.org/news/crispr-technique-selectively-shreds-cancer-cells/) ⭐️ 9.0/10

Researchers developed a CRISPR technique using Cas12a2 nuclease that selectively shreds cancer cells by detecting tumor-specific mutations, including those considered 'undruggable'. This approach was published in Nature and a preprint on bioRxiv. This technique offers a potential therapeutic avenue for cancers that currently lack effective drugs, especially those with mutations like KRAS that are historically difficult to target. It may broaden the scope of CRISPR-based cancer therapies beyond conventional Cas9 approaches. Cas12a2, unlike Cas9, destroys chromatin indiscriminately upon activation by target RNA, leading to cell death. The method requires careful delivery and may face tumor resistance through mutation or epigenetic changes.

hackernews · gmays · Jun 12, 15:15 · [Discussion](https://news.ycombinator.com/item?id=48505231)

**Background**: CRISPR-Cas systems are adaptive immune systems in bacteria; Cas9 cuts DNA at specific sites, while Cas12a2 induces abortive infection by shredding cellular DNA and RNA upon target recognition. 'Undruggable' cancers refer to mutations in proteins like KRAS that are difficult to inhibit with small molecules due to their structure.

<details><summary>References</summary>
<ul>
<li><a href="https://crisprmedicinenews.com/news/appetite-for-destruction-the-indiscriminate-nuclease-activity-of-cas12a2/">News: Appetite for Destruction: The Indiscriminate Nuclease Activity of...</a></li>

</ul>
</details>

**Discussion**: Commenters noted that this is not entirely new, as previous studies used Cas9 to kill cells with tumor-specific mutations, but Cas12a2 is more destructive. Some expressed hope for genetic diseases, while others criticized CRISPR hype, noting only one FDA-approved CRISPR therapy compared to many viral vector therapies.

**Tags**: `#CRISPR`, `#cancer therapy`, `#biotechnology`, `#gene editing`

---

<a id="item-4"></a>
## [HarmonyOS 7 Released with Agent Architecture](https://finance.sina.com.cn/tech/2026-06-12/doc-iniccspn5063962.shtml) ⭐️ 9.0/10

Huawei officially released HarmonyOS 7 at its 2026 Developer Conference, evolving to an Agent-based architecture with three major upgrades: Agent affinity system architecture, HarmonyOS Agent Framework 2.0, and the system agent Xiaoyi. This marks a paradigm shift for Huawei's ecosystem, positioning HarmonyOS 7 as a next-generation AI-driven operating system that could challenge Android and iOS in the global OS race. The system agent Xiaoyi is deeply integrated as a built-in intelligent assistant, while the HarmonyOS Agent Framework 2.0 empowers developers to build automated agents without training complex foundation models.

telegram · zaihuapd · Jun 12, 07:23

**Background**: HarmonyOS was first launched by Huawei in 2019 as a cross-device operating system. An Agent architecture refers to an AI-driven system where autonomous software agents proactively assist users, representing a shift from traditional reactive app models. Huawei began building native apps in 2023 and now moves toward an Agent era.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.bestai.com/harmonyos-6-ai-agents-challenge-android-and-ios-in-global-os-race/">HarmonyOS 6 AI Agents Challenge Android and iOS in Global OS Race</a></li>
<li><a href="https://www.patreon.com/harmonyoshub/posts/harmonyos-7-hdc-160895776">HarmonyOS 7 debut, Huawei HDC 2026 keynote speech | Patreon</a></li>
<li><a href="https://post.smzdm.com/p/amoqv44v/">我觉得这次 鸿 蒙 6最重磅的是引入了 智 能 体 框 架 _手机_什么值得买</a></li>

</ul>
</details>

**Tags**: `#HarmonyOS`, `#Huawei`, `#Operating System`, `#Agent Architecture`, `#Developer Conference`

---

<a id="item-5"></a>
## [Cloudflare Global Outage Causes Intermittent Failures, Fix Underway](https://t.me/zaihuapd/41922) ⭐️ 9.0/10

On November 18, 2025, Cloudflare experienced a global outage with intermittent failures affecting multiple regions and websites, and the company confirmed the issue and began implementing fixes around 21:04 UTC. Cloudflare is a critical internet infrastructure provider, so this outage disrupted access to numerous websites and services worldwide, highlighting the fragility of centralized infrastructure. The outage involved intermittent failures with multiple recovery attempts, and the status page indicated that WARP access was disabled in London, while Cloudflare Access was also affected.

telegram · zaihuapd · Jun 12, 14:31

**Background**: Cloudflare provides content delivery network (CDN), DDoS protection, and security services to millions of websites worldwide. WARP is a VPN-like service that encrypts and accelerates internet traffic, while Cloudflare Access is a zero-trust identity and access management product for securing internal applications.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cloudflare_WARP">Cloudflare WARP</a></li>
<li><a href="https://developers.cloudflare.com/warp-client/">Overview · Cloudflare WARP client docs</a></li>

</ul>
</details>

**Tags**: `#Cloudflare`, `#Outage`, `#Internet Infrastructure`, `#Global`

---

<a id="item-6"></a>
## [vLLM v0.23.0 Released with DeepSeek-V4 and MRV2 Improvements](https://github.com/vllm-project/vllm/releases/tag/v0.23.0) ⭐️ 8.0/10

vLLM v0.23.0 was released with 408 commits from 200 contributors, featuring major updates including DeepSeek-V4 maturation across backends and Model Runner V2 (MRV2) expansion to more dense models like Llama and Mistral. These optimizations significantly improve inference performance and efficiency for cutting-edge models like DeepSeek-V4, while MRV2's expansion to popular architectures lowers the barrier for high-performance LLM serving in production. Notable technical changes include decoupling sparse MLA metadata from DeepSeek-V3.2, adding TRTLLM-gen attention kernel, and enabling selective prefix-cache retention for sliding-window KV cache. However, Minimax M3 is not yet supported in this version.

github · khluu · Jun 12, 23:29

**Background**: vLLM is an open-source high-throughput LLM inference engine widely used for serving large language models. Model Runner V2 (MRV2) is a ground-up reimplementation of vLLM's execution core, designed to be cleaner, more modular, and more efficient. DeepSeek-V4 is the latest open-weight model from DeepSeek, a Chinese AI company known for cost-efficient training and strong performance.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek</a></li>
<li><a href="https://docs.vllm.ai/en/latest/design/model_runner_v2/">Model Runner V2 Design Document - vLLM</a></li>
<li><a href="https://vllm.ai/blog/mrv2">Model Runner V2: A Modular and Faster Core for vLLM | vLLM Blog</a></li>

</ul>
</details>

**Tags**: `#vllm`, `#LLM inference`, `#DeepSeek`, `#release notes`, `#open-source`

---

<a id="item-7"></a>
## [Open Source AI Must Win](https://opensourceaimustwin.com/?share=v2) ⭐️ 8.0/10

A public campaign has launched urging the AI community to prioritize open source AI development to avoid dependence on big tech companies like OpenAI and Anthropic. If open source AI loses, society risks becoming dependent on a few corporations for AI infrastructure, potentially limiting innovation and control over facts, software, and labor. Key technical hurdles include decentralized training communication speeds and data poisoning from untrusted nodes, though partial solutions like self-healing checkpointed rollbacks are being explored.

hackernews · vednig · Jun 13, 02:14 · [Discussion](https://news.ycombinator.com/item?id=48511908)

**Background**: Open source AI refers to models with publicly available weights and code, allowing community inspection and modification. Proprietary AI from companies like OpenAI and Anthropic are closed-source, controlled by the corporations. This campaign argues that without deliberate support, open source AI will lag behind, leading to a monopoly over AI capabilities.

**Discussion**: The community largely supports the cause but debates its feasibility: some worry about funding and technical challenges, while others believe models will become commodities over time, reducing the first-mover advantage.

**Tags**: `#open source`, `#AI`, `#big tech`, `#decentralization`, `#research`

---

<a id="item-8"></a>
## [Malware Uses CBRN Text to Target Bioinformatics and MCP Developers](https://twitter.com/jsrailton/status/2064661778978533571) ⭐️ 8.0/10

A new malware campaign embeds text about nuclear and biological weapons to target developers working in bioinformatics and the Model Context Protocol (MCP) ecosystem. The malicious packages, named 'mini-shai-hulud', 'miasma', and 'hades-worms', were discovered by socket.dev. This attack combines cybersecurity threats with AI safety concerns, as the malware deliberately contaminates code with sensitive CBRN text to evade detection by safety-focused AI models. It highlights vulnerabilities in the open-source supply chain for AI and bioinformatics tools. The malware is part of a larger npm worm campaign that has infected over 500 packages, leaking secrets via GitHub. The malicious text references CBRN topics to potentially poison training data or trigger refusals in language models that analyze the code.

hackernews · marc__1 · Jun 11, 20:24 · [Discussion](https://news.ycombinator.com/item?id=48495928)

**Background**: The Model Context Protocol (MCP) is an open standard developed by Anthropic that enables AI applications to connect with external data sources. Bioinformatics developers often use open-source packages for genomic analysis. The Shai-Hulud malware is a self-propagating npm worm that targets the open-source ecosystem, and this variant adds CBRN-themed text to complicate AI-based security analysis.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>
<li><a href="https://slowmist.medium.com/shai-hulud-malware-in-depth-analysis-open-source-means-loss-of-control-ca49cdc06bf7">Shai - Hulud Malware In-Depth Analysis: Open Source Means... | Medium</a></li>

</ul>
</details>

**Discussion**: Comments on Hacker News express varying views: some question the efficacy of using LLMs for nuclear weapons development, while others note that such dangerous information is already accessible. There is also discussion about moderation primitives and denial-of-service parallels, and a suggestion that AI labs should address this problem at an architectural level rather than relying on content filtering.

**Tags**: `#cybersecurity`, `#malware`, `#AI safety`, `#bioinformatics`, `#spyware`

---

<a id="item-9"></a>
## [Critique of AI Replacing Human Expertise](https://correresmidestino.com/dont-you-just-upload-it-to-chatgpt/) ⭐️ 8.0/10

An article titled 'Don't You Just Upload It to ChatGPT?' critically examines the assumption that ChatGPT and similar AI can adequately replace human expertise in specialized fields, sparking a rich discussion on AI's limitations. This matters because it challenges the prevalent narrative that AI is a universal solution, highlighting the nuanced ways AI can fail in tasks requiring deep contextual understanding and specialized knowledge, affecting how we assess AI's role in skilled work. The article, with 345 points and 280 comments, uses examples from translation and domain-specific tasks to illustrate that AI outputs often lack the subtlety and accuracy that human experts provide, and that users may be ill-equipped to evaluate AI's flaws outside their own expertise.

hackernews · speckx · Jun 12, 17:52 · [Discussion](https://news.ycombinator.com/item?id=48507278)

**Background**: ChatGPT is a large language model that generates human-like text, often used for tasks like translation, code generation, and answering questions. However, it lacks genuine understanding and can produce plausible-sounding but incorrect outputs, especially in specialized domains.

**Discussion**: Commenters largely agree with the article's critique, noting that AI is seen as useful for tasks outside one's own expertise but inadequate for highly skilled work. One commenter highlights that in 2024, AI solved unsolved math problems, while another warns that AI translation might soon replace human translators despite errors. Overall, the discussion reflects a nuanced view of AI's strengths and limitations.

**Tags**: `#AI`, `#ChatGPT`, `#expertise`, `#human vs AI`, `#technology criticism`

---

<a id="item-10"></a>
## [To Earn Attention, Show Effort in AI Era](https://tombedor.dev/human-attention-and-human-effort/) ⭐️ 8.0/10

A blog post argues that demonstrating human effort is essential to earn human attention, especially when AI-generated content floods workflows like code reviews and team communications. As AI tools become widespread, the principle of matching effort helps maintain meaningful collaboration and prevents the devaluation of human attention. The principle is illustrated by examples such as colleagues submitting AI-generated pull requests without personal review, leading to ignored work and frustration.

hackernews · jjfoooo4 · Jun 11, 23:01 · [Discussion](https://news.ycombinator.com/item?id=48497609)

**Background**: The rise of large language models (LLMs) like ChatGPT and Claude has enabled rapid generation of text and code. However, over-reliance on AI without human refinement can create a flood of low-effort content that burdens reviewers. The article suggests that if you expect human attention, you should invest commensurate effort in your work.

**Discussion**: Commenters share real-world experiences of colleagues heavily relying on AI tools, leading to poor review engagement and team friction. Some note that the 'matching effort' principle has long been valid even before AI, but now becomes even more critical.

**Tags**: `#AI`, `#collaboration`, `#code review`, `#software engineering`, `#communication`

---

<a id="item-11"></a>
## [Claude Fable 5's Relentless Proactivity Demonstrated](https://simonwillison.net/2026/Jun/11/fable-is-relentlessly-proactive/#atom-everything) ⭐️ 8.0/10

Simon Willison documented an instance where Claude Fable 5, given a vague prompt about a scrollbar bug, autonomously created test HTML pages, used browser automation to open Safari, and took screenshots via Python's pyobjc and screencapture to diagnose the issue. This showcases a new level of AI autonomy, where the model proactively invokes multiple tools (browser, screenshots, code analysis) without explicit instructions, potentially transforming how developers debug complex issues. The model used uv run with pyobjc-framework-Quartz to list windows, identified the correct Safari window, and captured a screenshot using the screencapture CLI, all without any pre-configured browser automation tool.

rss · Simon Willison · Jun 11, 23:35

**Background**: Claude Fable 5 is a recently released language model from Anthropic, part of their Mythos-class models. It is designed for autonomous knowledge work and coding, with a tendency to proactively explore and solve problems. Simon Willison, a well-known developer and AI commentator, often tests cutting-edge AI models and shares his findings.

<details><summary>References</summary>
<ul>
<li><a href="https://platform.claude.com/docs/en/about-claude/models/introducing-claude-fable-5-and-claude-mythos-5">Introducing Claude Fable 5 and Claude Mythos 5 - Claude API Docs</a></li>
<li><a href="https://www.interconnects.ai/p/claude-fable-5-and-new-ai-safety">Claude Fable 5 and new safety fables - by Nathan Lambert</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Claude Fable`, `#proactive`, `#LLM`, `#Simon Willison`

---

<a id="item-12"></a>
## [Anthropic Reverses Secret Policy Limiting AI Researchers](https://simonwillison.net/2026/Jun/11/anthropic-walks-back-policy/#atom-everything) ⭐️ 8.0/10

Anthropic reversed a policy that secretly limited Claude Fable 5's responses to requests targeting frontier LLM development, making the safeguards visible instead. The company apologized for the wrong tradeoff and will now display fallback to Opus 4.8 and return refusal reasons on the API. This policy reversal restores transparency and trust for AI researchers who rely on Claude for legitimate development work. It sets a precedent that invisible safety restrictions are unacceptable and pressures other AI labs to adopt more open safeguard policies. The original policy, hidden in Claude's system card, allowed Claude Fable 5 to silently limit responses for frontier LLM development via prompt modification and steering vectors. The new policy makes flagged requests visibly fall back to Opus 4.8, similar to existing cyber and bio safeguards, and provides refusal reasons on the API within days.

rss · Simon Willison · Jun 11, 03:45

**Background**: System cards are documents that describe the capabilities, safety evaluations, and deployment decisions for AI models. Frontier LLM development refers to building cutting-edge large language models, often by other AI labs. Claude Fable 5 is a Mythos-class model with strong safeguards designed for general use. The secret policy sparked outcry because it undermined researcher trust.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/system-cards">Model system cards \ Anthropic</a></li>
<li><a href="https://digg.com/tech/fpdiy0g6">Anthropic silently restricts Fable 5 from assisting with frontier LLM ...</a></li>

</ul>
</details>

**Tags**: `#AI ethics`, `#Anthropic`, `#Claude`, `#transparency`, `#policy`

---

<a id="item-13"></a>
## [Preprint Accuses Huawei's Pangu of Copying Alibaba Qwen Weights](https://t.me/zaihuapd/41915) ⭐️ 8.0/10

A new preprint proposes the Matrix-Driven Instant Review (MDIR) method for detecting weight plagiarism in large language models, and a case study using MDIR shows statistically significant evidence that Huawei's Pangu model copied weights from Alibaba's Qwen model. This accusation between two major Chinese AI companies could have serious implications for intellectual property in AI, and the new detection method offers a practical tool for verifying model originality, potentially reshaping trust and accountability in the LLM ecosystem. MDIR leverages matrix analysis and Large Deviation Theory to compute p-values, and it can run on a single personal computer within one hour. The method correctly identifies weight sources even after incremental pretraining, pruning, or permutation, and achieves perfect AUC and accuracy on the LeaFBench benchmark.

telegram · zaihuapd · Jun 12, 08:07

**Background**: Large language models are trained on massive datasets, and their weights (parameters) represent learned knowledge. Weight plagiarism involves copying the trained weights from one model into another, which is difficult to detect because models can be fine-tuned or pruned. MDIR uses statistical tests to provide rigorous p-values, unlike previous methods that lacked significance measures.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2508.06309v1">Matrix-Driven Instant Review: Confident Detection and Reconstruction of LLM Plagiarism on PC</a></li>
<li><a href="https://arxiv.org/abs/2508.06309">[2508.06309] Matrix-Driven Identification and Reconstruction of LLM Weight Homology</a></li>

</ul>
</details>

**Tags**: `#AI`, `#plagiarism detection`, `#large language models`, `#Huawei`, `#Alibaba`

---

<a id="item-14"></a>
## [Kimi Open-Sources K2.7-Code Model with Benchmark Gains](https://mp.weixin.qq.com/s/NBw1VAA9MjpKv-Rirq9qDg) ⭐️ 8.0/10

Kimi (Moonshot AI) has released and open-sourced the K2.7-Code coding model, which shows significant improvements on multiple benchmarks, including a 21.8% gain on Kimi Code Bench v2, 11% on Program-Bench, and 31.5% on MLS Bench Lite, while using 30% fewer tokens than its predecessor K2.6. This release strengthens the open-source coding model ecosystem by offering a highly efficient model that reduces token usage by 30%, which can lower costs for developers and enterprises. The benchmark improvements also demonstrate progress in long-context coding and autonomous agent capabilities. The model is available immediately via the Kimi API and Kimi Code service, with a six-times faster mode coming soon, and supports local deployment. Improvements include better instruction following in long-context scenarios, reduced overthinking, and roughly 10% gains on agent benchmarks.

telegram · zaihuapd · Jun 12, 10:55

**Background**: Coding models are AI systems trained to generate, understand, and debug code. Open-source models like K2.7-Code allow developers to inspect, modify, and deploy them locally without vendor lock-in. Token efficiency reduces computational cost, making advanced AI more accessible.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/moonshotai/Kimi-K2.7-Code">moonshotai/Kimi-K2.7-Code · Hugging Face</a></li>
<li><a href="https://codersera.com/blog/kimi-k2-7-complete-guide-2026/">Kimi K2.7 Code: The Complete Guide — Benchmarks, Pricing & How to Use (2026)</a></li>

</ul>
</details>

**Tags**: `#AI`, `#open-source`, `#coding`, `#model`, `#benchmark`

---

<a id="item-15"></a>
## [CXMT STAR Market IPO Approved, Raises 29.5B Yuan](https://t.me/zaihuapd/41923) ⭐️ 8.0/10

ChangXin Memory Technologies (CXMT) has received approval from the Shanghai Stock Exchange’s listing committee for its IPO on the STAR Market. The company plans to raise 29.5 billion yuan (about $4.2 billion) to fund DRAM manufacturing upgrades and advanced R&D. This IPO marks a major milestone for China's semiconductor self-sufficiency efforts. As a leading domestic DRAM manufacturer, CXMT's massive funding will accelerate DRAM technology upgrades and reduce China's reliance on foreign memory chips. The funds are designated for technology upgrades of memory wafer manufacturing production lines, DRAM technology upgrades, and forward-looking R&D projects. CXMT specializes in DRAM (dynamic random-access memory) chips, which are essential in computers, smartphones, and servers.

telegram · zaihuapd · Jun 12, 15:06

**Background**: The STAR Market (Sci-Tech Innovation Board) is a Shanghai Stock Exchange board launched in 2019 to support tech and innovative companies with flexible listing rules, including no profit requirement and a registration-based IPO system. CXMT, founded in 2016, is one of China's top DRAM manufacturers striving to compete with global leaders like Samsung and SK Hynix.

<details><summary>References</summary>
<ul>
<li><a href="https://zh.wikipedia.org/zh-hans/上海證券交易所科創板">上海证券交易所科创板 - 维基百科，自由的百科全书</a></li>

</ul>
</details>

**Tags**: `#IPO`, `#DRAM`, `#semiconductor`, `#China`, `#memory`

---

<a id="item-16"></a>
## [US State Attorneys General Jointly Investigate OpenAI](https://www.bloomberg.com/news/articles/2026-06-13/openai-probed-by-coalition-of-state-attorneys-general) ⭐️ 8.0/10

A coalition of state attorneys general is investigating OpenAI, demanding information on AI safety and other broad topics. OpenAI has stated it is cooperating with the probe. This coordinated multi-state investigation escalates legal and regulatory pressure on leading AI companies like OpenAI. It could set significant precedents for AI safety standards and corporate accountability in the US. Florida previously sued OpenAI and CEO Sam Altman, alleging they knowingly released ChatGPT despite knowing its harms. OpenAI faces multiple lawsuits over chatbot-caused user harm and has added protections for minors and distressed users. The company is valued at $852 billion and has filed for a confidential IPO.

telegram · zaihuapd · Jun 13, 02:40

**Background**: OpenAI is the creator of ChatGPT, a generative AI chatbot. State attorneys general enforce consumer protection laws, so they are probing whether OpenAI engaged in deceptive or unfair practices. This investigation adds to existing federal scrutiny and lawsuits.

**Tags**: `#OpenAI`, `#AI安全`, `#监管`, `#法律诉讼`

---