---
layout: default
title: "Horizon Summary: 2026-05-29 (ZH)"
date: 2026-05-29
lang: zh
---

> From 35 items, 8 important content pieces were selected

---

1. [美司法部要求 Reddit 和 X 提供 ICE 批评者数据](#item-1) ⭐️ 9.0/10
2. [GitHub 因零日 Windows 漏洞封禁安全研究员](#item-2) ⭐️ 8.0/10
3. [DBOS 博文称 Postgres 即可支撑持久化工作流](#item-3) ⭐️ 8.0/10
4. [在线发布的 LLM 生成文本‘气味’清单](#item-4) ⭐️ 8.0/10
5. [Anthropic 完成 650 亿美元 H 轮融资，估值 9650 亿美元](#item-5) ⭐️ 8.0/10
6. [高通与字节跳动合作定制 AI ASIC 芯片](#item-6) ⭐️ 8.0/10
7. [黄仁勋：台湾是 AI 革命中心，年投 1500 亿美元](#item-7) ⭐️ 8.0/10
8. [比亚迪量产 4nm 智驾芯片璇玑 A3](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [美司法部要求 Reddit 和 X 提供 ICE 批评者数据](https://www.bloomberg.com/news/articles/2026-05-28/trump-s-doj-ramps-up-probes-of-anonymous-ice-critics-with-x-reddit-subpoenas) ⭐️ 9.0/10

美国司法部向 Reddit 和 X 发出大陪审团传票，要求提供至少两个匿名账户的真实姓名、住址和银行信息，这些账户曾批评 ICE 的执法行动。受影响用户已聘请律师，在法庭上挑战这些传票。 从行政传票升级到大陪审团传票，标志着政府对网络批评者的调查力度加大，可能压制受第一修正案保护的言论。这引发了对用户隐私、言论自由以及数字平台上政府监控范围的严重担忧。 这些传票基于一项正在进行的刑事调查，但用户尚未被告知涉嫌的具体罪名。法官目前正在审理撤销传票的请求。

telegram · zaihuapd · May 28, 14:22

**背景**: 美国司法部有权调查联邦犯罪，并可通过传票强制平台披露用户数据。大陪审团传票比行政传票更具强制性，通常意味着刑事调查。虽然科技公司经常收到政府数据请求，但针对政治批评者的匿名账户采取如此升级的措施相对罕见，且在法律上存在争议。

**标签**: `#free speech`, `#government surveillance`, `#privacy`, `#digital rights`, `#US law`

---

<a id="item-2"></a>
## [GitHub 因零日 Windows 漏洞封禁安全研究员](https://www.tomshardware.com/tech-industry/cyber-security/microsofts-github-bans-security-researcher-who-posted-zero-day-windows-exploits-because-company-ruined-their-life-expert-claims-action-is-vindictive-and-promises-further-retaliation) ⭐️ 8.0/10

GitHub 封禁了一名安全研究员，因其发布了零日 Windows 漏洞利用代码，该研究员声称微软毁了自己的生活并誓言进一步报复。 这一事件凸显了漏洞赏金计划、平台政策与研究员伦理之间的紧张关系，可能会影响零日漏洞披露的处理方式以及研究员与大型科技公司之间的信任。 该研究员还被 GitLab 封禁，社区推测可能违反了关于托管漏洞利用代码的规则，但微软尚未公开发表评论。

hackernews · possibilistic · May 28, 21:45 · [社区讨论](https://news.ycombinator.com/item?id=48315968)

**背景**: 零日漏洞是指软件供应商未知的安全缺陷，可能在补丁发布之前被利用。漏洞赏金计划鼓励道德黑客私下报告此类缺陷以换取奖励，但公开发布利用代码可能导致封禁和法律问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zero-day_vulnerability">Zero-day vulnerability - Wikipedia</a></li>
<li><a href="https://bugbustersunited.com/bug-bounty-ethics-101-legal-and-ethical/">Bug Bounty Ethics 101: Legal and Ethical Best Practices | BugBustersUnited</a></li>

</ul>
</details>

**社区讨论**: 评论者担心微软的行为可能具有报复性且适得其反，迫使研究员将漏洞出售给他人。有人质疑为何 GitHub 和 GitLab 都封禁了该用户，暗示可能违反了规则。其他人指出，漏洞赏金计划通常激励发放奖励，因此这是一个不寻常的案例。

**标签**: `#security`, `#zero-day`, `#GitHub`, `#Microsoft`, `#bug bounty`

---

<a id="item-3"></a>
## [DBOS 博文称 Postgres 即可支撑持久化工作流](https://www.dbos.dev/blog/postgres-is-all-you-need-for-durable-execution) ⭐️ 8.0/10

DBOS 的一篇博文指出，仅凭 PostgreSQL 就足以构建持久化工作流执行系统，挑战了使用 Temporal 或 Restate 等外部工作流引擎的必要性。 这一讨论之所以重要，是因为它凸显了利用数据库自身实现可靠性的趋势，从而为构建分布式系统的开发者降低基础设施复杂性和运维开销。 该博文特别引用了 DBOS（一个基于 Postgres 原生的持久化执行框架），并与其他替代方案进行了比较。Postgres 的 advisory locks 和 LISTEN/NOTIFY 等关键特性使得无需外部依赖即可协调工作流。

hackernews · KraftyOne · May 28, 18:41 · [社区讨论](https://news.ycombinator.com/item?id=48313530)

**背景**: 持久化工作流通过持久化状态和重试机制，确保一系列步骤（如订单处理）即使在发生故障时也能可靠完成。传统上，这需要专用引擎如 Temporal。Postgres 提供了内置原语，如用于并发控制的 advisory locks 和用于实时通知的 LISTEN/NOTIFY，可以将这些组合起来直接在数据库中构建工作流编排。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.dbos.dev/blog/postgres-is-all-you-need-for-durable-execution">Postgres-backed Durable Workflow Execution | DBOS</a></li>
<li><a href="https://appmaster.io/blog/postgresql-advisory-locks-double-processing">PostgreSQL advisory locks for concurrency-safe workflows</a></li>
<li><a href="https://medium.com/@kaushalsinh73/10-reactive-postgres-tricks-with-listen-notify-00543968b566">10 Reactive Postgres Tricks With LISTEN / NOTIFY | Medium</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了实际经验：一些人使用 DBOS 处理需要与 Postgres 事务绑定的原子消息传递的工作流，而另一些人则因性能选择 Restate，或因成本选择 Cloudflare Workflows。用户还将 DBOS 与 Temporal 比较，指出 Temporal 存在负载大小限制，并称赞基于 Postgres 的方法更简单。

**标签**: `#postgres`, `#durable-workflows`, `#distributed-systems`, `#workflow-engines`

---

<a id="item-4"></a>
## [在线发布的 LLM 生成文本‘气味’清单](https://shvbsle.in/various-llm-smells/) ⭐️ 8.0/10

一篇题为《各种 LLM 气味》的博客文章整理了一份精心挑选的语言和风格模式清单，这些模式强烈表明文本由 AI 生成，引发了社区关于检测和使用的讨论。 随着 LLM 变得无处不在，能够检测 AI 生成的写作对于维护内容、教育和新闻的真实性至关重要，而这份清单为读者和作者提供了实用、可操作的标记。 该清单包括特定的短语，如“the honest caveat:”和隐喻性使用的“load bearing”，以及对比否定（“不是 X，而是 Y”）等结构模式，这些在 LLM 输出中常见，但在人类写作中并不典型。

hackernews · speckx · May 28, 19:02 · [社区讨论](https://news.ycombinator.com/item?id=48313810)

**背景**: 像 GPT-4 这样的大型语言模型（LLM）通过基于大量训练数据预测下一个词来生成文本。它们的输出常常表现出微妙的风格习惯，即“气味”，细心的读者可以识别出来。这种现象类似于维基百科的“AI 写作迹象”页面，该页面记录了类似的模式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Large_language_model">Large language model - Wikipedia</a></li>
<li><a href="https://blog.frohrer.com/how-to-detect-llm-writing-in-text/">Detecting LLM writing in Text | Fred Rohrer's Blog</a></li>

</ul>
</details>

**社区讨论**: 评论指出，对于缺乏领域专业知识的人来说，LLM 写作可能显得“明显更好”，并警告不要直接融入 AI 生成的短语。一些用户指出，像对比否定这样的结构模式是强烈的提示。其他人建议使用 LLM 进行编辑而不是生成，以保持个人风格。

**标签**: `#LLM`, `#AI detection`, `#writing`, `#analysis`, `#Hacker News`

---

<a id="item-5"></a>
## [Anthropic 完成 650 亿美元 H 轮融资，估值 9650 亿美元](https://www.anthropic.com/news/series-h) ⭐️ 8.0/10

Anthropic 宣布获得 650 亿美元的 H 轮融资，投后估值达到 9650 亿美元。该公司还报告称，其年化 run-rate revenue 在本月初超过了 470 亿美元。 这一巨额融资轮突显了领先 AI 公司对资本的巨大需求以及市场的期望。相对于所报告营收的高估值引发了对其可持续性和未来 IPO 前景的质疑。 470 亿美元的 run-rate revenue 数据是自行报告的，代表基于近期月度表现的年化营收，并非 GAAP 营收。这笔融资距离 2026 年 2 月的 G 轮融资仅过去了几个月。

hackernews · meetpateltech · May 28, 18:09 · [社区讨论](https://news.ycombinator.com/item?id=48313048)

**背景**: Run-rate revenue 通过将近期（例如一个月）的营收外推至全年来估算年度营收；快速成长的初创公司常用此指标，但如果增长不是线性的，则可能产生误导。风险投资融资轮按字母顺序分类（A 轮、B 轮、C 轮等），像 H 轮这样的后期轮次表明公司在考虑 IPO 之前已经进行了多轮融资。

**社区讨论**: 社区评论对估值表示怀疑，有人质疑还需要多少轮融资投资者才能获得回报。其他人则讨论了 run-rate revenue 与实际营收的含义和可靠性，并指出如果没有 IPO，公司对其财务声明的审查较少。

**标签**: `#Anthropic`, `#funding`, `#AI`, `#valuation`, `#venture capital`

---

<a id="item-6"></a>
## [高通与字节跳动合作定制 AI ASIC 芯片](https://t.me/zaihuapd/41616) ⭐️ 8.0/10

据报道，高通已与字节跳动达成协议，为字节跳动生产定制 AI ASIC 芯片，字节跳动将采购数百万颗芯片用于其 AI 工作负载。 这一合作可能对 AI 硬件格局产生重大影响，结合了高通的芯片设计专长与字节跳动庞大的 AI 服务需求。这反映了超大规模云服务商寻求定制芯片以优化性能和成本的趋势。 双方均未确认该交易，高通代表拒绝置评，字节跳动发言人未回应。高通曾在 4 月底宣布，将于今年向某超大规模云服务商交付首款 ASIC，这与该报道一致。

telegram · zaihuapd · May 28, 07:09

**背景**: ASIC（专用集成电路）是为特定任务定制的芯片，与通用 CPU 或 GPU 相比，提供更优越的性能和能效。在 AI 领域，ASIC 可以更高效地加速模型推理和训练。主要科技公司越来越多地设计定制 ASIC，以降低成本并提高其特定工作负载的性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Application-specific_integrated_circuit">Application-specific integrated circuit - Wikipedia</a></li>
<li><a href="https://www.arm.com/glossary/asic">What is ASIC? - ASIC Cost</a></li>

</ul>
</details>

**标签**: `#Qualcomm`, `#ByteDance`, `#AI`, `#ASIC`, `#hardware`

---

<a id="item-7"></a>
## [黄仁勋：台湾是 AI 革命中心，年投 1500 亿美元](https://arstechnica.com/tech-policy/2026/05/nvidia-ceo-wants-taiwan-to-be-center-of-ai-revolution-not-us/) ⭐️ 8.0/10

英伟达 CEO 黄仁勋宣称台湾是 AI 革命中心，并宣布计划每年在台湾投入约 1500 亿美元，用于 AI 芯片生产、系统制造和供应链合作。一座新的台北总部预计今年动工，2030 年启用，容纳 4000 名员工。 这一巨额投资大幅加深了英伟达对台湾供应链的依赖，强化了台湾在 AI 硬件生产中的战略地位。在中美持续紧张的背景下，这也具有地缘政治意义，凸显了台湾对全球 AI 产业的核心作用。 每年 1500 亿美元的投资较几年前每年 100-150 亿美元大幅增长。新台北总部将容纳 4000 名员工，预计 2030 年启用。

telegram · zaihuapd · May 28, 07:33

**背景**: 台湾拥有全球领先的半导体代工厂台积电（TSMC），以及鸿海（富士康）、纬创、广达等密集的电子制造生态系统。英伟达最先进的 AI 芯片依赖台积电生产，系统组装则依靠台湾的原始设计制造商（ODM）。黄仁勋的声明强化了台湾作为全球 AI 供应链关键节点的地位。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Wistron_Corporation">Wistron Corporation</a></li>
<li><a href="https://en.wikipedia.org/wiki/Quanta_Computer">Quanta Computer</a></li>
<li><a href="https://en.wikipedia.org/wiki/Semiconductor_industry_in_Taiwan">Semiconductor industry in Taiwan - Wikipedia</a></li>

</ul>
</details>

**标签**: `#NVIDIA`, `#AI`, `#Supply Chain`, `#Taiwan`, `#Investment`

---

<a id="item-8"></a>
## [比亚迪量产 4nm 智驾芯片璇玑 A3](https://finance.sina.com.cn/roll/2026-05-28/doc-inhznenn1371824.shtml) ⭐️ 8.0/10

2026 年 5 月 28 日，在'敢为'智能化战略发布会上，比亚迪总裁王传福宣布 4 纳米智驾芯片'璇玑 A3'已开启规模化量产。该芯片支持 L3、L4 级自动驾驶，三颗芯片总算力超过 2100 TOPS。 这一里程碑展示了比亚迪在自动驾驶硬件上的深度垂直整合，可能减少对外部供应商的依赖，并加速高级自动驾驶在大众市场电动车中的普及。4 纳米制程节点与领先芯片制造商相当，标志着中国在汽车半导体领域能力的提升。 该芯片结合比亚迪自研算法，算力利用率提升 100%。比亚迪还透露已推出 2000 多款芯片产品，并拥有 5 座晶圆工厂。

telegram · zaihuapd · May 28, 13:01

**背景**: 自动驾驶分为 0 到 5 级，L3 为有条件自动化，驾驶员可移开视线但需准备接管；L4 为高度自动化，车辆在特定条件下可完全自主驾驶。TOPS（每秒万亿次运算）是 AI 芯片性能的关键指标；2100 TOPS 足以支持自动驾驶所需的复杂实时感知与决策。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://torc.ai/understanding-the-levels-of-autonomy-3-4-5/">What Are The Levels of Autonomy? L3-L4 - Torc Robotics</a></li>
<li><a href="https://www.windowscentral.com/hardware/laptops/what-is-tops">What is TOPS and why is it important for AI? | Windows Central</a></li>

</ul>
</details>

**标签**: `#BYD`, `#autonomous driving`, `#4nm chip`, `#EV`, `#semiconductor`

---