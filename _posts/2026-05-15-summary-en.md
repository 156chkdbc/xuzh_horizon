---
layout: default
title: "Horizon Summary: 2026-05-15 (EN)"
date: 2026-05-15
lang: en
---

> From 37 items, 15 important content pieces were selected

---

1. [Severe 18-Year-Old NGINX RCE Vulnerability Disclosed](#item-1) ⭐️ 10.0/10
2. [First public macOS kernel memory corruption exploit on Apple M5](#item-2) ⭐️ 9.0/10
3. [New arXiv policy: 1-year ban for hallucinated references](#item-3) ⭐️ 9.0/10
4. [Bun Rewritten from Zig to Rust Merged](#item-4) ⭐️ 9.0/10
5. [DeepSeek session isolation bug leaks user chat history](#item-5) ⭐️ 9.0/10
6. [vLLM v0.21.0: Deprecates Transformers v4, Adds KV Offload and Blackwell Backend](#item-6) ⭐️ 8.0/10
7. [Removing Modem and GPS from 2024 Toyota RAV4 Hybrid](#item-7) ⭐️ 8.0/10
8. [Antirez unveils DwarfStar4: a focused LLM runtime for DeepSeek 4](#item-8) ⭐️ 8.0/10
9. [RTX 5090 eGPU Works on M4 MacBook Air for Gaming and LLM](#item-9) ⭐️ 8.0/10
10. [New Nginx exploit with specific rewrite/set preconditions](#item-10) ⭐️ 8.0/10
11. [MIT President Warns on Funding and Talent Pipeline](#item-11) ⭐️ 8.0/10
12. [US Clears H200 Sales to China; Nvidia CEO Visits to Boost Deals](#item-12) ⭐️ 8.0/10
13. [ChatGPT Android APK Teardown Reveals Codex Remote Desktop Control](#item-13) ⭐️ 8.0/10
14. [China in Talks with Boeing for Up to 500 737 MAX Jets](#item-14) ⭐️ 8.0/10
15. [Anima: 2B Parameter Open-Source Anime Text-to-Image Model](#item-15) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Severe 18-Year-Old NGINX RCE Vulnerability Disclosed](https://depthfirst.com/research/nginx-rift-achieving-nginx-rce-via-an-18-year-old-vulnerability) ⭐️ 10.0/10

A critical remote code execution vulnerability (CVE-2026-42945, CVSS 9.2) in NGINX's ngx_http_rewrite_module was disclosed on May 13, 2026, affecting all NGINX versions from 0.6.27 to 1.30.0 and multiple F5 enterprise products. This vulnerability, latent for 18 years, threatens billions of servers globally, especially in cloud-native Kubernetes ingress and API gateway deployments, where exploitation could lead to full server compromise without authentication. The vulnerability is a heap buffer overflow caused by inconsistent two-pass execution in the rewrite module's URI handling, where a placeholder character ('?') triggers improper buffer length calculation, leading to memory corruption exploitable via crafted HTTP requests.

telegram · zaihuapd · May 14, 02:41

**Background**: The ngx_http_rewrite_module uses a two-pass execution: first pass calculates the required buffer size, second pass writes data. A bug occurs when a rewrite directive's replacement string contains a '?' character, causing the length calculation to underestimate the required size because the second pass URL-encodes special characters, expanding them from 1 to 3 bytes. This discrepancy leads to heap overflow. Exploitation involves heap layout manipulation via connection timing and injecting payloads via POST request body.

<details><summary>References</summary>
<ul>
<li><a href="https://depthfirst.com/research/nginx-rift-achieving-nginx-rce-via-an-18-year-old-vulnerability">NGINX Rift: Achieving NGINX Remote Code Execution via... | depthfirst</a></li>
<li><a href="https://en.wikipedia.org/wiki/Buffer_overflow">Buffer overflow - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#security`, `#vulnerability`, `#nginx`, `#RCE`, `#CVE`

---

<a id="item-2"></a>
## [First public macOS kernel memory corruption exploit on Apple M5](https://blog.calif.io/p/first-public-kernel-memory-corruption) ⭐️ 9.0/10

Researchers from Calif, using the AI system Mythos Preview, developed the first public kernel memory corruption exploit for Apple M5 hardware, bypassing the MIE (Memory Integrity Enforcement) protection in just 5 days. This demonstrates that AI-assisted exploit development can rapidly break state-of-the-art hardware defenses like Apple's MIE, challenging the security assumptions of the entire Apple ecosystem. The exploit targets macOS 26.4.1 on M5 and works from an unprivileged user to gain root shell using only normal system calls, bypassing MIE's memory tagging. A full 55-page technical report will be released after Apple patches the vulnerabilities.

hackernews · quadrige · May 14, 18:25 · [Discussion](https://news.ycombinator.com/item?id=48139219)

**Background**: Memory Integrity Enforcement (MIE) is a hardware security feature on Apple M5 and A19 chips, using ARM's Enhanced Memory Tagging Extension (EMTE) in synchronous mode to protect against memory corruption attacks. It was touted as an unparalleled protection. Mythos Preview is an AI system developed by Anthropic that has been shown capable of autonomous hacking in tests.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.calif.io/p/first-public-kernel-memory-corruption">First public macOS kernel memory corruption exploit on Apple M5</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apple_M5">Apple M5 - Wikipedia</a></li>
<li><a href="https://www.computerworld.com/article/4124435/apple-touts-unparalleled-protection-for-m5-macs.html">Apple touts ‘unparalleled’ protection for M5 Macs</a></li>

</ul>
</details>

**Discussion**: Comments express excitement about AI's impact on security, with some noting that the exploit might be worth $100,000 to $1.5 million. One user sarcastically suggested Apple is faking vulnerabilities to hype Mythos, while others find the lack of technical details frustrating.

**Tags**: `#security`, `#kernel exploit`, `#Apple M5`, `#AI-assisted`, `#macOS`

---

<a id="item-3"></a>
## [New arXiv policy: 1-year ban for hallucinated references](https://twitter.com/tdietterich/status/2055000956144935055) ⭐️ 9.0/10

arXiv announced a policy imposing a 1-year ban on authors whose submissions contain hallucinated references, after which they must first have a paper accepted at a peer-reviewed venue before future submissions. This policy directly combats the surge of AI-generated fake citations in scientific literature, preserving research integrity and setting a precedent for other preprint repositories. Enforcement challenges include detecting hallucinated references at scale, possibly through automated DOI verification or manual spot checks; the policy also requires a peer-reviewed acceptance after the ban.

hackernews · gjuggler · May 14, 20:39 · [Discussion](https://news.ycombinator.com/item?id=48140922)

**Background**: arXiv is an open-access preprint server that does not require peer review. Hallucinated references are non-existent citations generated by AI tools; a Nature analysis suggested tens of thousands of 2025 publications may contain such errors, with a tenfold increase since 2023.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ArXiv">arXiv - Wikipedia</a></li>
<li><a href="https://www.nature.com/articles/d41586-026-00969-z">Hallucinated citations are polluting the scientific ... - Nature</a></li>
<li><a href="https://byteiota.com/arxiv-bans-authors-1-year-for-ai-hallucinated-citations/">arXiv Bans Authors 1 Year for AI-Hallucinated Citations</a></li>

</ul>
</details>

**Discussion**: Community comments largely support the policy but express concerns about enforcement scalability and detection methods; some suggest improving citation tools like Zotero, while others praise the move as upholding arXiv as a privilege.

**Tags**: `#arXiv`, `#academic publishing`, `#AI ethics`, `#hallucination`, `#policy`

---

<a id="item-4"></a>
## [Bun Rewritten from Zig to Rust Merged](https://github.com/oven-sh/bun/pull/30412) ⭐️ 9.0/10

The Bun project merged PR #30412, rewriting the entire runtime from Zig to Rust over approximately one week. This change adds over 1 million lines of Rust code and removes most of the previous Zig codebase. This rewrite could significantly impact Bun's memory safety and ecosystem compatibility, as Rust offers stronger guarantees than Zig in certain areas. It also sparks debate about LLM-assisted large-scale code migrations in production software. The PR was prepared with detailed instructions mapping Zig to Rust idioms, and the Bun codebase already used internal smart pointer types that map 1-to-1 to Rust equivalents. The rewrite adds 10,428 instances of 'unsafe' blocks across 736 files, and the Rust codebase now totals 929,213 lines.

hackernews · Chaoses · May 14, 08:15 · [Discussion](https://news.ycombinator.com/item?id=48132488)

**Background**: Bun is an all-in-one JavaScript runtime written in Zig and powered by JavaScriptCore, designed as a fast drop-in replacement for Node.js. Zig is a systems programming language focused on simplicity and performance. Rust is another systems language known for memory safety without garbage collection. This rewrite transitions Bun's core from Zig to Rust.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/oven-sh/bun">GitHub - oven-sh/bun: Incredibly fast JavaScript runtime ... Bun Guide: Install, Configure & Deploy the Fast JS Runtime ... Bun 2026: How the Anthropic Acquisition Reshapes the ... How to Install Bun - commandlinux.com What Is Bun JS? Ultra-Fast JavaScript Runtime Explained (2025 ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>

</ul>
</details>

**Discussion**: Comments show mixed reactions: some question how a one-week rewrite was possible, suggesting heavy LLM involvement; others defend the team's approach, emphasizing end results over process. Notable concerns include the high count of 'unsafe' Rust code (10,428 blocks) and the codebase size approaching that of the Rust compiler.

**Tags**: `#Bun`, `#Rust`, `#Zig`, `#JavaScript runtime`, `#software engineering`

---

<a id="item-5"></a>
## [DeepSeek session isolation bug leaks user chat history](https://github.com/deepseek-ai/DeepSeek-R1/issues/840) ⭐️ 9.0/10

A session isolation vulnerability in DeepSeek's dialogue system allows attackers to leak other users' conversation history by sending an unclosed '<think' string in an empty chat. This vulnerability can expose sensitive user data such as code, keys, and private conversations, posing a significant privacy risk across deployments. It undermines trust in AI chatbot security and highlights the need for robust session isolation. The vulnerability was reported by cancat2024 on May 11, 2026, who disclosed it responsibly without exploiting the flaw. The bug affects both DeepSeek Web and API, and community reports indicate it also appears in third-party deployments, suggesting it stems from model hallucination rather than implementation error.

telegram · zaihuapd · May 14, 13:15

**Background**: Session isolation is a security mechanism that ensures each user's conversation data remains separate and inaccessible to others. In AI chatbots, proper isolation prevents cross-user data leakage. The DeepSeek bug exploits the model's tendency to continue an incomplete thought (triggered by '<think') by generating content from other sessions, effectively bypassing session boundaries.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/shannon-torcato_i-tested-an-ai-chatbot-on-a-website-last-activity-7426978937877991424-nBb2">AI Chatbot Security Flaw: Session Isolation and Data Exposure | Shannon Torcato posted on the topic | LinkedIn</a></li>
<li><a href="https://proton.me/blog/deepseek">Using DeepSeek ? Here's why your privacy is at stake | Proton | Proton</a></li>
<li><a href="https://www.wired.com/story/deepseek-ai-china-privacy-data/">DeepSeek ’s Popular AI App Is Explicitly Sending US Data to... | WIRED</a></li>

</ul>
</details>

**Discussion**: Community comments note that third-party deployments also exhibit the bug, indicating it is a model hallucination issue rather than a system flaw. The discussion reflects concern over the widespread nature of the vulnerability and the potential for data exposure across different implementations.

**Tags**: `#security`, `#vulnerability`, `#DeepSeek`, `#data leak`, `#AI`

---

<a id="item-6"></a>
## [vLLM v0.21.0: Deprecates Transformers v4, Adds KV Offload and Blackwell Backend](https://github.com/vllm-project/vllm/releases/tag/v0.21.0) ⭐️ 8.0/10

vLLM v0.21.0 officially deprecates transformers v4, requiring migration to v5, and mandates a C++20-compatible compiler. It introduces KV offload with Hybrid Memory Allocator (HMA), speculative decoding with reasoning budget, and a new TOKENSPEED_MLA attention backend for Blackwell GPUs. This release introduces breaking changes that force users to update dependencies while delivering major performance and capability improvements. KV offload with HMA reduces memory waste in hybrid models, speculative decoding with reasoning budget improves inference for reasoning models, and the Blackwell backend enables efficient inference on NVIDIA's latest architecture, lowering inference costs and expanding vLLM's applicability. Transformers v4 support is deprecated; users must migrate to transformers v5 (tested with >4.46). The C++20 requirement may affect platforms with older compilers. KV offload now integrates HMA with sliding window group support, improving memory utilization for hybrid models like Gemma-2. Speculative decoding respects reasoning budgets, enabling correct speculative decoding for models such as DeepSeek-R1. The TOKENSPEED_MLA backend is designed for DeepSeek-R1 and Kimi-K25 on Blackwell GPUs (SM100+).

github · khluu · May 14, 23:15

**Background**: vLLM is an open-source high-throughput LLM inference engine. Transformers v4 is a widely used library, but vLLM is moving to transformers v5 for better support. Hybrid Memory Allocator (HMA) addresses memory waste in models with different attention layers, such as sliding window and full attention. Speculative decoding uses a smaller draft model to generate tokens quickly, verified by the large model, improving throughput. MLA (Multi-head Latent Attention) is an efficient attention mechanism used by DeepSeek models.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/vllm-project/vllm/issues/11382">[RFC]: Hybrid Memory Allocator · Issue #11382 · vllm-project/vllm</a></li>
<li><a href="https://pytorch.org/blog/hybrid-models-as-first-class-citizens-in-vllm/">Hybrid Models as First-Class Citizens in vLLM – PyTorch</a></li>
<li><a href="https://docs.vllm.ai/en/latest/design/attention_backends/">Attention Backend Feature Support - vLLM</a></li>

</ul>
</details>

**Tags**: `#vllm`, `#LLM inference`, `#transformers`, `#speculative decoding`, `#GPU acceleration`

---

<a id="item-7"></a>
## [Removing Modem and GPS from 2024 Toyota RAV4 Hybrid](https://arkadiyt.com/2026/05/13/removing-the-modem-and-gps-from-my-rav4/) ⭐️ 8.0/10

A detailed guide explains how to physically remove the Data Communication Module (DCM) and GPS from a 2024 RAV4 Hybrid to stop telemetry data transmission. This guide empowers owners to take direct action against unwanted vehicle data collection, highlighting growing privacy concerns and the need for hardware-level control. The removal requires plastic trim pry tools, 8mm and 10mm sockets. Even after modem removal, connecting phone via Bluetooth may still allow telemetry via the phone's internet, while USB connection avoids this.

hackernews · arkadiyt · May 14, 17:08 · [Discussion](https://news.ycombinator.com/item?id=48138136)

**Background**: Modern vehicles often include telematics units that collect and transmit data about driving behavior, location, and vehicle status to manufacturers. Many owners are concerned about privacy and data sharing with third parties like insurance companies. Physical removal of the modem is a radical but effective way to prevent such data transmission.

<details><summary>References</summary>
<ul>
<li><a href="https://www.rav4world.com/threads/how-to-fully-disable-telemetry-and-have-an-air-gapped-car.343029/">How to fully disable telemetry and have an "air-gapped" car | Toyota RAV4 Forums</a></li>
<li><a href="https://www.toyotanation.com/threads/clipping-the-claws-of-the-telematics-unit.1800659/">Clipping the Claws of the Telematics Unit | Toyota Forum</a></li>

</ul>
</details>

**Discussion**: Community comments highlight a caution that Bluetooth connections may still allow data transmission via phone's internet, while USB CarPlay avoids this. Some users share experiences with other vehicles like the Ford Maverick having a dedicated fuse for telematics. There is also discussion about Toyota allegedly sharing data with insurance companies.

**Tags**: `#privacy`, `#vehicle telemetry`, `#right-to-repair`, `#Toyota`, `#hardware modification`

---

<a id="item-8"></a>
## [Antirez unveils DwarfStar4: a focused LLM runtime for DeepSeek 4](https://antirez.com/news/165) ⭐️ 8.0/10

Antirez announced DwarfStar4 (DS4), a small LLM inference runtime optimized for running DeepSeek 4 models locally, with primary support for Metal on high-RAM Macs and NVIDIA CUDA, plus community-maintained AMD ROCm support. DS4 enables efficient local inference of state-of-the-art DeepSeek 4 models, reducing dependency on cloud APIs and fostering privacy and offline usage. Its narrow focus on high-RAM Macs and DGX Spark highlights a niche but growing demand for powerful local LLM runtimes. DS4 requires 96GB of VRAM for DeepSeek 4 models, targets MacBooks with 96GB RAM via Metal, and supports NVIDIA CUDA with special care for the DGX Spark. AMD ROCm support lives in a separate branch because antirez lacks direct hardware access.

hackernews · caust1c · May 14, 22:29 · [Discussion](https://news.ycombinator.com/item?id=48142108)

**Background**: An LLM inference runtime is software that executes a trained model to generate responses, optimizing for speed and memory efficiency. Metal is Apple's GPU programming framework, while ROCm is AMD's open-source compute platform. DeepSeek V4 series includes V4-Pro (1.6T total params, 49B active) and V4-Flash (284B total, 13B active), supporting million-token contexts. Quantization techniques like 'imatrix' reduce memory usage while preserving quality.

<details><summary>References</summary>
<ul>
<li><a href="https://pasqualepillitteri.it/en/news/2253/ds4-antirez-deepseek-v4-flash-inference-engine">DwarfStar4 (DS4) Roadmap by antirez: DeepSeek V4 Flash on Apple Silicon and CUDA</a></li>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Pro">deepseek-ai/DeepSeek-V4-Pro · Hugging Face</a></li>
<li><a href="https://rocm.docs.amd.com/en/docs-6.0.0/what-is-rocm.html">What is ROCm ? — ROCm Documentation</a></li>

</ul>
</details>

**Discussion**: Commenters expressed excitement about DS4's focus on local inference, with some noting it feels close to Claude in quality but slower. There is curiosity about whether less intelligent local models can match cloud models given more time, and speculation about future hardware requirements (e.g., 16GB RAM in a couple of years). The imatrix quantization is praised as better than some other backends.

**Tags**: `#LLM`, `#inference`, `#runtime`, `#DeepSeek`, `#open-source`

---

<a id="item-9"></a>
## [RTX 5090 eGPU Works on M4 MacBook Air for Gaming and LLM](https://scottjg.com/posts/2026-05-05-egpu-mac-gaming/) ⭐️ 8.0/10

A technical deep-dive demonstrates successfully using an NVIDIA RTX 5090 eGPU with an M4 MacBook Air via Thunderbolt 5 for gaming and LLM inference, overcoming Apple Silicon's official lack of eGPU support. This breakthrough enables high-end gaming and dramatically faster LLM prompt processing on Macs, previously impossible on Apple Silicon, potentially expanding the Mac's appeal to gamers and AI practitioners. The setup uses a Gigabyte AORUS RTX 5090 AI BOX enclosure over Thunderbolt 5, requiring VM passthrough and custom drivers for compute-only acceleration, but still limited by the 1.5 GB memory window for GPU direct access.

hackernews · allenleee · May 14, 15:47 · [Discussion](https://news.ycombinator.com/item?id=48137145)

**Background**: Apple Silicon Macs do not officially support external GPUs for graphics acceleration; only Intel-based Macs and AMD eGPUs were previously supported. However, Apple has approved third-party drivers allowing NVIDIA eGPUs to run on Apple Silicon for compute tasks like AI, but not for graphics. Thunderbolt 5 provides high bandwidth (up to 80 Gbps) necessary for eGPU performance, and the RTX 5090 is NVIDIA's latest flagship GPU with 32 GB VRAM.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/macoclock/why-dont-macs-with-apple-silicon-support-egpu-db13a705512c">Why Don’t Macs With Apple Silicon Support eGPU ? | Medium</a></li>
<li><a href="https://apple.gadgethacks.com/news/apple-silicon-egpu-support-explained-compute-only-not-graphics/">Apple Silicon eGPU Support Explained: Compute... :: Gadget Hacks</a></li>
<li><a href="https://egpu.io/forums/thunderbolt-enclosures/unboxing-gigabyte-aorus-rtx-5090-ai-box-thunderbolt-5-water-cooled-egpu/">[Unboxing] Gigabyte AORUS RTX 5090 AI BOX Thunderbolt 5 Wate...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed excitement, with many noting the LLM inference improvements as more practical than gaming. Some discussed MoltenVK limitations and macOS deprecation of OpenGL. There were also comments praising the workaround and hoping Apple would eventually provide better eGPU support.

**Tags**: `#eGPU`, `#Apple Silicon`, `#gaming`, `#LLM inference`, `#Mac`

---

<a id="item-10"></a>
## [New Nginx exploit with specific rewrite/set preconditions](https://github.com/DepthFirstDisclosures/Nginx-Rift) ⭐️ 8.0/10

A proof-of-concept exploit for Nginx, named Nginx-Rift, was published on GitHub, exploiting a vulnerability triggered by specific rewrite and set directives, with an optional ASLR bypass. This vulnerability, though requiring preconditions, could allow remote code execution in Nginx, affecting a massive number of servers; the active community discussion clarifies mitigation strategies and highlights the importance of defense-in-depth. The exploit requires a rewrite directive with a question mark in the replacement string, followed by a set directive referencing a regex capture group (e.g., set $var $1). The published proof-of-concept disables ASLR, but the author claims a reliable ASLR bypass is possible.

hackernews · hetsaraiya · May 14, 17:17 · [Discussion](https://news.ycombinator.com/item?id=48138268)

**Background**: Nginx's rewrite directive modifies request URIs using regular expressions, while the set directive assigns variables. ASLR (Address Space Layout Randomization) randomizes memory addresses to hinder exploitation; disabling it simplifies exploits but is not typical in production. Without ASLR bypass, exploitation is significantly harder.

<details><summary>References</summary>
<ul>
<li><a href="https://andy.codes/blog/security-articles/2025-11-02-exploit-mitigation-aslr.html">2025-11-02 - How to Bypass Basic Exploit Mitigation - Part ...</a></li>

</ul>
</details>

**Discussion**: The community debated the exploit's severity: some downplay it due to preconditions and the PoC's ASLR disablement, while others note the author's ASLR bypass claim and stress the importance of patching. Mitigation using named captures instead of unnamed ones was highlighted.

**Tags**: `#nginx`, `#security`, `#exploit`, `#vulnerability`

---

<a id="item-11"></a>
## [MIT President Warns on Funding and Talent Pipeline](https://president.mit.edu/writing-speeches/video-transcript-message-president-kornbluth-about-funding-and-talent-pipeline) ⭐️ 8.0/10

MIT President Sally Kornbluth released a video message addressing challenges in research funding and the talent pipeline, sparking broad community discussion on systemic issues in academia. This message highlights critical issues affecting the future of academic research and the pipeline of skilled talent, which directly impacts industries like software engineering and AI/ML. The video transcript emphasizes financial policy and grant declines, noting that unfunded students are less likely to accept admission offers, threatening the talent pipeline.

hackernews · dmayo · May 14, 14:51 · [Discussion](https://news.ycombinator.com/item?id=48136262)

**Background**: The talent pipeline refers to the flow of students and researchers from academia into industry and academia itself. Declining federal funding and long, poorly paid PhD programs are causing many graduates to leave academia, which could lead to a shortage of skilled researchers and innovators.

**Discussion**: Commenters express widespread disillusionment with academia, citing grueling PhD programs and poor job prospects. Some argue the system is broken and a generational reset is underway, while others note that PhDs leaving academia is not necessarily a waste but shifts talent to industry. A few comments highlight China's rise in higher education.

**Tags**: `#academia`, `#research funding`, `#talent pipeline`, `#MIT`, `#higher education`

---

<a id="item-12"></a>
## [US Clears H200 Sales to China; Nvidia CEO Visits to Boost Deals](https://www.reuters.com/business/retail-consumer/us-clears-h200-chip-sales-10-china-firms-nvidia-ceo-looks-breakthrough-2026-05-14/) ⭐️ 8.0/10

The US Commerce Department has approved about 10 Chinese companies, including Alibaba, Tencent, ByteDance, and JD.com, to purchase Nvidia's H200 chips, with individual customers allowed up to 75,000 units. Nvidia CEO Jensen Huang is visiting China to facilitate the deals, though no deliveries have been completed yet. This development signals a potential easing of AI chip trade restrictions between the US and China, impacting the global AI hardware supply chain. It also highlights the delicate balance Chinese firms must strike between importing advanced chips and developing domestic AI alternatives. The H200 is based on Nvidia's Hopper architecture and features 141 GB of HBM3e memory with 4.8 TB/s bandwidth, nearly double the capacity of the H100. However, some Chinese firms are exercising caution under guidance from Beijing, and no chips have been shipped yet.

telegram · zaihuapd · May 14, 08:57

**Background**: The Nvidia H200 is a high-end GPU designed for AI and HPC workloads, first announced in 2023 and launched in 2024. Previous US export controls restricted sales of advanced chips like the A100 and H100 to China, leading Nvidia to develop slower variants like the H800. The H200 represents a further step in the ongoing US-China tech rivalry.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/data-center/h200/">NVIDIA H200 GPU</a></li>
<li><a href="https://www.runpod.io/articles/guides/nvidia-h200-gpu">Nvidia H200 GPU: Specs, VRAM, Price, and AI Performance</a></li>

</ul>
</details>

**Tags**: `#AI chips`, `#geopolitics`, `#Nvidia`, `#China tech`, `#semiconductor trade`

---

<a id="item-13"></a>
## [ChatGPT Android APK Teardown Reveals Codex Remote Desktop Control](https://t.me/zaihuapd/41388) ⭐️ 8.0/10

A teardown of the ChatGPT Android app version 1.2026.125 reveals strings indicating OpenAI is building a remote desktop control feature using Codex, allowing mobile users to find, reconnect, and control desktop sessions. The feature is still in development with no release date announced. This feature could significantly streamline developer workflows by enabling remote coding and desktop management from a mobile device, expanding Codex's utility beyond the desktop environment. It also signals OpenAI's push to make AI-powered coding agents more accessible and portable. The APK strings mention features like finding and reconnecting remote sessions, and require the desktop to be logged into the same account. The feature is not yet available in a preview build, and its official launch timeline is unknown.

telegram · zaihuapd · May 14, 21:48

**Background**: OpenAI Codex is a suite of AI-powered coding agents designed to automate software engineering tasks, such as building features, refactoring, and migrations. It can run locally via Codex CLI or within IDEs like VS Code. This remote control feature would allow users to manage Codex sessions on their desktop from an Android device, adding a new layer of flexibility.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/codex/">Codex | AI Coding Partner from OpenAI</a></li>
<li><a href="https://github.com/openai/codex">GitHub - openai/codex: Lightweight coding agent that runs in ...</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#Codex`, `#ChatGPT`, `#remote control`, `#APK teardown`

---

<a id="item-14"></a>
## [China in Talks with Boeing for Up to 500 737 MAX Jets](https://t.me/zaihuapd/41389) ⭐️ 8.0/10

China and Boeing are negotiating a potential order of up to 500 Boeing 737 MAX jets, which would be the first major Chinese order in nearly a decade. The deal is expected to be announced around President Trump's visit to China. This order could signal a thaw in US-China trade relations and provide a major boost to Boeing's 737 MAX program, which has faced significant challenges including the global grounding after two fatal crashes. It also highlights China's growing influence in the aviation market. The negotiations also include about 100 wide-body aircraft such as the Boeing 787 and 777X, though those may be announced separately. The deal is not yet finalized, and whether it will result in a binding commitment remains under discussion.

telegram · zaihuapd · May 15, 01:09

**Background**: The Boeing 737 MAX is a narrow-body aircraft family that was grounded worldwide from March 2019 to late 2020 after two fatal crashes, with China being the first to ground it. The 777X is a wide-body twin-engine jet with folding wingtips, currently delayed and expected to enter service in 2027. Wide-body aircraft have two aisles and higher passenger capacity, typically used for long-haul international flights.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Boeing_777X">Boeing 777X - Wikipedia Images 777X - The Boeing Company Confirmed: Boeing 777X To Enter Service In 2027 After 7-Year ... Why The Boeing 777X Is Worth Waiting And Waiting And ... - Forbes Lufthansa’s 1st Boeing 777X is now in flight testing Boeing 777X Set for 2027 Debut After Costly Delays and ... Boeing 777X News Room - Latest news and breaking stories ...</a></li>
<li><a href="https://www.boeing.com/commercial/777x">777X - The Boeing Company Confirmed: Boeing 777X To Enter Service In 2027 After 7-Year ... Why The Boeing 777X Is Worth Waiting And Waiting And ... - Forbes Lufthansa’s 1st Boeing 777X is now in flight testing Boeing 777X Set for 2027 Debut After Costly Delays and ... Boeing 777X News Room - Latest news and breaking stories ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Wide-body_aircraft">Wide-body aircraft</a></li>

</ul>
</details>

**Tags**: `#aviation`, `#trade`, `#US-China relations`, `#Boeing`, `#737 MAX`

---

<a id="item-15"></a>
## [Anima: 2B Parameter Open-Source Anime Text-to-Image Model](https://civitai.com/models/2458426/anima) ⭐️ 8.0/10

CircleStone Labs and Comfy Org have released Anima, a 2-billion-parameter open-source text-to-image model specialized for anime and non-realistic art, trained on millions of real images without synthetic data. This release fills a gap in the open-source AI ecosystem for high-quality, specialized anime generation, enabling artists and developers to create anime-style content with greater control and attribution respecting copyrighted styles. The model is currently available for non-commercial use only on platforms like Civitai and Hugging Face, and it uses approximately 800,000 non-anime art images alongside millions of anime images for training.

telegram · zaihuapd · May 15, 03:00

**Background**: Text-to-image models generate images from textual descriptions, and open-source models allow community customization. Anima is built on the transformer architecture and competes with models like Stable Diffusion, but focuses specifically on anime aesthetics, a niche with high demand in the generative AI community.

<details><summary>References</summary>
<ul>
<li><a href="https://www.comfy.org/">Comfy Org - Professional Control of Visual AI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Civitai">Civitai</a></li>
<li><a href="https://github.com/Comfy-Org/">Comfy Org - GitHub</a></li>

</ul>
</details>

**Tags**: `#AI`, `#text-to-image`, `#anime`, `#open-source`, `#generative-models`

---