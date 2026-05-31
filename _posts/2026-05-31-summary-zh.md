---
layout: default
title: "Horizon Summary: 2026-05-31 (ZH)"
date: 2026-05-31
lang: zh
---

> From 35 items, 14 important content pieces were selected

---

1. [vLLM v0.22.0：DeepSeek V4 成熟化、MRv2 进展、实验性 Rust 前端](#item-1) ⭐️ 9.0/10
2. [华为提出韬定律：时间缩微替代几何缩微](#item-2) ⭐️ 9.0/10
3. [微软将永久授权 Office 降级为只读模式](#item-3) ⭐️ 8.0/10
4. [领域专长仍是真正的竞争优势](#item-4) ⭐️ 8.0/10
5. [埃森哲以 12 亿美元收购 Ookla 以增强网络智能](#item-5) ⭐️ 8.0/10
6. [Voxel Space（2017）——深入解析《科曼奇》地形渲染算法](#item-6) ⭐️ 8.0/10
7. [Zig ELF 链接器改进带来更快的迭代](#item-7) ⭐️ 8.0/10
8. [Openrsync：OpenBSD 安全版 rsync 实现备受关注](#item-8) ⭐️ 8.0/10
9. [OpenRouter 完成 1.13 亿美元 B 轮融资](#item-9) ⭐️ 8.0/10
10. [教皇利奥的首部通谕抨击技术救世主义](#item-10) ⭐️ 8.0/10
11. [Anthropic 详解 Claude 跨产品沙箱技术](#item-11) ⭐️ 8.0/10
12. [用 Pyodide 和服务工作者在浏览器中运行 Python ASGI 应用](#item-12) ⭐️ 8.0/10
13. [SpaceX 获 41.6 亿美元美军卫星导弹追踪合同](#item-13) ⭐️ 8.0/10
14. [新型 FROST 攻击利用 SSD 计时窥探浏览器活动](#item-14) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [vLLM v0.22.0：DeepSeek V4 成熟化、MRv2 进展、实验性 Rust 前端](https://github.com/vllm-project/vllm/releases/tag/v0.22.0) ⭐️ 9.0/10

vLLM v0.22.0 发布，包含 230 位贡献者的 459 次提交，引入了 DeepSeek V4 成熟支持（含 NVFP4 融合 MoE 和多令牌预测推测解码）、Model Runner V2 的改进以及实验性 Rust 前端。 此版本显著提升了 LLM 推理性能和对模型的支持，尤其是 DeepSeek V4，并尝试用 Rust 加速，对开源 LLM 服务生态产生重要影响。 批次不变推理配合 Cutlass FP8 实现了 28.9% 的端到端延迟降低；新的多层级 KV 缓存卸载框架将卸载范围扩展到磁盘；Rust 前端为实验性功能，并包含数据并行监管器。

github · khluu · May 29, 10:28

**背景**: vLLM 是一个用于快速 LLM 推理和服务的开源库，广泛用于生产环境。DeepSeek V4 是一个大型混合专家模型，需要高效的核，如 NVFP4 融合 MoE 和 MegaMoE。Model Runner V2 是重新设计的推理引擎，旨在提高性能和灵活性。Rust 前端探索使用 Rust 构建底层服务组件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/api/vllm/model_executor/layers/fused_moe/experts/trtllm_nvfp4_moe/">trtllm_ nvfp 4 _ moe - vLLM</a></li>
<li><a href="https://vllm-website-nj3unaiki-inferact-inc.vercel.app/blog/deepseek-v4">DeepSeek V4 in vLLM : Efficient Long-context Attention | vLLM Blog</a></li>
<li><a href="https://docs.vllm.ai/en/stable/api/vllm/models/deepseek_v4/nvidia/ops/prepare_megamoe/">prepare_ megamoe - vLLM</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#DeepSeek`, `#open-source`, `#AI systems`

---

<a id="item-2"></a>
## [华为提出韬定律：时间缩微替代几何缩微](https://t.me/zaihuapd/41648) ⭐️ 9.0/10

华为在 2026 年 IEEE 国际电路与系统研讨会（ISCAS）上提出了韬（τ）缩微定律，主张以时间缩微替代传统的几何缩微作为半导体演进的新原则。该公司声称过去六年已据此设计量产 381 款芯片，并计划于 2026 年秋季推出采用逻辑折叠技术的新麒麟手机芯片。 韬缩微定律可能推动半导体行业从摩尔定律转向优先减少信号传播时间（τ），从而在物理极限下持续提升性能。若经证实，这一方法有望帮助华为及中国芯片产业在地缘政治出口限制下取得突破。 该定律通过器件、电路、芯片到系统的多层级协同优化，专注于降低时间常数（τ）。华为计划到 2031 年利用逻辑折叠技术实现相当于 1.4 纳米制程节点的晶体管密度，该技术将关键门电路拆分为垂直堆叠的有源层，并通过超细间距混合键合完成层间互连。

telegram · zaihuapd · May 30, 02:18

**背景**: 摩尔定律数十年来驱动半导体进步，预测晶体管密度通过几何缩微（缩小晶体管尺寸）约每两年翻一番。然而，随着物理极限逼近，传统缩微日益困难且昂贵。韬缩微定律提出替代方案：不缩小晶体管，而是通过优化整个系统层级的电阻和电容来降低信号传播时间（τ），并可能借助逻辑折叠等 3D 堆叠技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.huawei.com/en/news/2026/5/ieee-iscas-tau-scaling">HUAWEI Presents the Tau (τ) Scaling Law, Enabling Breakthroughs in Transistor Density and System Performance - Huawei</a></li>
<li><a href="https://www.yicaiglobal.com/news/huawei-presents-tau-law-to-replace-geometric-scaling-with-time-scaling-in-semiconductor-industry">Huawei Proposes Tau Scaling Law to Replace Moore’s Law in Chip Industry</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-05-27/what-to-know-about-huawei-s-new-ai-chipmaking-plan-logicfolding-tech">What to Know About Huawei’s New AI Chipmaking Plan... - Bloomberg</a></li>

</ul>
</details>

**标签**: `#semiconductor`, `#Huawei`, `#Moore's Law`, `#chip design`, `#time scaling`

---

<a id="item-3"></a>
## [微软将永久授权 Office 降级为只读模式](https://consumerrights.wiki/w/Microsoft_Office_2019_and_2021_for_Mac_view-only_conversion_(2026)) ⭐️ 8.0/10

微软计划将永久授权的 Office 2019 和 2021 Mac 版转换为只读模式，实质上去除了用户花钱购买的编辑功能。 此举破坏了软件所有权的概念，因为永久授权本应赋予用户无限期使用所购版本的权利。这也推动用户转向 Microsoft 365 订阅，引发了消费者对权利缩水的强烈反弹。 此变更适用于 Office 2019 和 2021 Mac 版永久授权，据报道只读转换计划于 2026 年生效。用户仍可打开和查看文档，但无法编辑、创建或保存更改。

hackernews · antipurist · May 30, 23:26 · [社区讨论](https://news.ycombinator.com/item?id=48341578)

**背景**: Microsoft Office 的永久授权允许用户一次性付费并无限期使用该特定版本，但支持和安全更新可能在几年后终止。这有别于基于订阅的 Microsoft 365，后者需要持续付费才能使用。微软一直在其产品中推行订阅模式，此次对离线永久授权的降级被视为又一步推进。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.compugen.us/blog/microsofts-perpetual-vs.-subscription-licensing-program-explained">Microsoft’s Perpetual vs. Subscription Licensing Program Explained</a></li>
<li><a href="https://www.quora.com/What-is-the-difference-between-an-Office-365-subscription-and-a-perpetual-license-for-Microsoft-Office-products-Are-they-both-subscription-based-but-with-different-terms">What is the difference between an Office 365 subscription and a perpetual license for Microsoft Office products? Are they both subscription-based, but with different terms? - Quora</a></li>

</ul>
</details>

**社区讨论**: 社区评论表达了强烈的愤怒和抵制呼吁，用户 jmward01 敦促人们停止购买微软软件并‘愤怒起来’。其他人指出法律影响，如澳大利亚消费者法，并预测微软会执意推进。一些人建议转向 LibreOffice 作为替代方案。

**标签**: `#Microsoft`, `#software licensing`, `#consumer rights`, `#Office`, `#perpetual license`

---

<a id="item-4"></a>
## [领域专长仍是真正的竞争优势](https://www.brethorsting.com/blog/2026/05/domain-expertise-has-always-been-the-real-moat/) ⭐️ 8.0/10

一篇最近的博文指出，领域专长而非 AI 工具或通用编码技能，才是开发者和企业持久的竞争优势。 这一观点挑战了关于 AI 取代开发者的炒作，并强调了在快速变化的技术格局中深厚行业知识的持久价值。 文章引用了实例，例如领域专家的应用因糟糕的数据库设计而失败，以及一次包船钓鱼之旅揭示了领域知识与软件工程之间的差距。

hackernews · aaronbrethorst · May 30, 20:40 · [社区讨论](https://news.ycombinator.com/item?id=48340411)

**背景**: “领域专长”指对特定行业或领域（如金融、渔业）的深厚知识。“Vibe coding”指在不完全理解代码的情况下使用 AI 助手构建软件的术语。这场辩论的核心在于 AI 工具是否让通用开发者过时，还是领域专长仍然至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vibe_coding">Vibe coding - Wikipedia</a></li>
<li><a href="https://agentsroom.dev/what-is-vibe-coding">What is Vibe Coding ? Definition , Origin, and How It... | AgentsRoom</a></li>

</ul>
</details>

**社区讨论**: 评论普遍赞同领域专长仍然至关重要。用户分享了因缺乏领域知识而项目失败的例子，同时也有评论指出软件工程本身也是一个专业领域。

**标签**: `#domain-expertise`, `#AI`, `#software-engineering`, `#moat`, `#vibe-coding`

---

<a id="item-5"></a>
## [埃森哲以 12 亿美元收购 Ookla 以增强网络智能](https://newsroom.accenture.com/news/2026/accenture-to-acquire-ookla-to-strengthen-network-intelligence-and-experience-with-data-and-ai-for-enterprises) ⭐️ 8.0/10

埃森哲宣布将以 12 亿美元收购 Ookla，Ookla 旗下拥有 Speedtest、Downdetector 等网络测试工具。 此次收购使埃森哲能够利用 Ookla 庞大的网络性能数据和人工智能能力，帮助电信运营商和企业优化网络，可能重塑网络智能服务市场。 Ookla 的数据平台每月处理超过 2.5 亿次消费者发起的测试，辅以受控的驾车和步行测试，提供网络性能的精细洞察。

hackernews · Garbage · May 30, 16:28 · [社区讨论](https://news.ycombinator.com/item?id=48337987)

**背景**: Ookla 最著名的是 Speedtest.net，一个广泛使用的互联网速度测试网站，以及追踪服务中断的 Downdetector。该公司还提供企业级网络测试和分析解决方案。埃森哲是一家全球专业服务公司，一直在扩展其网络智能和人工智能服务。

**社区讨论**: 社区评论指出，此次收购主要是关于数据货币化，因为 Ookla 向电信运营商出售网络性能数据，年费可达六位数。一些用户对产品看似简单却估值如此之高感到惊讶，而前员工则指出公司从数据计划和奖项中获得了可观的收入。

**标签**: `#acquisition`, `#network intelligence`, `#data monetization`, `#telecom`, `#Accenture`

---

<a id="item-6"></a>
## [Voxel Space（2017）——深入解析《科曼奇》地形渲染算法](https://s-macke.github.io/VoxelSpace/) ⭐️ 8.0/10

该文章详细解析了 1992 年游戏《科曼奇：最大杀伤力》中使用的 Voxel Space 地形渲染算法，包含代码示例和历史背景。还收录了社区关于将该算法用于现代项目的趣闻。 该算法在当时具有革命性意义，能在 386SX 这样的低端硬件上实现流畅的 3D 地形渲染。理解它能为游戏开发者、复古计算爱好者以及对高效实时图形技术感兴趣的人提供宝贵见解。 从技术上讲，该算法通过从颜色图中绘制垂直线来渲染高度图，并非使用真正的体积化体素；它更类似于基于棱柱的高度图。整个渲染引擎可以用极少的代码行来实现。

hackernews · davikr · May 30, 14:25 · [社区讨论](https://news.ycombinator.com/item?id=48336564)

**背景**: Voxel Space 是一种地形渲染技术，由 NovaLogic 在 20 世纪 90 年代初的《科曼奇》系列游戏中推广。它利用高度场和颜色纹理，通过水平投射射线并采样高度场来决定屏幕列，从而生成 3D 视图。与真正均匀表示体积的体素引擎不同，Voxel Space 将地形视为 2.5D 表面，从而在当时的 CPU 上实现极快的渲染速度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/s-macke/voxelspace">s-macke/VoxelSpace: Terrain rendering algorithm in less than 20 lines of code - GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Voxel">Voxel - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区评论表达了怀旧之情和技术上的赞赏，有用户将最小测试的概念（“油罐假期”）应用到代码中。另一位评论者澄清该算法并非真正的体素渲染，而是一种高度图技术。还有些人分享了将其移植到现代引擎（如 AGS 和 C++）的成果。

**标签**: `#voxel`, `#terrain rendering`, `#game development`, `#history`, `#algorithm`

---

<a id="item-7"></a>
## [Zig ELF 链接器改进带来更快的迭代](https://ziglang.org/devlog/2026/#2026-05-30) ⭐️ 8.0/10

Zig 团队发布了对其 ELF 链接器的重大改进，实现了快速增量链接，大幅降低了开发过程中的编译时间。该消息在 2026 年 5 月 30 日的 Zig 开发日志中公布。 这些改进有望使 Zig 成为可行的 C 语言替代品，提供与解释型语言相当的迭代速度，同时保持类似 C 或 Rust 的性能。这可能彻底改变系统编程的工作流程，实现更快的开发周期。 新的链接器支持 ELF 目标的增量编译，但增量链接通常与链接时优化（LTO）互斥。因此，此功能主要用于开发构建而非发布构建。

hackernews · kristoff_it · May 30, 17:29 · [社区讨论](https://news.ycombinator.com/item?id=48338673)

**背景**: ELF（可执行与可链接格式）是类 Unix 系统上可执行文件、目标代码和共享库的标准文件格式。增量编译是一种仅重新编译程序中已更改部分的技术，从而加快编辑-编译-测试循环。Zig 是一种系统编程语言，旨在现代、安全且实用，常被定位为 C 语言的潜在替代品。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Executable_and_Linkable_Format">Executable and Linkable Format - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Incremental_compilation">Incremental compilation</a></li>

</ul>
</details>

**社区讨论**: 社区反应非常热烈，像 bpavuk 这样的用户预测 Zig 将成为决定性的 C 语言替代品，实现与 Python 或 JavaScript 相当的迭代速度。Derefr 提出了一个技术问题，认为增量链接可能无法与链接时优化共存，限制了其在开发构建中的使用。总体情绪非常积极，许多人对这一进展表示兴奋。

**标签**: `#Zig`, `#ELF Linker`, `#compiler`, `#systems programming`, `#incremental compilation`

---

<a id="item-8"></a>
## [Openrsync：OpenBSD 安全版 rsync 实现备受关注](https://github.com/kristapsdz/openrsync) ⭐️ 8.0/10

OpenBSD 的 openrsync 是一个采用 BSD 许可、支持 pledge 和 unveil 安全特性的 rsync 重新实现，正在开源社区中获得广泛关注和讨论。 该项目通过限制程序能力和文件系统访问来提升文件同步的安全性，解决了广泛使用的 rsync 工具中的漏洞，并为类 Unix 系统提供了一个可移植的替代方案。 Openrsync 在 GitHub 上可用，可在多种 UNIX 系统上编译，但官方支持 OpenBSD。目前在某些边缘情况下（例如 --rsync-path 选项的行为）尚未完全兼容 rsync。

hackernews · sph · May 30, 10:51 · [社区讨论](https://news.ycombinator.com/item?id=48334854)

**背景**: Rsync 是一个标准的 Unix 工具，用于在本地或网络上高效同步文件。OpenBSD 以其主动的安全方法闻名，引入了 pledge(2) 系统调用来限制进程能力，以及 unveil(2) 来限制文件系统可见性。Openrsync 集成了这些机制以最大限度地减少攻击面。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Openrsync">OpenBSD - Wikipedia</a></li>
<li><a href="https://man.openbsd.org/openrsync.1">openrsync(1) - OpenBSD manual pages</a></li>
<li><a href="https://github.com/kristapsdz/openrsync">GitHub - kristapsdz/openrsync: BSD-licensed implementation of rsync · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenBSD_security_features">OpenBSD security features - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区反馈总体积极，用户报告其稳定性随时间改进。但仍存在一些问题，例如与 --rsync-path 的不同行为，以及关于在 Linux 上支持 pledge 的讨论。此外，用户指出 openrsync 是作为 RPKI 验证器的一部分开发的，并且 Gokrazy 团队也有一个 Go 实现。

**标签**: `#rsync`, `#OpenBSD`, `#security`, `#file-synchronization`, `#open-source`

---

<a id="item-9"></a>
## [OpenRouter 完成 1.13 亿美元 B 轮融资](https://openrouter.ai/announcements/series-b) ⭐️ 8.0/10

OpenRouter 宣布完成 1.13 亿美元的 B 轮融资，凸显其作为关键 LLM API 代理和计费平台的增长。 本轮融资凸显了市场对统一多 LLM 接入和集中计费管理的需求日益增长，这为全球开发者简化了 AI 开发流程。 该公司仍由创始人领导和控制，旨在继续为 AI 开发者构建产品。OpenRouter 对昂贵模型收取少量附加费，但提供低摩擦的模型试验和硬性计费上限。

hackernews · freeCandy · May 30, 17:27 · [社区讨论](https://news.ycombinator.com/item?id=48338660)

**背景**: LLM API 代理充当用户与多个大语言模型提供商之间的中介，提供统一的 API、集中计费和便捷的模型切换。OpenRouter 是该概念的托管版本，使开发者无需为每个提供商管理独立账户和 API 密钥即可访问众多模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/Mirrowel/LLM-API-Key-Proxy">GitHub - Mirrowel/LLM-API-Key-Proxy: Universal LLM Gateway: One API, every LLM. OpenAI/Anthropic-compatible endpoints with multi-provider translation and intelligent load-balancing. · GitHub</a></li>
<li><a href="https://docs.litellm.ai/docs/simple_proxy">LiteLLM AI Gateway (LLM Proxy) | liteLLM</a></li>

</ul>
</details>

**社区讨论**: 社区评论褒贬不一但总体正面：SimonW 最初持怀疑态度，但现在看到了计费上限和易用性的价值；numlocked 强调了创始人控制和长期承诺；minimaxir 称赞模型试验的便利性，但指出了昂贵模型的附加费；其他人质疑名称中的“开放”含义，并对品牌表达困惑。

**标签**: `#LLM`, `#AI Infrastructure`, `#Funding`, `#API Proxy`, `#OpenRouter`

---

<a id="item-10"></a>
## [教皇利奥的首部通谕抨击技术救世主义](https://www.economist.com/europe/2026/05/28/leos-first-encyclical-attacks-technological-messianism) ⭐️ 8.0/10

教皇利奥发布了其首部通谕，明确批评技术救世主义——即认为技术（尤其是人工智能和超人类主义）能拯救人类的信念。该文件针对山姆·奥特曼和达里奥·阿莫迪等技术领袖的言论，他们曾谈及创建宗教或建造神明。 这部通谕标志着一个主要宗教权威的重大文化干预，为关于人工智能、超人类主义以及谁应控制技术的日益激烈的辩论增添了道德和哲学分量。它可能通过将不受约束的技术乐观主义视为一种偶像崇拜来影响公众话语和政策。 该通谕可能认为技术救世主义转移了对人类和精神需求的关注，并呼吁以人为中心的创新方式。它特别驳斥了 AI 可能获得意识或超智能的观点，与那些认为当前大型语言模型只是伪 AI、仍需人类监督的批评者观点一致。

hackernews · 1vuio0pswjnm7 · May 30, 10:30 · [社区讨论](https://news.ycombinator.com/item?id=48334710)

**背景**: 技术救世主义是一种相信技术将带来救赎或乌托邦的信念，常与超人类主义目标相关联——通过人工智能、基因工程和纳米技术增强人类能力。教宗通谕是教皇写给天主教会的权威信函，针对道德和社会问题，在全球数十亿天主教徒中具有重大影响力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.catholicity.com/commentary/shea/02282.html">Mark Shea: Technological Messianism</a></li>
<li><a href="https://www.merriam-webster.com/dictionary/messianism">MESSIANISM Definition & Meaning - Merriam-Webster</a></li>
<li><a href="https://en.wikipedia.org/wiki/Transhumanism">Transhumanism - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者们对通谕的主题进行了深入讨论，有人（如 alecco）认为 AI CEO 表现出“AI 精神病”，且大型语言模型虽强大但并非真正的人工智能。其他人（如 merelydev）将此问题框定为一场关于谁控制技术的权力斗争——技术专家、用户、政府，还是现在的神职人员。讨论还提及了彼得·蒂尔关于敌基督和存在风险的观点。

**标签**: `#religion`, `#artificial intelligence`, `#technology criticism`, `#transhumanism`, `#philosophy`

---

<a id="item-11"></a>
## [Anthropic 详解 Claude 跨产品沙箱技术](https://simonwillison.net/2026/May/30/how-we-contain-claude/#atom-everything) ⭐️ 8.0/10

Anthropic 发布了一份详细的技术概述，介绍了其用于在 Claude.ai、Claude Code 和 Cowork 等产品中隔离 Claude 的沙箱技术。 这解决了沙箱文档普遍缺乏透明度的问题，帮助用户和开发者评估 AI 代理的安全性及其潜在风险。 Claude.ai 使用 gVisor，Claude Code 在 macOS 上使用 Seatbelt、在 Linux 上使用 Bubblewrap，而 Cowork 在 macOS 上通过 Apple 虚拟化框架、在 Windows 上通过 HCS 运行完整虚拟机。

rss · Simon Willison · May 30, 21:36

**背景**: 沙箱是一种安全技术，通过隔离应用程序或进程来限制漏洞利用或异常行为可能造成的损害。gVisor 是 Google 开发的容器沙箱，在用户空间实现 Linux 系统调用；Seatbelt 是 Apple 为 macOS 提供的沙箱内核扩展；Bubblewrap 是一种轻量级的无特权沙箱工具，被 Flatpak 等项目使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GVisor">gVisor - Wikipedia</a></li>
<li><a href="https://theapplewiki.com/wiki/Dev:Seatbelt">Dev:Seatbelt - The Apple Wiki</a></li>
<li><a href="https://wiki.archlinux.org/title/Bubblewrap">Bubblewrap - ArchWiki</a></li>

</ul>
</details>

**标签**: `#AI`, `#security`, `#sandbox`, `#Anthropic`, `#Claude`

---

<a id="item-12"></a>
## [用 Pyodide 和服务工作者在浏览器中运行 Python ASGI 应用](https://simonwillison.net/2026/May/30/pyodide-asgi-browser/#atom-everything) ⭐️ 8.0/10

Simon Willison 展示了一种方法，利用 Pyodide 和服务工作者在浏览器中运行 Python ASGI 应用，使 script 标签中的 JavaScript 能够正确执行，而此前使用 Web Worker 无法做到。 这一进展显著增强了浏览器内 Python 应用（如 Datasette Lite）的能力，使得依赖 JavaScript 的插件和功能得到完全支持。它为在客户端完全运行服务端 Python 框架开辟了新的可能性。 该方法使用服务工作者拦截网络请求，并返回由 Pyodide 中运行的 ASGI 应用生成的响应，确保嵌入的 script 标签被浏览器执行。Simon Willison 通过 Claude Code 使用 Claude Opus 4.8 来开发这一解决方案。

rss · Simon Willison · May 30, 21:02

**背景**: ASGI（异步服务器网关接口）是异步 Python Web 服务器和应用的标准，是 WSGI 的继任者。Pyodide 是 CPython 到 WebAssembly 的移植，使 Python 能在浏览器中运行。服务工作者充当浏览器中的代理服务器，拦截网络请求。此前，使用 Web Worker 在浏览器中运行 Python 时，由于响应以文本方式获取，script 标签中的 JavaScript 无法执行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Asynchronous_Server_Gateway_Interface">Asynchronous Server Gateway Interface - Wikipedia</a></li>
<li><a href="https://github.com/pyodide/pyodide">pyodide / pyodide : Pyodide is a Python distribution for the browser ...</a></li>
<li><a href="https://asgi.readthedocs.io/">ASGI Documentation — ASGI 3.0 documentation</a></li>

</ul>
</details>

**标签**: `#Python`, `#ASGI`, `#WebAssembly`, `#Service Workers`, `#Pyodide`

---

<a id="item-13"></a>
## [SpaceX 获 41.6 亿美元美军卫星导弹追踪合同](https://www.bloomberg.com/news/articles/2026-05-29/spacex-wins-4-billion-contract-for-us-golden-dome-satellites) ⭐️ 8.0/10

SpaceX 获得美国太空军 41.6 亿美元合同，建设一套天基追踪网络，用于识别和跟踪导弹、飞机等空中威胁，这是 Golden Dome 防御计划的一部分。 该合同标志着 SpaceX 在国家安全太空系统中角色的显著扩展，有望减少地面传感器的覆盖盲区，并实现对高超音速导弹等先进威胁的跟踪。它也强化了国防关键基础设施向商业伙伴关系转变的趋势。 该追踪网络将整合天基传感器、通信系统和地面处理能力。SpaceX 此前已参与 Golden Dome 的天基拦截器原型开发，并加入了该计划底层软件系统的多公司联盟。

telegram · zaihuapd · May 30, 01:53

**背景**: Golden Dome 计划是美国于 2025 年宣布的导弹防御计划，旨在保护全国免受导弹袭击。当前的导弹预警卫星针对可预测弹道的传统弹道导弹进行了优化，但难以跟踪以超过 5 马赫速度机动的高超音速导弹。天基传感器旨在填补与地面雷达和飞机相比的探测盲区。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Golden_Dome_(missile_defense_system)">Golden Dome (missile defense system) - Wikipedia</a></li>
<li><a href="https://www.airandspaceforces.com/article/enhanced-space-based-missile-tracking/">Enhanced Space - Based Missile Tracking | Air & Space Forces...</a></li>
<li><a href="https://arstechnica.com/space/2025/07/pentagon-may-put-spacex-at-the-center-of-a-sensor-to-shooter-targeting-network/">Pentagon may put SpaceX at the center of... - Ars Technica</a></li>

</ul>
</details>

**标签**: `#SpaceX`, `#defense`, `#space technology`, `#satellite`, `#military`

---

<a id="item-14"></a>
## [新型 FROST 攻击利用 SSD 计时窥探浏览器活动](https://futurism.com/future-society/websites-spying-solid-state-drive) ⭐️ 8.0/10

研究人员披露了一种名为 FROST 的无交互攻击，利用浏览器的源私有文件系统（OPFS）和 SSD 读写时序来推测用户同时访问的网站或应用。 FROST 实现了高准确率（网站 88.95%，应用 95.83%），且无需安装软件或用户交互，这通过标准 Web API 揭示了新的侧信道向量，引发了严重的隐私担忧。 该攻击仅在 macOS 和 Linux 上测试，但研究人员称 Windows 并非免疫；不使用网页时及时关闭标签页可降低风险。FROST 通过测量 OPFS 操作的时序来创建并发活动的指纹。

telegram · zaihuapd · May 31, 01:55

**背景**: 源私有文件系统（OPFS）是浏览器 API，为每个源提供沙箱化文件系统，专为快速 I/O 操作设计。侧信道攻击通过测量时序变化等间接效应推断敏感信息。FROST 利用 SSD 读写速度随并发活动变化这一特性，使恶意网站能够监控其他标签页或应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tomshardware.com/tech-industry/cyber-security/researchers-say-they-can-spy-on-your-browsing-by-measuring-ssd-activity-through-a-browser-api">Researchers say they can spy on your browsing by measuring SSD activity through a browser API - Tom's Hardware</a></li>
<li><a href="https://arstechnica.com/security/2026/05/websites-have-a-new-way-to-spy-on-visitors-analyzing-their-ssd-activity/">Websites have a new way to spy on visitors: Analyzing their SSD activity - Ars Technica</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/File_System_API/Origin_private_file_system">Origin private file system - Web APIs | MDN</a></li>

</ul>
</details>

**标签**: `#security`, `#side-channel`, `#SSD`, `#browser privacy`, `#FROST`

---