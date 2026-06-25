---
layout: default
title: "Horizon Summary: 2026-06-25 (EN)"
date: 2026-06-25
lang: en
---

> From 34 items, 10 important content pieces were selected

---

1. [OpenAI Unveils First Custom Chip Jalapeno with Broadcom](#item-1) ⭐️ 9.0/10
2. [Qualcomm Acquires AI Startup Modular for $4B](#item-2) ⭐️ 9.0/10
3. [Krea 2: Open-weights 12B image model released](#item-3) ⭐️ 9.0/10
4. [Micron's Record Q3: 346% Revenue Surge, $3.1B Daily Profit](#item-4) ⭐️ 9.0/10
5. [Anthropic Accuses Alibaba of Massive Distillation Attack on Claude](#item-5) ⭐️ 9.0/10
6. [NVIDIA's 45°C Liquid Cooling Cuts Data Center Water Use Near Zero](#item-6) ⭐️ 8.0/10
7. [Nub: Bun-like all-in-one toolkit for Node.js](#item-7) ⭐️ 8.0/10
8. [Generative AI for homework may lower Chinese students' exam scores](#item-8) ⭐️ 8.0/10
9. [Cloudflare and Partners Propose PACT to Replace CAPTCHAs](#item-9) ⭐️ 8.0/10
10. [Google Play Expands External Billing to US, UK, and EEA](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI Unveils First Custom Chip Jalapeno with Broadcom](https://techcrunch.com/2026/06/24/openai-unveils-its-first-custom-chip-built-by-broadcom/) ⭐️ 9.0/10

OpenAI and Broadcom have introduced Jalapeño, a custom AI inference chip designed for large language models, manufactured by TSMC and developed in just nine months. This marks OpenAI's entry into custom AI hardware, potentially reducing reliance on NVIDIA GPUs for inference and improving energy efficiency at scale. Early testing shows Jalapeño delivers substantially better performance per watt than existing solutions, and the chip's design was accelerated using OpenAI's own AI models.

hackernews · jamdesk · Jun 24, 17:47 · [Discussion](https://news.ycombinator.com/item?id=48663324)

**Background**: AI inference chips are specialized hardware designed to run trained machine learning models efficiently. Companies like Google have developed their own Tensor Processing Units (TPUs) for similar purposes. Custom chips allow optimization for specific workloads, potentially offering cost and performance advantages over general-purpose GPUs.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/openai-broadcom-jalapeno-inference-chip/">OpenAI and Broadcom unveil LLM-optimized inference chip</a></li>
<li><a href="https://www.techpowerup.com/forums/threads/openai-unveils-jalapeno-llm-inferencing-accelerator-built-in-collaboration-with-broadcom.350253/">OpenAI Unveils Jalapeno LLM Inferencing Accelerator Built in ...</a></li>

</ul>
</details>

**Discussion**: The community had mixed reactions: some users were skeptical about the claimed AI-accelerated design process, calling it marketing speak, while others praised the potential efficiency gains and compared the move to Google's TPU strategy. A few commenters also discussed alternative approaches like burning model weights directly into silicon.

**Tags**: `#OpenAI`, `#custom chip`, `#AI hardware`, `#Broadcom`, `#inference`

---

<a id="item-2"></a>
## [Qualcomm Acquires AI Startup Modular for $4B](https://www.reuters.com/business/qualcomm-buy-ai-startup-modular-2026-06-24/) ⭐️ 9.0/10

Qualcomm announced on June 24, 2026, the acquisition of Modular, the company behind the Mojo programming language and MAX AI inference stack, for approximately $4 billion. This acquisition strengthens Qualcomm's AI inference capabilities, providing an alternative to NVIDIA's CUDA stack, and could accelerate adoption of ARM-based AI inference at scale. The deal includes Modular's Mojo language, which combines Python-like syntax with high performance via the MLIR compiler framework, and the MAX framework for heterogeneous hardware inference. Mojo is expected to open-source in fall 2026.

hackernews · timmyd · Jun 24, 13:49 · [Discussion](https://news.ycombinator.com/item?id=48659798)

**Background**: Mojo is a programming language designed for AI infrastructure, leveraging the MLIR compiler framework to target CPUs, GPUs, and accelerators, while maintaining Python compatibility. Modular also developed MAX, a hardware-agnostic serving framework for deploying AI models efficiently. Qualcomm, a leading designer of ARM-based chips, has been expanding its AI portfolio to compete with NVIDIA and others in the data center and edge AI markets.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mojo_(programming_language)">Mojo (programming language)</a></li>
<li><a href="https://www.modular.com/">Modular: Inference from Kernel to Cloud</a></li>
<li><a href="https://github.com/modular/modular">GitHub - modular/modular: The Modular Platform (includes MAX & Mojo) · GitHub</a></li>

</ul>
</details>

**Discussion**: Community comments express surprise at the early acquisition and mixed feelings about Mojo's direction, with some viewing it as a waste of Chris Lattner's talent. Others see strategic implications for ARM vs NVIDIA and RISC-V, noting Qualcomm's recent moves to build AI-focused technologies.

**Tags**: `#acquisition`, `#AI`, `#compilers`, `#Qualcomm`, `#Modular`

---

<a id="item-3"></a>
## [Krea 2: Open-weights 12B image model released](https://www.krea.ai/blog/krea-2-technical-report) ⭐️ 9.0/10

Krea AI released Krea 2, a state-of-the-art open-weights 12B parameter text-to-image model, along with a detailed technical report covering data curation, architecture, and training infrastructure. The release includes two versions: Krea 2 and Krea 2 Turbo (distilled for faster inference). This release significantly advances open-source AI image generation, as Krea 2 achieves competitive results against leading closed-source models while being open-weights and locally hostable. It empowers developers and researchers to customize and deploy high-quality image generation without relying on proprietary APIs. The Krea 2 Turbo model uses guidance distillation and timestep distillation to achieve fast generation in as few as 8 steps, outperforming many other locally hostable models. The technical report provides unprecedented detail on data curation, captioning, model architecture, post-training, RL pipelines, prompt expansion, and style references.

hackernews · mattnewton · Jun 23, 15:31 · [Discussion](https://news.ycombinator.com/item?id=48646659)

**Background**: Open-weights models provide the trained neural network weights but may not include the full training data or pipeline, allowing users to run the model locally with sufficient hardware. A 12B parameter model is considered large for image generation, requiring substantial computational resources but offering high quality. This is part of a trend where open models are catching up to proprietary ones.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Large_language_model">Large language model - Wikipedia</a></li>
<li><a href="https://huggingface.co/blog/daya-shankar/open-source-llms">Best Open -Source LLM Models in 2026: Coding, Local, Agentic AI ...</a></li>
<li><a href="https://www.ibm.com/think/topics/mistral-ai">What is Mistral AI? | IBM</a></li>

</ul>
</details>

**Discussion**: The authors engaged actively in comments, highlighting the detailed technical report and the two model releases. One commenter praised the turbo model's speed and competitiveness, noting it outperformed most locally hostable models except Ideogram 4, while also mentioning common failure cases. Another commenter appreciated the open weights but questioned the approach's relevance given newer composition-focused models.

**Tags**: `#AI`, `#image generation`, `#open-weights`, `#machine learning`, `#text-to-image`

---

<a id="item-4"></a>
## [Micron's Record Q3: 346% Revenue Surge, $3.1B Daily Profit](https://www.globenewswire.com/news-release/2026/06/24/3317151/14450/en/micron-technology-inc-reports-record-results-for-the-third-quarter-of-fiscal-2026.html) ⭐️ 9.0/10

Micron reported fiscal Q3 2026 results with revenue of $414.6 billion, up 346% year-over-year, and net profit of $28.24 billion, equivalent to $3.1 billion per day. This extraordinary performance underscores explosive AI-driven demand for high-bandwidth memory, positioning Micron as a key beneficiary of the AI infrastructure buildout. It signals sustained memory shortages and could pressure competitors to accelerate HBM production. Data center revenue surged 653% to $115.2 billion, and non-GAAP gross margin rose to 84.9%. Micron has started mass production of HBM4 and expects HBM4E in 2027, with 16 long-term agreements in place.

telegram · zaihuapd · Jun 24, 22:22

**Background**: High Bandwidth Memory (HBM) is a 3D-stacked DRAM technology that provides significantly higher bandwidth than traditional DDR memory, crucial for AI accelerators and high-performance GPUs. HBM4 is the latest generation, and HBM4E is an enhanced version expected to offer even greater speeds and efficiency. The memory industry is in a race to mass-produce these next-gen chips to meet AI infrastructure demands.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://nerds.xyz/2026/06/samsung-hbm4e-memory/">Samsung ships industry-first HBM 4 E memory as AI infrastructure race...</a></li>

</ul>
</details>

**Tags**: `#Micron`, `#semiconductors`, `#AI infrastructure`, `#memory`, `#earnings`

---

<a id="item-5"></a>
## [Anthropic Accuses Alibaba of Massive Distillation Attack on Claude](https://www.cnbc.com/2026/06/24/anthropic-alibaba-distillation-campaign.html) ⭐️ 9.0/10

On June 10, 2026, Anthropic sent a letter to the U.S. Senate Banking Committee accusing Alibaba and its Qwen lab of orchestrating the largest known distillation attack against Claude, using approximately 25,000 fraudulent accounts to conduct over 28.8 million interactions from April 22 to June 5, 2026. This accusation highlights escalating AI intellectual property tensions between the U.S. and China, potentially affecting international tech competition and AI security practices. It also underscores the vulnerability of frontier AI models to distillation attacks, which could erode competitive advantages and safety controls. The letter was sent ahead of a congressional AI hearing and references earlier U.S. actions including the White House's April accusation of Chinese AI IP theft and the June 12 Commerce Department export restrictions on Anthropic's Mythos and Fable models. Alibaba has not yet responded to the allegations.

telegram · zaihuapd · Jun 25, 01:36

**Background**: Distillation attacks involve using a weaker model to learn from a stronger model's outputs, effectively copying its capabilities. In 2026, such attacks have become a major AI security concern; Anthropic had previously accused three Chinese AI firms (DeepSeek, Kimi, MiniMax) of similar attacks in February 2026.

<details><summary>References</summary>
<ul>
<li><a href="https://jangwook.net/zh/blog/zh/ai-distillation-attacks-enterprise-defense/">AI 模型 蒸 馏 攻 击 实态——CTO必知的IP保护策略</a></li>
<li><a href="https://zmyx.net/knowledge-distillation-or-distillation-theft/">中美 AI 博弈的最新焦点：“知识 蒸 馏 ”和“ 蒸 馏 攻 击 ” - 中美印象</a></li>

</ul>
</details>

**Tags**: `#AI security`, `#distillation attack`, `#Anthropic`, `#Alibaba`, `#geopolitics`

---

<a id="item-6"></a>
## [NVIDIA's 45°C Liquid Cooling Cuts Data Center Water Use Near Zero](https://blogs.nvidia.com/blog/liquid-cooling-ai-factories/) ⭐️ 8.0/10

NVIDIA has introduced a new liquid cooling architecture for AI data centers that uses coolant at up to 45°C, dramatically reducing water consumption by enabling dry cooling or free cooling in many climates. As AI workloads drive unprecedented heat densities, this design addresses water scarcity concerns and opens the door to district heating synergies, potentially turning data centers into local heat sources. The cooling uses direct-to-chip liquid cooling with coolant temperatures up to 45°C (113°F), which is higher than traditional liquid cooling loops, and works especially well in favorable climates where ambient air can cool the coolant.

hackernews · nitin_flanker · Jun 24, 14:10 · [Discussion](https://news.ycombinator.com/item?id=48660178)

**Background**: Traditional data centers rely on energy-intensive air conditioning or chilled water systems, consuming large amounts of water for evaporative cooling. Liquid cooling directly removes heat from chips, and raising the coolant temperature allows for dry cooling or heat rejection without water evaporation. District heating networks can use low-grade heat (around 45°C) to warm buildings, creating a potential synergy.

<details><summary>References</summary>
<ul>
<li><a href="https://www.guru3d.com/story/nvidia-unveils-liquid-cooling-design-for-ai-data-centers/">NVIDIA Unveils 45 ° C Liquid Cooling Design for AI Data Centers</a></li>
<li><a href="https://www.techbuzz.ai/articles/nvidia-s-45-c-liquid-cooling-redefines-ai-data-center-energy">NVIDIA's 45 ° C Liquid Cooling Redefines AI Data Center Energy</a></li>
<li><a href="https://www.araner.com/blog/data-center-and-district-heating-an-outstanding-combination">Data center and district heating : an outstanding combination</a></li>

</ul>
</details>

**Discussion**: Community members noted the potential for district heating synergies, with one commenter suggesting data centers could offer free heat to communities. Others questioned the innovation, pointing out that higher coolant temperatures are not new and asked for more detail on climate dependency. A reference to NASA's similar high-temperature water cooling was provided.

**Tags**: `#data center`, `#cooling`, `#water conservation`, `#sustainability`, `#AI infrastructure`

---

<a id="item-7"></a>
## [Nub: Bun-like all-in-one toolkit for Node.js](https://github.com/nubjs/nub) ⭐️ 8.0/10

Nub is a new toolkit that provides a Bun-like developer experience for Node.js using preload hooks and oxc-based transpilation. It significantly improves the Node.js developer experience by bringing fast TypeScript transpilation and polyfills without leaving the Node.js ecosystem. Nub uses a --require preload hook to integrate an oxc-powered transpiler as a Node-API add-on and registers a module resolution hook, injecting polyfills for APIs like Worker and Temporal purely additively.

hackernews · colinmcd · Jun 24, 14:14 · [Discussion](https://news.ycombinator.com/item?id=48660267)

**Background**: Bun is an all-in-one JavaScript runtime with built-in transpilation and package management. Node.js traditionally needs separate tools for TypeScript support. Nub leverages Node's --require hook and the high-performance oxc transpiler (written in Rust) to emulate Bun's streamlined DX on top of stock Node.js.

<details><summary>References</summary>
<ul>
<li><a href="https://git-stars.org/repositories/topic/transpiler">Top transpiler Repositories - GitHub Projects for transpiler ... | Git Stars</a></li>
<li><a href="https://stackoverflow.com/questions/67256729/difference-between-nodejs-preload-option-r-and-explicit-require-in-in-repl">javascript - Difference between NodeJs preload ... - Stack Overflow</a></li>

</ul>
</details>

**Discussion**: Community comments are largely positive, praising the concept and the author's credibility. Technical discussion revolves around the choice of --require over --import for ESM support, and whether a transpiler is needed given Node's native TypeScript support. Some users report seamless migration to Nub.

**Tags**: `#Node.js`, `#TypeScript`, `#Bun`, `#developer-tools`, `#toolkit`

---

<a id="item-8"></a>
## [Generative AI for homework may lower Chinese students' exam scores](https://cepr.org/publications/dp21577) ⭐️ 8.0/10

A 30-month study of 26,811 Chinese students in grades 7-12 found that while generative AI improved homework scores by 18% and reduced completion time by 30%, it led to 18-24% lower scores on high-stakes exams such as the Zhongkao and Gaokao, with effects fully manifesting after about two years. This large-scale empirical study provides robust evidence that reliance on generative AI for homework can negatively impact deep learning and exam performance, raising concerns about the integration of AI tools in education and highlighting the need for balanced usage policies. The study found that social science subjects suffered the greatest score drops, followed by STEM and languages; lower-grade, high-achieving, and male students were more affected. Roughly 80% of AI users exhibited 'homework outsourcing' behavior with very short homework times and high scores, bearing the main losses.

telegram · zaihuapd · Jun 24, 05:15

**Background**: Generative AI, such as large language models (e.g., GPT, Claude), can produce coherent text and solve problems, making it tempting for students to use for homework. However, this may bypass the learning process needed to retain knowledge for closed-book exams. This study tracked 26,811 Chinese students over 30 months to assess long-term impacts.

**Tags**: `#generative AI`, `#education`, `#exam performance`, `#empirical study`, `#impact analysis`

---

<a id="item-9"></a>
## [Cloudflare and Partners Propose PACT to Replace CAPTCHAs](https://www.techtimes.com/articles/318891/20260623/cloudflare-chrome-firefox-plan-replace-captchas-cryptographic-tokens.htm) ⭐️ 8.0/10

Cloudflare, along with Chrome, Firefox, Edge, and Shopify, has proposed the PACT protocol to replace CAPTCHAs with anonymous cryptographic tokens, using blind signatures from Privacy Pass. This could eliminate frustrating CAPTCHA challenges while preserving user privacy, as tokens do not reveal identity or browsing history, and also differentiate legitimate AI agents from malicious bots. The PACT protocol is currently a proposal without a finalized standards body or timeline, and Apple has not joined; governance of token issuers remains unresolved.

telegram · zaihuapd · Jun 24, 06:30

**Background**: CAPTCHAs are widely used to distinguish humans from bots but are often inconvenient and inaccessible. Privacy Pass, an IETF standard, enables anonymous token-based verification using blind signatures, where a token is signed without the signer seeing the content, ensuring unlinkability.

<details><summary>References</summary>
<ul>
<li><a href="https://privacypass.github.io/">Privacy Pass</a></li>
<li><a href="https://en.wikipedia.org/wiki/Blind_signature">Blind signature</a></li>

</ul>
</details>

**Tags**: `#web security`, `#CAPTCHA replacement`, `#cryptographic tokens`, `#privacy`

---

<a id="item-10"></a>
## [Google Play Expands External Billing to US, UK, and EEA](https://android-developers.googleblog.com/2026/06/play-expanded-billing.html) ⭐️ 8.0/10

Google announced that from June 30, developers can offer external billing options to users in the US, UK, and European Economic Area, with a restructured service fee that separates the Play service fee from the billing fee. This expansion marks the largest rollout of external billing on Google Play, likely in response to regulatory pressures, and could fundamentally alter the economics of app distribution by giving developers more flexibility and potentially lower fees. For the first $1 million annual revenue and auto-renewing subscriptions, the service fee is 10%; other transactions are categorized as 'new install' or 'existing install'. In these regions, an additional 5% billing fee applies only when using Google Play Billing.

telegram · zaihuapd · Jun 25, 02:33

**Background**: Traditionally, Google Play required developers to use its own billing system, which charged a commission of 15-30%. External billing allows developers to use third-party payment processors, reducing Google's cut. The new structure separates service fee (for Play's platform services) from billing fee (for payment processing).

<details><summary>References</summary>
<ul>
<li><a href="https://developer.android.com/google/play/billing/external">External offers APIs | Play Billing | Android Developers</a></li>
<li><a href="https://play.google.com/console/about/">Google Play for business | Launch & monetize your apps</a></li>

</ul>
</details>

**Tags**: `#Google Play`, `#external billing`, `#antitrust`, `#developer policy`, `#mobile ecosystem`

---