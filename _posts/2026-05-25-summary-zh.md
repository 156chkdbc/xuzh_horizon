---
layout: default
title: "Horizon Summary: 2026-05-25 (ZH)"
date: 2026-05-25
lang: zh
---

> From 34 items, 8 important content pieces were selected

---

1. [APKPure 上的 Telegram 官方版被发现植入间谍后门](#item-1) ⭐️ 9.0/10
2. [内存成本已占 AI 芯片成本的近三分之二](#item-2) ⭐️ 8.0/10
3. [约束衰减：LLM 代理在架构规则下表现不佳](#item-3) ⭐️ 8.0/10
4. [微软开源已知最早的 DOS 源代码](#item-4) ⭐️ 8.0/10
5. [格雷格·布罗克曼专访：OpenAI 历史与领导层变动](#item-5) ⭐️ 8.0/10
6. [AMD 在 Vivado 2026.1 免费版中取消 Linux 支持](#item-6) ⭐️ 8.0/10
7. [华为提出半导体时间缩微‘韬定律’](#item-7) ⭐️ 8.0/10
8. [Epic 公布虚幻引擎 6，《火箭联盟》从 UE3 直接升级至 UE6](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [APKPure 上的 Telegram 官方版被发现植入间谍后门](https://x.com/EricParker/status/2058411298195661221) ⭐️ 9.0/10

在 APKPure 上分发的 Telegram 12.6.5 版本被发现重新签名打包，植入了名为 DataCollector 的间谍框架，可窃取聊天记录、通讯录、照片等敏感数据。恶意代码嵌入在超过 3000 行的 classes3.dex 文件中，数据经 AES-GCM 加密后上传至远程 C2 服务器 38.190.225.166。 这种针对广泛使用的消息应用的供应链攻击凸显了从第三方应用商店下载软件的风险，可能危及无数用户的隐私和安全。它强调了加强对软件分发渠道审查和验证的必要性。 恶意版本被重新签名打包，但外观上与官方 Telegram 应用一致。DataCollector 间谍软件使用 AES-GCM 加密进行数据外泄，增加了检测难度，并与指定 IP 地址的命令与控制服务器通信。

telegram · zaihuapd · May 24, 11:38

**背景**: APKPure 是一个第三方 Android 应用商店，分发未经官方来源验证的应用。供应链攻击是指合法软件分发渠道被攻陷以注入恶意软件。在 Android 应用中，代码通常存储在.dex（Dalvik 可执行）文件中，由 Android 运行时执行。AES-GCM 是一种认证加密模式，提供机密性和完整性。命令与控制（C2）服务器被攻击者用于接收窃取的数据并向受感染设备发送指令。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Block_cipher_mode_of_operation">Block cipher mode of operation - Wikipedia</a></li>
<li><a href="https://source.android.com/docs/core/runtime/dex-format">Dalvik executable format | Android Open Source Project</a></li>
<li><a href="https://en.wikipedia.org/wiki/Botnet">Botnet - Wikipedia</a></li>

</ul>
</details>

**标签**: `#security`, `#malware`, `#telegram`, `#supply-chain attack`, `#spyware`

---

<a id="item-2"></a>
## [内存成本已占 AI 芯片成本的近三分之二](https://epoch.ai/data-insights/ai-chip-component-cost-shares) ⭐️ 8.0/10

根据 Epoch AI 的数据，内存成本已升至 AI 芯片组件总成本的近三分之二，凸显了 AI 硬件中严重的成本瓶颈。 这种成本集中意味着，如果内存价格不下降，AI 硬件的可负担性将仍然受限，可能减缓 AI 推理和训练的规模扩展。同时，这也凸显了内存技术创新或供应扩张的必要性。 内存成本份额包括高带宽内存（HBM）和 DRAM，由 AI 加速器需求飙升驱动。尽管计算技术不断创新，内存成本却大幅上涨，造成了不成比例的费用。

hackernews · intelkishan · May 24, 16:31 · [社区讨论](https://news.ycombinator.com/item?id=48258684)

**背景**: AI 芯片（如 GPU 和专用加速器）需要大量快速内存来向计算单元提供数据。高带宽内存（HBM）是一种 3D 堆叠 DRAM 技术，可提供高带宽但生产成本昂贵。内存带宽瓶颈是 AI 工作负载中众所周知的挑战，从内存加载模型参数常常限制性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://winbuzzer.com/2026/05/11/micron-memory-bottlenecks-threaten-ai-inference-efficiency-xcxwbn/">Micron Warns Memory Bottlenecks Threaten AI Inference</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，这一成本趋势意味着如果 DRAM 供应满足需求，硬件成本可能降低 3 倍，但目前的高价格正在伤害消费者和游戏玩家。一些用户报告称，近几年内存价格已上涨超过四倍，许多人因此推迟升级。

**标签**: `#AI hardware`, `#memory costs`, `#semiconductors`, `#supply chain`, `#economics`

---

<a id="item-3"></a>
## [约束衰减：LLM 代理在架构规则下表现不佳](https://arxiv.org/abs/2605.06445) ⭐️ 8.0/10

一项发表在 arXiv 上的新研究识别出名为‘约束衰减’的现象：基于 LLM 的编码代理在无约束代码生成中表现良好，但当引入明确的架构规则时，其性能显著下降，断言通过率平均下降 30 个百分点。 这一发现对在生产级后端开发中使用 LLM 代理具有关键意义，表明虽然它们适合快速原型开发，但在复杂、规则密集的真实应用中仍不可靠。它也凸显了未来模型改进必须解决的根本性限制。 该研究评估了多个 LLM，发现约束衰减表现为代码在特定数据库条件或查询形状下行为异常，而非明显的崩溃。论文指出，随着约束累积，即使是强大的模型其断言通过率也平均下降 30 个百分点。

hackernews · wek · May 24, 12:55 · [社区讨论](https://news.ycombinator.com/item?id=48256912)

**背景**: LLM 代理是能够根据自然语言提示生成代码的 AI 系统，越来越多地被用于软件开发。然而，现实世界的后端系统需要遵循特定的架构规则，如数据库模式、ORM 模式和风格指南。本研究系统性地调查了 LLM 代理如何处理这些约束。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48256912">Constraint Decay: The Fragility of LLM Agents in Back End ...</a></li>
<li><a href="https://byteiota.com/llm-agent-constraint-decay-backend-code/">LLM Agent Constraint Decay: Why Real Backends Break AI Code</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了与研究发现一致的个人经验。有人指出复杂项目需要增加更多约束，另有人观察到代理在被迫遵循架构模式时表现更差，但逐步引入约束会有所帮助。批评意见认为，由于成本原因，该研究未测试最先进的模型，可能低估了最佳情况下的性能。

**标签**: `#LLM agents`, `#code generation`, `#backend development`, `#AI reliability`, `#software engineering`

---

<a id="item-4"></a>
## [微软开源已知最早的 DOS 源代码](https://arstechnica.com/gadgets/2026/04/microsoft-open-sources-the-earliest-dos-source-code-discovered-to-date/) ⭐️ 8.0/10

微软开源了已知最早的 DOS 源代码，这些代码由 Yufeng Gao 和 Rich Cini 领导的保护团队通过纸打印件精心重建而成。 此次发布让历史学家和开发人员史无前例地接触到 PC 革命的基础代码，保护了险些丢失的关键计算历史。 源代码是从 Tim Paterson 车库中存放的纸打印件转录而来，因为没有数字副本存在；现代 OCR 软件难以处理年代久远的打印质量，因此需要手动转录。

hackernews · DamnInteresting · May 24, 01:21 · [社区讨论](https://news.ycombinator.com/item?id=48253386)

**背景**: DOS（磁盘操作系统）是驱动早期 IBM PC 及其兼容机的操作系统，最初由 Tim Paterson 于 1980 年用汇编语言编写。源代码从未以数字形式存储，仅存纸打印件保存了数十年。此次开源发布使得社区能够研究启动 PC 时代的最早版本软件。

**社区讨论**: 评论者表达了对微软的感谢（如 jmward01：“我很少这么说，但谢谢微软！”），并对仅用少量汇编代码就创立了一家公司的成就表示钦佩（nananana9）。其他人注意到了从 OCR 打印件重建的努力，并确认代码在 DOSBox 中运行流畅（wpnx）。

**标签**: `#Microsoft`, `#DOS`, `#open source`, `#software history`, `#preservation`

---

<a id="item-5"></a>
## [格雷格·布罗克曼专访：OpenAI 历史与领导层变动](https://fs.blog/knowledge-project-podcast/greg-brockman/) ⭐️ 8.0/10

OpenAI 联合创始人格雷格·布罗克曼在《知识项目》播客中接受深度访谈，讨论了公司历史、包括萨姆·奥尔特曼被解雇及复职在内的领导层变动，以及他的个人经历。 此次访谈提供了对领先 AI 研究机构 OpenAI 关键事件的内部视角，揭示了其领导层变动和战略方向的变化。这对于理解塑造先进 AI 系统发展的内部动态具有重要意义。 访谈涵盖了 OpenAI 的早期、从非营利向有限盈利的转型，以及涉及萨姆·奥尔特曼和伊利亚·苏茨克维尔的近期领导危机。布罗克曼的描述部分由其个人日记佐证，该日记在埃隆·马斯克对 OpenAI 的诉讼中被公开。

hackernews · prakashqwerty · May 24, 08:29 · [社区讨论](https://news.ycombinator.com/item?id=48255593)

**背景**: 格雷格·布罗克曼是领先人工智能研究实验室 OpenAI 的联合创始人兼前总裁。该组织经历了重大领导层动荡，包括 2023 年底 CEO 萨姆·奥尔特曼被暂时罢免，随后员工抗议并恢复其职务。此次访谈提供了布罗克曼对这些事件的个人视角。

**社区讨论**: 对此次访谈的评论褒贬不一：有人认为对公司政治的讨论令人生厌，也有人指出布罗克曼的日记条目揭示了他的个人动机。一个引人注意的问题是，为何无人询问伊利亚·苏茨克维尔在萨姆·奥尔特曼被解雇及随后支持其复职事件中的角色。

**标签**: `#OpenAI`, `#AI`, `#Greg Brockman`, `#interview`, `#leadership`

---

<a id="item-6"></a>
## [AMD 在 Vivado 2026.1 免费版中取消 Linux 支持](https://adaptivesupport.amd.com/s/question/0D5Pd00001YQLdMKAX/why-is-vivado-20261-dropping-linux-support-for-free-tier-?language=en_US) ⭐️ 8.0/10

AMD 的 Vivado 2026.1 引入了新的分层许可模式，从免费 Basic 版中移除了 Linux 支持，而 Windows 仍受支持。 这一变化可能疏远依赖 Linux 的学生、爱好者和开发者，从而缩小 FPGA 社区规模，并可能将用户推向 Lattice 或 Intel 等竞争对手。 免费 Basic 版现在仅支持 Windows，而付费版仍保留 Linux；AMD 声称此举可实现更灵活的定价，但用户认为这是对之前全平台免费 WebPACK 版本的倒退。

hackernews · zdw · May 24, 04:14 · [社区讨论](https://news.ycombinator.com/item?id=48254309)

**背景**: Vivado 是 AMD（前身为 Xilinx）的 FPGA 设计套件。免费的 WebPACK 版本历来支持 Windows 和 Linux，为教育和爱好者提供了广泛访问。新的分层模式用 Basic 版取代了 WebPACK，但限制了 Linux，引发了强烈反对。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.amd.com/en/products/software/adaptive-socs-and-fpgas/vivado.html">AMD Vivado™ Design Suite</a></li>
<li><a href="https://pcbsync.com/xilinx-vivado-editions/">Vivado WebPACK vs Standard vs Enterprise: Which Edition Do You Actually Need? - PCBSync</a></li>

</ul>
</details>

**社区讨论**: 用户表达了强烈不满，许多人威胁要转向 Lattice 或 Altera。长期 AMD 用户认为此举损害了生态系统的成长，教育工作者计划更换供应商。一些人指出付费许可仍然繁琐且昂贵。

**标签**: `#FPGA`, `#Vivado`, `#Linux`, `#AMD`, `#hardware design`

---

<a id="item-7"></a>
## [华为提出半导体时间缩微‘韬定律’](https://www.peopleapp.com/column/30052220655-500007509895) ⭐️ 8.0/10

华为在 2026 年国际电路与系统研讨会上公布了“τ（韬）缩微定律”，提出以时间缩微替代几何缩微来推动半导体发展。过去六年，华为已基于该定律设计并量产了 381 款芯片，并计划今年秋季推出采用逻辑折叠技术的新麒麟芯片。 “韬定律”为在摩尔定律逼近物理极限后继续提升半导体性能提供了潜在路径。如果成功，它可减少对极紫外光刻技术的依赖，并使中国芯片制造商在出口限制下仍能实现高密度芯片。 该定律专注于通过降低时间常数来实现器件、电路和系统的协同优化，而非缩小晶体管尺寸。华为声称，到 2031 年，基于“韬定律”设计的芯片可实现相当于 1.4 纳米制程的晶体管密度。

telegram · zaihuapd · May 25, 01:35

**背景**: 摩尔定律预测晶体管数量每两年翻一番，但随着几何缩微（缩小晶体管尺寸）遇到物理和经济障碍，该定律已经放缓。丹纳德缩放定律（保持功率密度恒定）在 2000 年代中期失效。“韬定律”提出时间缩微——通过架构和电路创新减少信号传播延迟来提升性能，而非单纯依赖更小的晶体管。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.gizmochina.com/2026/05/25/huawei-proposes-tao-law-as-alternative-to-moores-law-first-logic-folding-chip-arrives-this-autumn/">Huawei proposes “Tao Law” as alternative to Moore’s Law, first logic-folding chip arrives this autumn</a></li>
<li><a href="https://www.globaltimes.cn/page/202605/1361841.shtml">Huawei unveils new semiconductor law, charting fresh... - Global Times</a></li>
<li><a href="https://en.wikipedia.org/wiki/Moore's_law">Moore's law - Wikipedia</a></li>

</ul>
</details>

**标签**: `#semiconductor`, `#Huawei`, `#Moore's Law`, `#chip design`, `#Tao's Law`

---

<a id="item-8"></a>
## [Epic 公布虚幻引擎 6，《火箭联盟》从 UE3 直接升级至 UE6](https://www.pcgamer.com/gaming-industry/epic-reveals-first-unreal-engine-6-game-and-its-not-fortnite/) ⭐️ 8.0/10

Epic Games 在巴黎火箭联盟冠军系列赛上宣布了虚幻引擎 6，并确认《火箭联盟》将跳过 UE4 和 UE5，直接从 UE3 升级到 UE6。预告片展示了在 UE6 中运行的更新版《火箭联盟》。 虚幻引擎 6 代表了从 UE5 的重要下一步，可能带来性能提升和新功能（如 Nanite v2 和 Lumen 2.0），解决长期以来的优化批评。这一升级也表明了 Epic 持续推进元宇宙的意图，预告片中包含了与《堡垒之夜》等游戏的关联。 《火箭联盟》自 2015 年发布以来一直运行在 UE3 上，此次跨代升级堪比续作。UE5 在 PC 端因性能问题饱受批评，UE6 预计将通过增强渲染技术和 AI 工具来解决这些问题，但尚未公布发布日期。

telegram · zaihuapd · May 25, 02:20

**背景**: 虚幻引擎是由 Epic Games 开发的游戏引擎，广泛应用于游戏、影视等行业。UE5 于 2022 年发布，引入了 Nanite 和 Lumen 等技术，但因 PC 端优化问题受到批评。UE6 是下一代版本，于 2026 年 5 月公布，是 Epic 元宇宙战略的演进。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Unreal_Engine_6">Unreal Engine 6</a></li>
<li><a href="https://www.ign.com/articles/unreal-engine-6-revealed-as-rocket-league-gets-a-new-coat-of-paint">Unreal Engine 6 Revealed - IGN</a></li>

</ul>
</details>

**标签**: `#Unreal Engine`, `#Game Development`, `#Epic Games`, `#Rocket League`, `#Metaverse`

---