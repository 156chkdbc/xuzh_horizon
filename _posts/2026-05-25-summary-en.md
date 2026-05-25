---
layout: default
title: "Horizon Summary: 2026-05-25 (EN)"
date: 2026-05-25
lang: en
---

> From 34 items, 8 important content pieces were selected

---

1. [Official Telegram on APKPure Found with Spyware Backdoor](#item-1) ⭐️ 9.0/10
2. [Memory now accounts for nearly two-thirds of AI chip costs](#item-2) ⭐️ 8.0/10
3. [Constraint Decay: LLM Agents Fail Under Architectural Rules](#item-3) ⭐️ 8.0/10
4. [Microsoft open-sources earliest known DOS source code](#item-4) ⭐️ 8.0/10
5. [Greg Brockman Interview: OpenAI's History and Leadership](#item-5) ⭐️ 8.0/10
6. [AMD drops Linux support from free Vivado tier in 2026.1](#item-6) ⭐️ 8.0/10
7. [Huawei Proposes 'Tao's Law' for Semiconductor Time Scaling](#item-7) ⭐️ 8.0/10
8. [Epic Reveals Unreal Engine 6, Rocket League Jumps from UE3 to UE6](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Official Telegram on APKPure Found with Spyware Backdoor](https://x.com/EricParker/status/2058411298195661221) ⭐️ 9.0/10

A repackaged version of Telegram 12.6.5 distributed via APKPure was found to contain a spyware framework called DataCollector, capable of stealing chats, contacts, photos, and other sensitive data. The malicious code, embedded in a classes3.dex file with over 3000 lines, exfiltrates data encrypted with AES-GCM to a remote C2 server at 38.190.225.166. This supply-chain attack on a widely-used messaging app highlights the risks of downloading software from third-party app stores, potentially compromising countless users' privacy and security. It underscores the need for stronger scrutiny and verification of software distribution channels. The malicious version was re-signed and repackaged while appearing as the official Telegram app. The DataCollector spyware uses AES-GCM encryption for data exfiltration, making detection difficult, and communicates with a command-and-control server located at the given IP address.

telegram · zaihuapd · May 24, 11:38

**Background**: APKPure is a third-party Android app store that distributes apps not always verified by official sources. A supply-chain attack occurs when a legitimate software distribution channel is compromised to inject malware. In Android apps, code is often stored in .dex (Dalvik Executable) files, which are executed by the Android Runtime. AES-GCM is an authenticated encryption mode that provides both confidentiality and integrity. Command-and-control (C2) servers are used by attackers to receive stolen data and send instructions to infected devices.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Block_cipher_mode_of_operation">Block cipher mode of operation - Wikipedia</a></li>
<li><a href="https://source.android.com/docs/core/runtime/dex-format">Dalvik executable format | Android Open Source Project</a></li>
<li><a href="https://en.wikipedia.org/wiki/Botnet">Botnet - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#security`, `#malware`, `#telegram`, `#supply-chain attack`, `#spyware`

---

<a id="item-2"></a>
## [Memory now accounts for nearly two-thirds of AI chip costs](https://epoch.ai/data-insights/ai-chip-component-cost-shares) ⭐️ 8.0/10

According to Epoch AI data, memory has grown to nearly two-thirds of the total cost of AI chip components, highlighting a severe cost bottleneck in AI hardware. This cost concentration means that without memory price reductions, AI hardware affordability will remain limited, potentially slowing the scaling of AI inference and training. It also underscores the need for innovations in memory technology or supply expansion. The memory cost share includes High Bandwidth Memory (HBM) and DRAM, driven by skyrocketing demand for AI accelerators. While technical innovations in compute are advancing, memory costs have surged, creating a disproportionate expense.

hackernews · intelkishan · May 24, 16:31 · [Discussion](https://news.ycombinator.com/item?id=48258684)

**Background**: AI chips, such as GPUs and specialized accelerators, require large amounts of fast memory to feed data to compute units. High Bandwidth Memory (HBM) is a 3D-stacked DRAM technology that provides high bandwidth but is expensive to produce. The memory bandwidth bottleneck is a well-known challenge in AI workloads, where loading model parameters from memory often limits performance.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://winbuzzer.com/2026/05/11/micron-memory-bottlenecks-threaten-ai-inference-efficiency-xcxwbn/">Micron Warns Memory Bottlenecks Threaten AI Inference</a></li>

</ul>
</details>

**Discussion**: Commenters noted that this cost trend implies a potential 3x hardware cost reduction if DRAM supply meets demand, but current high prices are hurting consumers and gamers. Some users reported that RAM prices have more than quadrupled in recent years, and many are postponing upgrades.

**Tags**: `#AI hardware`, `#memory costs`, `#semiconductors`, `#supply chain`, `#economics`

---

<a id="item-3"></a>
## [Constraint Decay: LLM Agents Fail Under Architectural Rules](https://arxiv.org/abs/2605.06445) ⭐️ 8.0/10

A new study published on arXiv identifies a phenomenon called 'constraint decay,' where LLM-based coding agents perform well on unconstrained code generation but their performance degrades significantly when explicit architectural rules are introduced, with assertion pass rates dropping by an average of 30 points. This finding has critical implications for using LLM agents in production-grade backend development, suggesting that while they are reliable for rapid prototyping, they remain unreliable for complex, rule-intensive real-world applications. It also highlights a fundamental limitation that future model improvements must address. The study evaluated multiple LLMs and found that constraint decay manifests as code that behaves incorrectly under specific database conditions or query shapes, not as visible crashes. The paper notes that even capable models lose an average of 30 points in assertion pass rates when constraints accumulate.

hackernews · wek · May 24, 12:55 · [Discussion](https://news.ycombinator.com/item?id=48256912)

**Background**: LLM agents are AI systems that can generate code from natural language prompts, increasingly used for software development. However, real-world backend systems require adherence to specific architectural rules such as database schemas, ORM patterns, and style guides. This study systematically investigates how well LLM agents handle such constraints.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48256912">Constraint Decay: The Fragility of LLM Agents in Back End ...</a></li>
<li><a href="https://byteiota.com/llm-agent-constraint-decay-backend-code/">LLM Agent Constraint Decay: Why Real Backends Break AI Code</a></li>

</ul>
</details>

**Discussion**: Commenters shared personal experiences aligning with the study's findings. One noted that complex projects require adding more constraints, and another observed that agents perform worse when forced into architectural patterns, though including constraints incrementally helps. A criticism was that the study did not test the most advanced models due to cost, potentially underestimating best-case performance.

**Tags**: `#LLM agents`, `#code generation`, `#backend development`, `#AI reliability`, `#software engineering`

---

<a id="item-4"></a>
## [Microsoft open-sources earliest known DOS source code](https://arstechnica.com/gadgets/2026/04/microsoft-open-sources-the-earliest-dos-source-code-discovered-to-date/) ⭐️ 8.0/10

Microsoft open-sourced the earliest known version of DOS source code, which was painstakingly reconstructed from paper printouts by a preservation team led by Yufeng Gao and Rich Cini. This release gives historians and developers unprecedented access to the foundational code of the PC revolution, preserving a crucial piece of computing history that was nearly lost. The source code was transcribed from paper printouts stored in Tim Paterson's garage, as no digital copy existed; modern OCR struggled with the aged print quality, making manual transcription necessary.

hackernews · DamnInteresting · May 24, 01:21 · [Discussion](https://news.ycombinator.com/item?id=48253386)

**Background**: DOS (Disk Operating System) was the operating system that powered early IBM PCs and their compatibles, originally written in assembly language by Tim Paterson in 1980. The source code was never stored digitally, and only paper printouts survived for decades. This open-source release allows the community to study the earliest version of the software that launched the PC era.

**Discussion**: Commenters expressed gratitude to Microsoft (e.g., jmward01: 'It is rare that I say this but, thanks MS!') and admiration for the modest amount of assembly code that launched a company (nananana9). Others noted the reconstruction effort from OCR'd printouts and confirmed the code runs smoothly in DOSBox (wpnx).

**Tags**: `#Microsoft`, `#DOS`, `#open source`, `#software history`, `#preservation`

---

<a id="item-5"></a>
## [Greg Brockman Interview: OpenAI's History and Leadership](https://fs.blog/knowledge-project-podcast/greg-brockman/) ⭐️ 8.0/10

Greg Brockman, co-founder of OpenAI, gives an in-depth interview on The Knowledge Project podcast discussing the company's history, leadership changes including Sam Altman's firing and rehiring, and his personal narrative. This interview provides an insider perspective on pivotal events at OpenAI, the leading AI research organization, offering insights into its shifting leadership and strategic direction. It is significant for understanding the internal dynamics that shaped the development of advanced AI systems. The interview covers topics such as the early days of OpenAI, the transition from non-profit to capped-profit, and the recent leadership crisis involving Sam Altman and Ilya Sutskever. Brockman's account is partly corroborated by his personal diary, which was made public as part of Elon Musk's lawsuit against OpenAI.

hackernews · prakashqwerty · May 24, 08:29 · [Discussion](https://news.ycombinator.com/item?id=48255593)

**Background**: Greg Brockman is a co-founder and former president of OpenAI, a leading artificial intelligence research laboratory. The organization has experienced significant leadership turmoil, including the temporary ousting of CEO Sam Altman in late 2023, which was followed by employee protests and Altman's reinstatement. This interview offers Brockman's personal perspective on these events.

**Discussion**: Comments on the interview are mixed: some find the focus on corporate politics boring, while others point to Brockman's diary entries as revealing personal motivations. A notable query is why no one asks about Ilya Sutskever's role in the Sam Altman firing and subsequent support for Altman's reinstatement.

**Tags**: `#OpenAI`, `#AI`, `#Greg Brockman`, `#interview`, `#leadership`

---

<a id="item-6"></a>
## [AMD drops Linux support from free Vivado tier in 2026.1](https://adaptivesupport.amd.com/s/question/0D5Pd00001YQLdMKAX/why-is-vivado-20261-dropping-linux-support-for-free-tier-?language=en_US) ⭐️ 8.0/10

AMD's Vivado 2026.1 introduces a new tiered licensing model that removes Linux support from the free Basic tier, while Windows remains supported. This change risks alienating students, hobbyists, and developers who rely on Linux, potentially shrinking the FPGA community and driving users to competitors like Lattice or Intel. The free Basic tier now only supports Windows, while paid tiers retain Linux; AMD claims the move enables more flexible pricing, but users see it as a regression from the previous all-platform free WebPACK edition.

hackernews · zdw · May 24, 04:14 · [Discussion](https://news.ycombinator.com/item?id=48254309)

**Background**: Vivado is AMD's (formerly Xilinx's) FPGA design suite. The free WebPACK edition historically supported both Windows and Linux, enabling broad access for education and hobbyists. The new tiered model replaces WebPACK with a Basic tier that restricts Linux, causing backlash.

<details><summary>References</summary>
<ul>
<li><a href="https://www.amd.com/en/products/software/adaptive-socs-and-fpgas/vivado.html">AMD Vivado™ Design Suite</a></li>
<li><a href="https://pcbsync.com/xilinx-vivado-editions/">Vivado WebPACK vs Standard vs Enterprise: Which Edition Do You Actually Need? - PCBSync</a></li>

</ul>
</details>

**Discussion**: Users express strong dissatisfaction, with many threatening to switch to Lattice or Altera. Long-time AMD users argue the move harms ecosystem growth, and educators plan to change vendors. Some note that paid licenses remain cumbersome and expensive.

**Tags**: `#FPGA`, `#Vivado`, `#Linux`, `#AMD`, `#hardware design`

---

<a id="item-7"></a>
## [Huawei Proposes 'Tao's Law' for Semiconductor Time Scaling](https://www.peopleapp.com/column/30052220655-500007509895) ⭐️ 8.0/10

Huawei unveiled the Tau (τ) Scaling Law, also known as 'Tao's Law', at the 2026 International Circuit and Systems Symposium, proposing to replace geometric scaling with time scaling for semiconductor advancement. The company has already designed and mass-produced 381 chips based on this principle over the past six years, and plans to release a new Kirin chip using logic folding technology this autumn. Tao's Law offers a potential path to continue semiconductor performance scaling beyond Moore's Law, which is approaching physical limits. If successful, it could reduce reliance on extreme ultraviolet lithography and enable Chinese chipmakers to achieve high-density chips despite export restrictions. The law focuses on reducing time constants to optimize devices, circuits, and systems jointly, rather than shrinking transistor dimensions. Huawei claims that by 2031, chips designed under Tao's Law can achieve transistor density equivalent to 1.4nm process technology.

telegram · zaihuapd · May 25, 01:35

**Background**: Moore's Law, which predicted doubling of transistors every two years, has slowed as geometric scaling (shrinking transistor size) faces physical and economic barriers. Dennard scaling, which kept power density constant with scaling, broke down in the mid-2000s. Tao's Law proposes time scaling — improving performance by reducing signal propagation delays through architectural and circuit innovations, rather than solely relying on smaller transistors.

<details><summary>References</summary>
<ul>
<li><a href="https://www.gizmochina.com/2026/05/25/huawei-proposes-tao-law-as-alternative-to-moores-law-first-logic-folding-chip-arrives-this-autumn/">Huawei proposes “Tao Law” as alternative to Moore’s Law, first logic-folding chip arrives this autumn</a></li>
<li><a href="https://www.globaltimes.cn/page/202605/1361841.shtml">Huawei unveils new semiconductor law, charting fresh... - Global Times</a></li>
<li><a href="https://en.wikipedia.org/wiki/Moore's_law">Moore's law - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#Huawei`, `#Moore's Law`, `#chip design`, `#Tao's Law`

---

<a id="item-8"></a>
## [Epic Reveals Unreal Engine 6, Rocket League Jumps from UE3 to UE6](https://www.pcgamer.com/gaming-industry/epic-reveals-first-unreal-engine-6-game-and-its-not-fortnite/) ⭐️ 8.0/10

Epic Games announced Unreal Engine 6 at the Paris Rocket League Championship Series, confirming that Rocket League will skip UE4 and UE5 to upgrade directly from UE3 to UE6. A teaser trailer showed an updated version of Rocket League running in UE6. Unreal Engine 6 represents a major next step from UE5, with potential improvements in performance and new features like Nanite v2 and Lumen 2.0, addressing longstanding optimization criticisms. The jump also signals Epic's ongoing push toward the metaverse, as the teaser included connections to Fortnite and other games. Rocket League has been running on UE3 since its 2015 release, making this cross-generational upgrade comparable to a sequel. UE5 has faced criticism for performance issues on PC, and UE6 is expected to address these with enhanced rendering techniques and AI tools, though no release date has been announced.

telegram · zaihuapd · May 25, 02:20

**Background**: Unreal Engine is a game engine developed by Epic Games, widely used in gaming, film, and other industries. UE5, released in 2022, introduced technologies like Nanite and Lumen, but has been criticized for optimization issues on PC. UE6 is the next iteration, announced in May 2026 as an evolution of Epic's metaverse strategy.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Unreal_Engine_6">Unreal Engine 6</a></li>
<li><a href="https://www.ign.com/articles/unreal-engine-6-revealed-as-rocket-league-gets-a-new-coat-of-paint">Unreal Engine 6 Revealed - IGN</a></li>

</ul>
</details>

**Tags**: `#Unreal Engine`, `#Game Development`, `#Epic Games`, `#Rocket League`, `#Metaverse`

---