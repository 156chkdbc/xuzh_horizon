---
layout: default
title: "Horizon Summary: 2026-08-05 (EN)"
date: 2026-08-05
lang: en
---

> From 39 items, 12 important content pieces were selected

---

1. [Keyv and Related npm Packages Hit by Shai-Hulud Supply Chain Attack](#item-1) ⭐️ 9.0/10
2. [Huawei unveils Tau Scaling Law, proposing time scaling to replace geometric scaling in chips](#item-2) ⭐️ 9.0/10
3. [Gwern Retires from Pseudonymous Writing to Launch Guardian Angel AI](#item-3) ⭐️ 8.0/10
4. [Mistral Releases Shieldstral, a 3B Open-Weights Multimodal Moderation Model](#item-4) ⭐️ 8.0/10
5. [Custom color space and algorithm for diverse skin tone generation](#item-5) ⭐️ 8.0/10
6. [Waymo Opens Driverless Ride-Hailing to Everyone in Dallas](#item-6) ⭐️ 8.0/10
7. [Oxide Computer raises $445M (SEC Form D)](#item-7) ⭐️ 8.0/10
8. [LLM 0.32 Adds Reasoning Traces, Server-Side Tools, and OpenAI Responses Support](#item-8) ⭐️ 8.0/10
9. [MiniMax-H3 Omni-Modal Model Gets MLX Port for Apple Silicon](#item-9) ⭐️ 8.0/10
10. [Cloudflare replaces third-party security tools with $58/month AI for bug bounties](#item-10) ⭐️ 8.0/10
11. [Google Builds $200B Wall Street Financing Machine for Anthropic AI Chips](#item-11) ⭐️ 8.0/10
12. [China's First Mandatory L3/L4 Autonomous Driving Safety Standard Heads to Public Comment](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Keyv and Related npm Packages Hit by Shai-Hulud Supply Chain Attack](https://www.aikido.dev/blog/keyv-and-friends-compromised-in-npm-supply-chain-attack) ⭐️ 9.0/10

JFrog security researchers identified a new wave of the Shai-Hulud worm spreading through compromised npm packages, starting with keyv and cacheable. The worm harvests credentials, publishes itself to other writable npm packages, and plants execution hooks in GitHub repositories. Keyv is a popular key-value storage library with 1,703 downstream projects, so a compromise can cascade widely through the npm ecosystem. This attack underscores how pre-install hooks turn ordinary package installs into a dangerous supply chain vector. According to JFrog, the worm steals developer credentials, self-publishes to every writable npm package it can access, and plants hooks in GitHub repositories. Notably, setting the LANG environment variable to ru_RU does not stop the spreading mechanism, so this variant behaves differently from earlier Shai-Hulud versions.

hackernews · cimi_ · Aug 4, 11:01 · [Discussion](https://news.ycombinator.com/item?id=49166874)

**Background**: Shai-Hulud is a supply chain worm family that previously compromised hundreds of npm packages by harvesting developer credentials and abusing npm automation. It spreads through lifecycle scripts such as pre-install hooks that run automatically when packages are installed, which is why they are now a focus of security scrutiny. Keyv is a simple key-value store that works with multiple backends, making it a common dependency for Node.js projects.

<details><summary>References</summary>
<ul>
<li><a href="https://research.jfrog.com/post/shai-hulud-is-back-august/">Major Shai Hulud campaign strikes npm again, affecting keyv and 400+ packages - JFrog Security Research</a></li>
<li><a href="https://www.npmjs.com/package/keyv">keyv - npm</a></li>
<li><a href="https://www.securityweek.com/shai-hulud-supply-chain-attack-worm-used-to-steal-secrets-180-npm-packages-hit/">Shai - Hulud Supply Chain Attack : Worm Used to... - SecurityWeek</a></li>

</ul>
</details>

**Discussion**: Developers in the discussion broadly agree that pre-install and post-install hooks should be restricted or removed, with one commenter calling for a moratorium on new ones. Others shared mitigation tools such as Packj and Antimiasma, while some recommended using devcontainers to isolate environments from worm behavior.

**Tags**: `#security`, `#npm`, `#supply-chain`, `#malware`, `#open-source`

---

<a id="item-2"></a>
## [Huawei unveils Tau Scaling Law, proposing time scaling to replace geometric scaling in chips](https://t.me/zaihuapd/42966) ⭐️ 9.0/10

At ISCAS 2026 in Shanghai, Huawei executives presented the Tau (τ) Scaling Law, which replaces traditional geometric scaling with time (τ) scaling as a guiding principle for semiconductor evolution. Huawei stated it has already designed and mass-produced 381 chips based on this law and will release a new Kirin smartphone chip using logic folding this autumn. This is reportedly the first time a Chinese company has proposed an industry-level evolution principle in the global semiconductor field, potentially reshaping industry discourse in the post-Moore era. If the 2031 target is met — transistor density equivalent to a 1.4nm process — it could offer an alternative path for chip advancement beyond traditional process miniaturization. The Tau Scaling Law focuses on systematically reducing the time constant τ to compress signal propagation delays, using techniques such as logic folding. Logic folding restructures the logic circuits within a single chip into layered arrangements rather than stacking multiple chips, and Huawei plans to promote the law through open collaboration.

telegram · zaihuapd · Aug 4, 08:04

**Background**: Moore's Law predicted that transistors on integrated circuits would double roughly every two years via geometric scaling — making transistors smaller and packing them more densely. As this approaches physical limits, new scaling paradigms are needed. The Tau Scaling Law shifts optimization from transistor sizes to time-domain compression, aiming to continue performance gains without relying solely on more advanced manufacturing nodes.

<details><summary>References</summary>
<ul>
<li><a href="https://www.huawei.com/en/news/2026/5/ieee-iscas-tau-scaling">HUAWEI Presents the Tau (τ) Scaling Law, Enabling ...</a></li>
<li><a href="https://www.guancha.cn/economy/2026_05_25_818264.shtml">华为何庭波：今年麒麟芯片首次实施逻辑折叠技术，性能将大幅提升</a></li>
<li><a href="https://www.zhihu.com/question/2042194731078247407/answer/2042243939521058797">华为麒麟 2026 手机芯片今秋面世，率先采用逻辑折叠技术，这是一项怎样的技术？用户能感受到什么变化？ - 现实主义理想者 的回答</a></li>

</ul>
</details>

**Discussion**: Initial community discussion on platforms like Zhihu focuses on how logic folding works, with some analysts emphasizing that it is a novel circuit-architecture approach rather than traditional 3D stacking. While there is curiosity about user-perceivable performance gains, many commenters note that technical details remain scarce and require further verification.

**Tags**: `#semiconductors`, `#Huawei`, `#chip design`, `#Moore's Law`, `#integrated circuits`

---

<a id="item-3"></a>
## [Gwern Retires from Pseudonymous Writing to Launch Guardian Angel AI](https://twitter.com/gwern/status/2084739205071343837) ⭐️ 8.0/10

Gwern announced his retirement from full-time writing and pseudonymity to launch Guardian Angel, a project proposing deeply personalized AI assistants. The accompanying essay introduces 'digital twin LLMs' that emulate a single user's personality, values, and preferences. Gwern is a highly respected figure in AI/ML research, so this career shift signals a move from analysis to applied development. The project challenges mainstream chatbot alignment and offers a user-centric alternative, potentially influencing how future AI personalization and safety are discussed. The Guardian Angel proposal emphasizes three core principles: enhancement rather than replacement, mental sovereignty, and self-actualization. Gwern also argues that chatbot personas are aligned with their owners, not users, and that economic incentives currently push toward ads, subscriptions, and replacing the user rather than amplifying them.

hackernews · mattsterett · Aug 4, 20:48 · [Discussion](https://news.ycombinator.com/item?id=49174900)

**Background**: Gwern is known for long-form, rigorous essays on AI, machine learning, and other topics, written under a pseudonym. The new project proposes building 'Guardian Angels'—digital twin LLMs personalized to a single user's goals and values, with the aim of countering the misaligned incentives of mainstream chatbots. Alignment in AI refers to ensuring AI systems act in accordance with human intentions, but industry chatbot designs often prioritize engagement and profit over user well-being.

<details><summary>References</summary>
<ul>
<li><a href="https://gwern.net/guardian-angel">Guardian Angels: LLM Personalization for Productivity and Security · Gwern.net</a></li>
<li><a href="https://news.ycombinator.com/item?id=49174900">I am retiring from fulltime writing (& pseudonymity) to launch Guardian Angel | Hacker News</a></li>

</ul>
</details>

**Discussion**: Comments on Hacker News were mixed: some fully supported the three core principles of GA, while others called the framing 'a kind of mania' that treats LLMs as quasi-gods. A longtime collaborator praised Gwern's humanity and care, while another commenter questioned the heavy emphasis on productivity and asked how it reconciles with self-actualization.

**Tags**: `#AI`, `#LLM`, `#pseudonymity`, `#research`, `#career`

---

<a id="item-4"></a>
## [Mistral Releases Shieldstral, a 3B Open-Weights Multimodal Moderation Model](https://mistral.ai/news/shieldstral/) ⭐️ 8.0/10

Mistral AI has released Shieldstral-1.0-3B, a 3-billion-parameter open-weights model for multimodal content moderation. According to the paper, it matches or outperforms models nearly 7 times its size on text safety benchmarks and sets a new state of the art on multimodal safety classification. This matters because it offers a relatively small, cost-effective, and adaptable alternative to large proprietary moderation systems, potentially lowering the barrier for platforms that need robust content safety. The open-weights approach also allows developers to tune the model to their own policies, which could shift how online communities enforce moderation rules. The model is available on Hugging Face as 'mistralai/Shieldstral-1.0-3B', and Mistral describes it as a 'policy-adaptive' safety classifier. The associated arXiv paper (2607.25857) reports that Shieldstral sets a new state of the art on multimodal safety classification.

hackernews · riadsila · Aug 4, 16:36 · [Discussion](https://news.ycombinator.com/item?id=49171268)

**Background**: Open-weights models make advanced AI accessible to developers and startups without billion-dollar budgets, while still allowing fine-tuning and customization. Multimodal content moderation automatically detects unsafe material across text, images, audio, and video, which is increasingly necessary as harmful content on social media often spans multiple modalities, such as memes.

<details><summary>References</summary>
<ul>
<li><a href="https://mistral.ai/news/shieldstral/">Introducing Shieldstral. | Mistral AI</a></li>
<li><a href="https://arxiv.org/abs/2607.25857">[2607.25857] Shieldstral</a></li>
<li><a href="https://www.analyticsvidhya.com/blog/2024/09/building-multi-modal-models-for-content-moderation/">Building Multi-Modal Models for Content Moderation</a></li>

</ul>
</details>

**Discussion**: Commenters are generally positive about the model's economics and practicality, with one noting it could solve the moderation problem for image-sharing platforms. Others joked about the name and raised questions about how much the model can be tuned without retraining, and one commenter praised Mistral's shift toward smaller, fine-tuned models.

**Tags**: `#AI`, `#content moderation`, `#Mistral`, `#open-weights`, `#multimodal`

---

<a id="item-5"></a>
## [Custom color space and algorithm for diverse skin tone generation](https://toneyalexander.github.io/inclusive-color-space/) ⭐️ 8.0/10

The author released an interactive project introducing a custom color space and procedural generation algorithm that makes it easy to pick diverse, plausible skin tones for digital art and game development. The page includes live demos, equations, and detailed methodology, along with a Future Work section. This project directly addresses a practical pain point for artists and game developers who need inclusive character palettes, and it contributes to a broader industry discussion about modeling skin tones accurately and fairly. It also offers a hands-on alternative to established approaches like Oklab and Pantone Skin Tones, which are often less accessible to hobbyists. The color space is built by fitting functions (executed by hand) to observed skin-tone data, and sampling is performed from ellipses in a U-space formed by PCA-like basis vectors. The author admits the methodology is "a bit shaky" and lists several possible improvements in the Future Work section.

hackernews · automatoney · Aug 4, 15:16 · [Discussion](https://news.ycombinator.com/item?id=49170165)

**Background**: A color space is a mathematical way to represent colors in a coordinate system, and skin tones occupy a relatively small, curved region within standard RGB spaces. Existing research and tools, such as Oklab, Pantone Skin Tones, and The Pudding's makeup shade dataset, have explored this region, and the resulting distributions often form a crescent shape. PCA (principal component analysis) is a statistical technique that can reduce dimensions—here, it could map 3D color data to a 2D selector, but the author chose a different path based on fitted functions.

<details><summary>References</summary>
<ul>
<li><a href="https://terrific.tools/color/skin-color-generator">Skin Color Generator Tool [2026] - terrific.tools 20+ Real Skin Tone Color Palettes: HEX, RGB & HTML Codes This Free Tool Generates Diverse Skin Tones for Game Art True Tones: Skin Color Palettes for Inclusive Designs Skin Color Palettes: Light, Dark, Human & Anime Tones Skin color palette generator made easy - Logo Motion Graphics Skin color palettes maker easy way - Motion Visuals</a></li>
<li><a href="https://arxiv.org/html/2509.10980">TrueSkin: Towards Fair and Accurate Skin Tone Recognition and ...</a></li>
<li><a href="https://arxiv.org/pdf/2509.10980v1">TrueSkin: Towards Fair and Accurate Skin Tone Recognition and ...</a></li>

</ul>
</details>

**Discussion**: The community overwhelmingly praised the project: one commenter found the function fitting idea “very slick,” while another appreciated the first-principles approach and suggested referencing Pantone Skin Tones. Others connected the work to Oklab and makeup shade data, verified the crescent shape, and noted that fully saturated skin of any race appears orange.

**Tags**: `#color-space`, `#procedural-generation`, `#digital-art`, `#algorithm`, `#graphics`

---

<a id="item-6"></a>
## [Waymo Opens Driverless Ride-Hailing to Everyone in Dallas](https://waymo.com/blog/shorts/dallas-open-to-all/) ⭐️ 8.0/10

Waymo has expanded its fully driverless ride-hailing service to all users in Dallas, Texas, removing the earlier waitlist and making robotaxis available to anyone in the service area. The expansion adds another major metropolitan area to Waymo's growing list of operational cities. This marks a major commercial expansion of autonomous vehicle technology into a large Southern U.S. city, demonstrating Waymo's confidence in scaling Level 4 robotaxi operations. It will shape daily transportation options for Dallas residents and could influence local policy debates about autonomous vehicle safety and regulation. The service is fully driverless (SAE Level 4) and operates within a defined operational design domain (ODD) covering portions of Dallas. Some community observers note that Dallas's sprawling, hub-and-spoke urban layout may require a larger service area to make the service practically useful compared to cities like Austin or Houston.

hackernews · xnx · Aug 4, 18:29 · [Discussion](https://news.ycombinator.com/item?id=49172836)

**Background**: Waymo is a subsidiary of Alphabet that develops the Waymo Driver, an autonomous driving system designed to handle all driving tasks from pickup to destination. As of March 2026, Waymo operates about 3,000 robotaxis, provides 500,000 paid rides per week, and drives 4 million rider-only miles weekly. Level 4 autonomy means the vehicle can operate without human intervention within a specific operational design domain, such as predefined city zones or routes.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Waymo">Waymo - Wikipedia</a></li>
<li><a href="https://blogs.nvidia.com/blog/level-4-autonomous-driving-ai/">Level 4 Autonomous Driving and the Breakthroughs That Are ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Operational_design_domain">Operational design domain - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed but generally positive: some residents praise Waymo's predictability and claim it causes fewer traffic incidents than human drivers, while one commenter cites a New York City pilot that found Waymo to be more hazardous than human drivers. A commercial real estate professional argues driverless cars could serve as an effective affordable housing policy by reducing parking requirements. Another user notes the Dallas service area needs to expand quickly to be genuinely useful, given the city's spread-out layout.

**Tags**: `#autonomous-vehicles`, `#Waymo`, `#transportation`, `#urban-tech`, `#AI`

---

<a id="item-7"></a>
## [Oxide Computer raises $445M (SEC Form D)](https://www.sec.gov/Archives/edgar/data/1795071/000179507126000002/xslFormDX01/primary_doc.xml) ⭐️ 8.0/10

Oxide Computer raises $445M in a Series D round, signaling significant investor confidence in their cloud-native hardware approach.

hackernews · depr · Aug 4, 20:13 · [Discussion](https://news.ycombinator.com/item?id=49174407)

**Tags**: `#funding`, `#hardware`, `#cloud`, `#startups`

---

<a id="item-8"></a>
## [LLM 0.32 Adds Reasoning Traces, Server-Side Tools, and OpenAI Responses Support](https://simonwillison.net/2026/Aug/4/new-release-of-llm/#atom-everything) ⭐️ 8.0/10

Simon Willison released LLM 0.32, which can now display reasoning traces from reasoning models on stderr, adds server-side tools such as OpenAI CodeInterpreter and WebSearch, includes the GPT-5.6 model family with GPT-5.6 Luna as the new default, and leverages the OpenAI Responses API. The companion llm-anthropic plugin was also updated with WebFetch, CodeExecution, and AnthropicMCP tools. LLM is a widely used command-line tool for interacting with many model providers, so its latest release directly affects a large developer audience by making reasoning visible, enabling provider-hosted tool execution, and modernizing API integration. The update reflects growing industry momentum toward agentic workflows with built-in tool use and standardized interfaces. New command-line details include a -R/--hide-reasoning flag to suppress reasoning trace output, and a new llm openai endpoint command that sends one-off prompts to any OpenAI-compatible endpoint without logging them. The redesigned SQLite logs are content-addressable, and the llm-anthropic plugin adds an AnthropicMCP tool that lets Anthropic models call arbitrary MCP servers during a single request/response interaction.

rss · Simon Willison · Aug 4, 23:58

**Background**: LLM is an open-source command-line utility by Simon Willison that lets developers run prompts against many different language models from the terminal. Reasoning models generate intermediate 'reasoning traces' before producing a final answer, and LLM 0.32 displays these separately on standard error so they do not pollute piped output. Server-side tools are capabilities like code execution or web search that run on the provider's infrastructure, enabling agentic workflows without local setup. The OpenAI Responses API, released in March 2025, unifies chat-style calls with built-in tool use and stateful interactions, and LLM 0.32 builds on it.

<details><summary>References</summary>
<ul>
<li><a href="https://developers.openai.com/api/reference/responses/overview">Responses Overview | OpenAI API Reference</a></li>
<li><a href="https://jumpcloud.com/it-index/what-are-reasoning-traces-in-ai">What Are Reasoning Traces in AI ? - JumpCloud</a></li>
<li><a href="https://blog.textile.io/the-quest-for-a-content-addressable-sqlite">The Quest for a Content Addressable SQLite</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#AI tools`, `#release`, `#OpenAI`, `#developer tools`

---

<a id="item-9"></a>
## [MiniMax-H3 Omni-Modal Model Gets MLX Port for Apple Silicon](https://simonwillison.net/2026/Aug/4/minimax-h3-mlx/#atom-everything) ⭐️ 8.0/10

MiniMax has released MiniMax-H3, a general-purpose omni-modal generative system capable of generating up to 15-second video clips with audio. A new MLX port, minimax-h3-mlx, enables running this model locally on Apple Silicon, as demonstrated by Simon Willison on an M5 Max MacBook Pro. This lowers the barrier for experimenting with state-of-the-art multimodal generation on consumer hardware, making advanced AI tools more accessible to developers and researchers. It also highlights the rapid maturation of open omni-modal models and the growing ecosystem of MLX ports. The model requires downloading roughly 115 GB of files, and generating a single video took just under 45 minutes on an M5 Max MacBook Pro. Following the official prompting guide is important, as unguided audio output can be meaningless (e.g., speech-like garbage).

rss · Simon Willison · Aug 4, 19:10

**Background**: Omni-modal models integrate text, images, audio, and video into a single unified architecture, going beyond traditional multimodal systems. MLX is Apple's open-source machine learning framework designed for Apple Silicon, featuring a unified memory model that lets CPU and GPU share data efficiently. MiniMax-H3 is an open model that supports 768p video with native 32 kHz stereo audio and multiple languages. The MLX port adapts the original MiniMax-H3 weights for local inference on Apple hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://opensource.apple.com/projects/mlx/">Apple Open Source</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/omni-model/">What is an Omni-Model? Definition, Architecture, & NVIDIA Solutions</a></li>
<li><a href="https://comfyui-wiki.com/en/models/minimax">MiniMax H3: Open Omni-Modal Video Model With Native Audio</a></li>

</ul>
</details>

**Tags**: `#AI`, `#MLX`, `#multimodal`, `#video generation`, `#MiniMax`

---

<a id="item-10"></a>
## [Cloudflare replaces third-party security tools with $58/month AI for bug bounties](https://www.theregister.com/security/2026/08/04/cloudflare-has-mostly-ditched-third-party-security-tools-suggests-not-trying-that-at-home/5282600) ⭐️ 8.0/10

Cloudflare's Chief Security Officer Grant Bourzikas revealed in Sydney that the company now uses Anthropic's Claude Sonnet model to automate bug bounty report triage, costing only $58 per month. Cloudflare has also built more than 200 autonomous security agents and largely replaced third-party security tools with internally developed, AI-assisted applications. This demonstrates a dramatic cost reduction in security operations, as the same bug triage work with the security-specific Mythos model would cost roughly $200,000 per month. It signals a broader industry shift toward AI-driven security automation, while Cloudflare's caution that other firms should not blindly copy the approach highlights the need for strong in-house engineering capabilities. Claude Sonnet is responsible for deduplicating and assessing the value of incoming bug bounty reports, while the Mythos security model would cost about $200,000 per month for the same workload. Bourzikas cautioned that not every company should build its own security software, and Cloudflare itself has laid off 1,100 people, which its chief strategy officer attributed to AI-driven automation changes.

telegram · zaihuapd · Aug 4, 09:24

**Background**: Bug bounty triage is the process of reviewing, filtering, and evaluating vulnerability reports submitted by external security researchers before they are acted upon. Claude Sonnet is Anthropic's mid-tier large language model, while Mythos is Anthropic's specialized security model designed for fixing software vulnerabilities and subject to additional safeguards. Cloudflare's approach reflects its unique position as a security-focused cloud company with deep engineering expertise, and it is also exploring becoming an intermediary between AI companies and publishers through micropayments.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/claude/sonnet">Claude Sonnet \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Mythos">Claude Mythos - Wikipedia</a></li>
<li><a href="https://www.hackerone.com/platform/triage-101">Triage 101 | HackerOne</a></li>

</ul>
</details>

**Tags**: `#security`, `#AI`, `#Cloudflare`, `#automation`, `#bug-bounty`

---

<a id="item-11"></a>
## [Google Builds $200B Wall Street Financing Machine for Anthropic AI Chips](https://www.ft.com/content/549f2e23-5aa2-49c7-9ea6-a9784ab7087c) ⭐️ 8.0/10

Google has quietly created one of the largest infrastructure financing mechanisms ever, delivering more than $150 billion in AI chips to Anthropic through a roughly $200 billion Wall Street-backed structure. The first transactions, completed in June via the Compute SPV, bought about $35 billion in hardware, including 1 GW of compute and 1 million TPUs. This unprecedented off-balance-sheet financing model could redefine how AI compute is funded and scaled, setting a new precedent for the industry. It gives Anthropic massive compute access without straining its balance sheet, while deepening Google's strategic grip on the AI ecosystem and attracting major financial players into AI infrastructure. The contracts total about $200 billion, with roughly 80% directly tied to chips; Broadcom, Apollo, Blackstone, Morgan Stanley, and several crypto miners are involved. Risk is shared: Google guarantees data centers, Broadcom buys and helps finance chips, and Apollo and Blackstone purchase hardware and lease it back to Anthropic, following the vendor financing model used by Boeing and GE.

telegram · zaihuapd · Aug 4, 10:52

**Background**: A special purpose vehicle (SPV) is a separate legal entity used to isolate financial risk and keep assets off the sponsor's balance sheet. Vendor financing, pioneered by Boeing and GE for aircraft and engines, allows a supplier to help a customer fund a large purchase while sharing risk. TPUs are Google's custom application-specific integrated circuits (ASICs) designed to accelerate machine learning workloads. Anthropic, an AI startup without a credit rating, relies on Google Cloud TPUs to train and run its large language models.

<details><summary>References</summary>
<ul>
<li><a href="https://www.investopedia.com/terms/s/spv.asp">investopedia.com/terms/s/ spv .asp</a></li>
<li><a href="https://en.wikipedia.org/wiki/Tensor_Processing_Unit">Tensor Processing Unit - Wikipedia</a></li>
<li><a href="https://cloud.google.com/tpu">Tensor Processing Units (TPUs) | Google Cloud</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Anthropic`, `#Google`, `#Financing`, `#Infrastructure`

---

<a id="item-12"></a>
## [China's First Mandatory L3/L4 Autonomous Driving Safety Standard Heads to Public Comment](https://t.me/zaihuapd/42972) ⭐️ 8.0/10

China's Ministry of Industry and Information Technology (MIIT) has completed the draft of the mandatory national standard 'Safety Requirements for Intelligent Connected Vehicle Autonomous Driving Systems' and opened it for public comment on June 17, with a proposed implementation date of July 1, 2027. This is China's first mandatory national standard specifically targeting L3 and L4 autonomous driving. The standard marks a shift from loose conceptual marketing to hard safety constraints for automakers, requiring them to systematically demonstrate safety through a Safety Case mechanism. It will affect all companies developing L3 and L4 systems in China, raising the bar for market entry and potentially influencing global regulatory trends. The standard introduces a Safety Case (声明—论据—证据) framework, requiring companies to articulate and substantiate safety claims with evidence. It separately addresses L3 human-machine handover requirements and L4 system autonomous risk handling.

telegram · zaihuapd · Aug 4, 13:06

**Background**: L3 and L4 refer to SAE automation levels: L3 allows conditional automation where the driver must remain ready to take over, while L4 can handle all driving in defined conditions without driver intervention. A Safety Case is a structured argument, supported by evidence, that a system is safe to operate in a given environment; it has become best practice for autonomous vehicle safety since UL 4600. L3 handover is widely considered an unsolved challenge, as drivers may need several seconds to regain control.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2404.05444">The Open Autonomy Safety Case Framework - arXiv.org</a></li>
<li><a href="https://urgentcomm.com/drones-robots/vehicle-human-handover-at-level-3-still-an-unsolved-challenge-on-path-to-autonomous-vehicles">Vehicle-human handover at Level 3 still an unsolved challenge on path to autonomous vehicles</a></li>
<li><a href="https://eu.36kr.com/en/p/3787724574448901">New Regulations Set the Tone: Say Goodbye to Ineffective L3 Involution, L4 as the Ultimate Goal of Autonomous Driving Commercialization</a></li>

</ul>
</details>

**Tags**: `#autonomous-driving`, `#regulation`, `#safety-standards`, `#China`, `#L3-L4`

---