---
layout: default
title: "Horizon Summary: 2026-08-29 (ZH)"
date: 2026-08-29
lang: zh
---

> From 33 items, 13 important content pieces were selected

---

1. [Triton v3.8.0 发布：新增 Aggregate API 与 TopK 选项](#item-1) ⭐️ 9.0/10
2. [OpenAI 在 SpaceX 收购 Cursor 后限制其使用其模型](#item-2) ⭐️ 9.0/10
3. [美国对意大利托管集体 A/I 实施制裁，并将 noblogs.org 列为恐怖实体](#item-3) ⭐️ 9.0/10
4. [GLM-5.3 开放权重发布，成为强大的开源替代方案](#item-4) ⭐️ 9.0/10
5. [新 CLI 工具借助苹果 Virtualization.framework 启动虚拟 iPhone](#item-5) ⭐️ 8.0/10
6. [博文主张 GUI 应完全由键盘驱动](#item-6) ⭐️ 8.0/10
7. [Htmx 4.0 已发布，带来新特性与兼容性改进](#item-7) ⭐️ 8.0/10
8. [仅凭漏洞传言即可催生漏洞利用，分析师如是说](#item-8) ⭐️ 8.0/10
9. [OpenAI Python SDK 迁移至 HTTPX2 以避免破坏性变更](#item-9) ⭐️ 8.0/10
10. [新攻击破解 Claude Code 自动模式，成功率 80%](#item-10) ⭐️ 8.0/10
11. [OpenAI 被曝开发常驻 Codex 代理，持续工作直至休眠](#item-11) ⭐️ 8.0/10
12. [腾讯开源 Hy4 preview：770B 参数 MoE 模型](#item-12) ⭐️ 8.0/10
13. [Z.ai 发布 GLM-5.3-Flash：320B 总参数、18B 激活，价格降至十分之一](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Triton v3.8.0 发布：新增 Aggregate API 与 TopK 选项](https://github.com/triton-lang/triton/releases/tag/v3.8.0) ⭐️ 9.0/10

Triton v3.8.0 已在 triton-lang GitHub 仓库发布，将 @triton.aggregate 和 @gluon.aggregate 作为公开 API，并为 tl.topk 新增了 descending 参数。该版本还包含大量编译器、NVIDIA/AMD 后端以及 multi-CTA/TMA 的改进。 Triton 是 AI/ML 领域广泛使用的 GPU 编程语言和编译器，因此该版本的改进将惠及面向 NVIDIA 和 AMD 硬件的内核开发者。公开的 aggregate API 和扩展的 topk 支持让编写复杂、可读性强的 JIT 内核更加容易。 值得注意的技术细节包括：JIT 缓存键现在可确定性生成、解释器支持 tl.dot_scaled、tl.fdiv 支持 IEEE 舍入、修复了 argmin/argmax/minimum/maximum/clamp 对 NaN 的处理。multi-CTA 支持扩展到了布局转换、归约和 TMA gather/scatter，tma.store_wait 也新增了 read_only 参数。

github · warrendeng · Aug 28, 18:25

**背景**: Triton 是一种用于编写高性能 GPU 内核的领域特定语言和编译器，与深度学习框架关系密切。新增的 aggregate 类型允许开发者定义传递给内核的结构化数据，类似于 dataclass。tl.topk 是一种常见的操作，用于沿张量维度查找 k 个最大或最小元素；新的 descending 参数可让用户设置它为 False 来获取最小值。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://triton-lang.org/main/python-api/generated/triton.language.topk.html">triton.language.topk — Triton documentation</a></li>
<li><a href="https://triton-lang.org/main/dialects/GluonDialect.html">‘gluon’ Dialect — Triton documentation</a></li>
<li><a href="https://github.com/triton-lang/triton/issues/8781">[Frontend] OOP + aggregate in triton/gluon #8781 - GitHub</a></li>

</ul>
</details>

**标签**: `#triton`, `#GPU`, `#compiler`, `#release`, `#deep learning`

---

<a id="item-2"></a>
## [OpenAI 在 SpaceX 收购 Cursor 后限制其使用其模型](https://openai.com/index/our-decision-on-cursor-following-its-acquisition-by-spacex/) ⭐️ 9.0/10

OpenAI 决定在 SpaceX 收购 AI 代码编辑器 Cursor 后，限制 Cursor 使用其模型。此举与 Anthropic 早前的禁令如出一辙，并使 Cursor 的 API 转售商业模式面临重大压力。 此举标志着前沿 AI 模型提供商在分销渠道和服务条款执行方面的竞争不断升级。依赖 Cursor 在 OpenAI、Anthropic 等模型之间切换的开发者，可能会失去对其首选模型的访问权限，或面临更高成本。 OpenAI 的这项限制措施是在 Anthropic 基于服务条款封禁 xAI 之后出台的，此前 Musk 承认蒸馏了竞争对手的模型。Cursor 允许用户在同一个编辑器中使用多家提供商的模型，这一限制可能会动摇其多模型工作流和订阅价值。

hackernews · meetpateltech · Aug 29, 01:47 · [社区讨论](https://news.ycombinator.com/item?id=49486172)

**背景**: Cursor 是总部位于旧金山的 Anysphere 公司（成立于 2022 年）开发的 AI 原生代码编辑器和编程代理。其业务部分依赖 API 转售：Cursor 从 OpenAI、Anthropic 等提供商购买模型访问权限，再打包进订阅服务，让开发者能在编辑器内切换不同模型。此前 Anthropic 曾以类似理由封禁 xAI，因此 OpenAI 的决定延续了模型提供商管控自家模型使用范围的先例。SpaceX 收购 Cursor 使后者进入 Elon Musk 的企业版图，与 OpenAI 形成直接竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cursor_(company)">Cursor (company) - Wikipedia</a></li>
<li><a href="https://builtin.com/articles/what-is-cursor-ai">What Is Cursor? AI Code Editor Explained | Built In</a></li>
<li><a href="https://cloudinsight.cc/en/blog/ai-api-reseller-guide">How to Choose an AI API Reseller ? 2026 Taiwan Enterprise...</a></li>

</ul>
</details>

**社区讨论**: 评论者大多认为 OpenAI 此举是意料之中的商业博弈，并指出 Anthropic 早已封禁过 xAI。一些 Cursor 用户感到失望，表示多模型切换是其工作流的核心，有人表示会转向仅使用 Anthropic 模型的订阅；另一些人则认为 Cursor 的 API 转售模式本就脆弱，模型提供商的补贴套餐最终会使其失去竞争力。

**标签**: `#AI`, `#OpenAI`, `#Cursor`, `#Acquisition`, `#Developer Tools`

---

<a id="item-3"></a>
## [美国对意大利托管集体 A/I 实施制裁，并将 noblogs.org 列为恐怖实体](https://www.inventati.org/) ⭐️ 9.0/10

2026 年 8 月底，美国国务院将意大利隐私与托管集体 Autistici/Inventati（A/I 集体）列为“特别指定全球恐怖分子”。该指定也涵盖该集体旗下的博客平台 noblogs.org。 这是美国首次将互联网基础设施提供商指定为全球恐怖组织，此举可能将隐私和通信工具的运营定为犯罪。它可能在全球范围内对言论自由和加密项目产生寒蝉效应，因为任何托管服务都可能面临类似制裁。 美国国务院将 A/I 描述为“位于意大利的极端组织”，为“暴力 Antifa 组织和其他极左激进分子”建立数字基础设施。该指定是根据第 13224 号行政令作出的，冻结该集体在美国的任何资产，并禁止美国人与之进行交易，但对一个非营利托管集体的实际执行方式尚不明确。

hackernews · exiguus · Aug 28, 12:58 · [社区讨论](https://news.ycombinator.com/item?id=49477854)

**背景**: Autistici/Inventati 由意大利活动人士于 2001 年创立，旨在为社会运动提供免费通信、隐私和托管工具。Noblogs.org 是该集体运营的免费博客平台，被包括无政府主义者和 Antifa 支持者在内的各种群体使用，也有普通用户。美国的行动标志着反恐制裁前所未有地扩展到互联网基础设施，这让数字权利倡导者对基本在线隐私工具的未来感到担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.state.gov/releases/office-of-the-spokesperson/2026/08/designation-of-autistici-inventati-as-a-specially-designated-global-terrorist/">Designation of Autistici/Inventati as a Specially Designated ...</a></li>
<li><a href="https://www.autistici.org/who/collective">A short history of the A/I Collective - autistici.org</a></li>
<li><a href="https://noblogs.org/">noblogs . org</a></li>

</ul>
</details>

**社区讨论**: 新闻评论区大多持批评态度，许多用户称这一指定是对基础设施提供商的“前所未有”的攻击。一条高赞评论警告说，如果基础设施提供商可以被标记为恐怖分子，那么 I2P、Monero、Signal 和 Tox 等项目可能成为下一个目标；其他用户则分享了 A/I 激进主义历史背景，并指出国务院声明中的不实之处。

**标签**: `#sanctions`, `#privacy`, `#internet freedom`, `#infrastructure`, `#surveillance`

---

<a id="item-4"></a>
## [GLM-5.3 开放权重发布，成为强大的开源替代方案](https://huggingface.co/zai-org/GLM-5.3) ⭐️ 9.0/10

智谱（Z.ai）已将 GLM-5.3 作为开放权重模型发布，它在与 GLM-5.2 相同的基础模型上进行了大幅扩展的后训练，从而提升了编码和智能体能力。该模型也以 GLM-5.3-Flash 的形式在智谱平台上提供。 此次发布提供了一个极具竞争力的开放权重模型，作为专有模型之外的替代选择，因其能力和 token 使用效率而受到好评。它加剧了开放权重大语言模型领域的竞争，尤其凸显了中国 AI 实验室的快速进步。 GLM-5.3 使用与 GLM-5.2 相同的基础模型，所有改进均来自后训练而非预训练。据称它具有良好的 token 与准确率之比，输出 token 涵盖推理和工具调用，并且比 Kimi 等一些竞争模型更容易运行。

hackernews · jeudesprits · Aug 28, 15:20 · [社区讨论](https://news.ycombinator.com/item?id=49479878)

**背景**: 开放权重模型是指其训练参数公开释出的人工智能模型，任何人都可以下载、运行和修改它们。GLM 是由中国人工智能公司智谱（Z.ai，原智谱 AI）开发的一系列大语言模型。后训练是指在初始预训练阶段之后进行的额外训练，目的是让模型与预期行为对齐并提升特定能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://z.ai/blog/glm-5.3">GLM-5.3: Frontier Coding with Emergent Cyber Capabilities</a></li>
<li><a href="https://docs.z.ai/guides/llm/glm-5.3">GLM-5.3 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>
<li><a href="https://www.interconnects.ai/p/glm-53-how-chinese-labs-keep-stride">GLM-5.3: How Chinese labs keep stride with the frontier</a></li>

</ul>
</details>

**社区讨论**: 社区反应总体正面，用户称赞 GLM-5.3“很棒”，并指出它能以 DeepSeek Flash 所缺乏的直觉处理难题。有人将其比作 Opus 4.8，也有人指出它在能力上略逊于 Kimi，但更容易运行，而且第三方提供商的价格可能更低。

**标签**: `#AI`, `#LLM`, `#open-weights`, `#GLM`, `#machine-learning`

---

<a id="item-5"></a>
## [新 CLI 工具借助苹果 Virtualization.framework 启动虚拟 iPhone](https://github.com/Lakr233/vphone-cli) ⭐️ 8.0/10

一款名为 vphone-cli 的新型开源 CLI 工具可以利用苹果官方的 Virtualization.framework 启动虚拟 iPhone。它首次在 Apple 硬件上提供了一条本地的、命令行驱动的全 iOS 虚拟化路径。 这一进展意义重大，因为它为 iOS 测试和 CI 流水线提供了一种基于苹果官方 API 的替代方案，可替代实体 iPhone，从而降低成本并改进自动化。它也对 Corellium 等第三方解决方案构成挑战，并用完整的操作系统虚拟化补充了 iOS 模拟器。 该工具利用苹果官方为 macOS 和 Linux 虚拟机设计的 Virtualization.framework，并将其改用于启动 iOS。有评论指出，在 iOS 设置过程中，选择日本或欧盟作为地区会引入虚拟机无法满足的监管检查；该工具还依赖 macOS 主机，这限制了其可扩展性。

hackernews · hentrep · Aug 28, 23:02 · [社区讨论](https://news.ycombinator.com/item?id=49485267)

**背景**: Apple 的 Virtualization.framework 提供了在 Apple silicon 和基于 Intel 的 Mac 上创建和管理虚拟机的高级 API，通常用于 macOS 或 Linux 客户机。虚拟化 iOS 并非官方支持的用例，但开发者一直在尝试将此框架改造为运行 iOS，逆向工程社区和技术博客对此有所记载。相比之下，iOS 模拟器只是模拟 iOS 应用，而非启动完整的操作系统，因此真正的虚拟 iPhone 填补了不同的空白。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.apple.com/documentation/virtualization">Virtualization | Apple Developer Documentation</a></li>
<li><a href="https://www.reddit.com/r/ReverseEngineering/comments/1chcob6/virtualizing_ios_on_apple_silicon/">r/ReverseEngineering on Reddit: Virtualizing iOS on Apple Silicon</a></li>
<li><a href="https://nickb.website/blog/virtualizing-ios-on-apple-silicon">Virtualizing iOS on Apple Silicon | Nick Botticelli</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论显得谨慎而积极，但充满了实际问题：用户询问它能否在 localhost 上测试手机浏览器、它与 iOS 模拟器有何区别，以及它是否包含虚拟基带。一些人称这是 CI 流水线的重大胜利，而另一些人则指出，对 macOS 主机的依赖仍然限制了其扩展性。

**标签**: `#iOS`, `#virtualization`, `#developer-tools`, `#Apple`, `#CI`

---

<a id="item-6"></a>
## [博文主张 GUI 应完全由键盘驱动](https://ckardaris.com/blog/2026/08/28/keyboard-driven-guis.html) ⭐️ 8.0/10

软件工程师 ckardaris 发表博客文章，主张图形用户界面（GUI）应完全由键盘驱动，该文在 Hacker News 上引发热议，获得 712 分和 343 条评论。 这场讨论触及软件设计中的根本矛盾：残疾用户的无障碍访问、高级用户的操作效率，以及 UI 框架开箱即用地支持键盘导航的责任。它揭示了一个常被忽视、却影响数百万用户的 UX 层面。 原帖是一篇个人博客文章而非正式提案，摘要中未包含具体技术建议。评论者指出，Cocoa/AppKit 等较老框架让键盘无障碍相对容易实现，而现代 Web 框架往往默认不提供该能力。

hackernews · ckardaris · Aug 28, 15:17 · [社区讨论](https://news.ycombinator.com/item?id=49479837)

**背景**: 键盘驱动的 GUI 是指无需鼠标即可完成所有操作的界面，通常通过 Tab 导航、快捷键和焦点管理实现。键盘无障碍是行动或视力障碍用户的核心需求，也惠及不喜欢在键盘和鼠标间切换的高级用户。许多桌面 UI 框架提供内置支持，但 Web 应用常常忽视这一点，部分原因是开发者依赖的浏览器默认行为并不完整。

**社区讨论**: 评论者普遍认同键盘无障碍的重要性，但在实现方式上存在分歧。一位用户主张 ADA 合规与包容应优先，另一位则反对强迫所有用户学习键盘驱动界面，认为高级用户体验与普通用户体验不是一回事。还有评论者提出‘键盘驱动’的真正含义，认为仅仅分配快捷键只是‘兼容键盘’，而非真正的键盘驱动。

**标签**: `#accessibility`, `#keyboard-driven`, `#GUI`, `#UX`, `#software engineering`

---

<a id="item-7"></a>
## [Htmx 4.0 已发布，带来新特性与兼容性改进](https://four.htmx.org/announcements/2026-08-28-htmx-4.0.0-is-released) ⭐️ 8.0/10

Htmx 4.0 于 2026 年 8 月 28 日发布，为超媒体驱动的 Web 开发带来了新特性和兼容性改进。社区对发布的讨论提到一个新的 `hx-alpine-compat` 扩展，用于解决 htmx 与 Alpine.js 之间的兼容性问题。 作为最广泛使用的超媒体库之一的重要版本，Htmx 4.0 强化了超媒体驱动应用作为复杂 JavaScript 框架替代方案的可行性。对于偏好服务端渲染和最少客户端脚本的开发者来说，这一点尤为重要。 新的 `hx-alpine-compat` 扩展旨在解决 htmx 与 Alpine.js（一种轻量级 JavaScript 库）之间的互操作性问题。该公告在社区平台上获得了 592 分和 145 条评论，显示出强烈的关注度和多样化的观点。

hackernews · rmsaksida · Aug 28, 13:28 · [社区讨论](https://news.ycombinator.com/item?id=49478178)

**背景**: htmx 是一个小巧、无依赖、可扩展的 JavaScript 库，允许开发者直接从 HTML 访问现代浏览器特性，而无需编写 JavaScript。据维基百科介绍，htmx 是作为 intercooler.js 的不依赖 jQuery 的改进版本而创建的，1.0.0 版本于 2020 年 11 月发布。在超媒体驱动开发中，客户端通过选择服务器响应中的链接和表单来转换应用状态，这一方法源于 RESTful 设计中的 HATEOAS 概念。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Htmx">htmx - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/HATEOAS">HATEOAS - Wikipedia</a></li>
<li><a href="https://hypermedia.systems/hypermedia-a-reintroduction/">Hypermedia: A Reintroduction</a></li>

</ul>
</details>

**社区讨论**: 社区讨论总体积极，但也包含一个相反观点。htmx 的首席执行官表示他非常喜欢 htmx，另一位开发者评论说 htmx 带给他快乐，并认为 Hugs 技术栈（Go、htmx、SQLite）让事情保持简单。然而，一位 .NET/Angular 开发者发现 htmx 让事情变得更困难，因为它迫使展示关注点回到后端；另一位评论者指出，alpine-ajax 比 htmx 更小，同时提供了所需功能。

**标签**: `#htmx`, `#web development`, `#hypermedia`, `#javascript`, `#release`

---

<a id="item-8"></a>
## [仅凭漏洞传言即可催生漏洞利用，分析师如是说](https://anil.recoil.org/notes/rumour-is-the-exploit) ⭐️ 8.0/10

该博文指出，仅仅凭借漏洞传言就足以让攻击者找到可用的漏洞利用，而 LLM 的规模化与普及化进一步加速了这一趋势。现实佐证是 rclone 在最近一个月收到超过 40 份安全披露，而项目前十年总共才收到约 20 份。 这改变了安全格局：攻击者不再需要内部细节即可开始寻找漏洞，开源维护者因此面临大量低质量但耗时耗力的报告。同时也显示出 AI 正在改变漏洞发现与响应方式，兼具攻防两方面的深远影响。 rclone 维护者称近期安全披露的命中率约为 75%，即很多报告确实包含值得关注的问题。另一位评论者指出，LLM 驱动的漏洞挖掘在概念上并非全新，但已大规模地将漏洞利用普及到低价值目标，也有人已开始用 AI 监控提交记录以识别隐藏的 bug 修复。

hackernews · avsm · Aug 28, 15:58 · [社区讨论](https://news.ycombinator.com/item?id=49480466)

**背景**: 传统上，漏洞研究人员通过分析补丁、提交信息和偶然言论来寻找利用方式。如今 LLM 降低了门槛，任何人都能通过模糊的提示或传言生成具体的漏洞利用 PoC。这使得漏洞利用更快、更广，开源维护者需要处理激增的报告，压力倍增。同时，AI 也能帮助防御方进行分诊和修复，但组织意愿仍是瓶颈。

**社区讨论**: 维护者普遍表示不堪重负，rclone 的 nickcw 称即使借助 AI 分诊也耗费大量时间。部分评论者认为核心问题不是 AI 能力，而是组织缺乏修复漏洞的意愿；也有人指出 LLM 只是把老做法扩大到了大规模、低价值目标的利用。此外，还有评论担忧部署延迟和供应链风险使得快速修复并不现实。

**标签**: `#security`, `#AI`, `#vulnerabilities`, `#open source`, `#LLM`

---

<a id="item-9"></a>
## [OpenAI Python SDK 迁移至 HTTPX2 以避免破坏性变更](https://github.com/openai/openai-python/blob/main/httpx2.md) ⭐️ 8.0/10

OpenAI 的 Python SDK 正在迁移到 HTTPX2，这是 httpx 库的一个分支，它保留现有 API，而不是跟随 httpx 计划中的 1.0 破坏性变更。Anthropic 随后也在其 Python SDK 中做了同样的切换。 这很重要，因为 OpenAI 和 Anthropic 是使用最广泛的 Python SDK 之一，它们的依赖选择会影响成千上万的开发者。选择稳定的分支而不是不断变化的目标，有助于保护下游项目免受 httpx 1.0 意外破坏性变更的影响。 根据社区讨论，HTTPX2 本质上是 httpx 的一个分支，承诺不破坏现有 API，从而成为更稳定的依赖。一个值得注意的行为变化是，SDK 现在使用操作系统的 TLS 信任库，而不是 certifi。

hackernews · tosh · Aug 28, 11:51 · [社区讨论](https://news.ycombinator.com/item?id=49477212)

**背景**: httpx 是一个流行的 Python 下一代 HTTP 客户端，提供同步和异步 API，并支持 HTTP/1.1 和 HTTP/2。包括 OpenAI 在内的许多 SDK 都依赖 httpx 发起 API 请求。由于 httpx 正迈向带有破坏性变更的 1.0 版本，一些库维护者更倾向于选择像 HTTPX2 这样能提供 API 稳定性的分支。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pypi.org/project/httpx/">httpx · PyPI</a></li>
<li><a href="https://www.python-httpx.org/">HTTPX</a></li>

</ul>
</details>

**社区讨论**: Hacker News 评论者的反应不一。Simon Willison 确认 Anthropic 也做了同样的切换，并解释说 httpx2 承诺不破坏现有 API，而 jklehm 则想知道是否评估过 niquests 这一替代方案。还有人询问这一改变的好处是什么，tosh 指出 SDK 现在使用操作系统的 TLS 信任库而不是 certifi。

**标签**: `#openai`, `#httpx`, `#python`, `#http-client`, `#sdk`

---

<a id="item-10"></a>
## [新攻击破解 Claude Code 自动模式，成功率 80%](https://simonwillison.net/2026/Aug/27/breaking-claude-code-opus-5-auto-mode/) ⭐️ 8.0/10

安全研究员 Johann Rehberger 展示了一种提示注入攻击，可在约 80%的情况下绕过 Claude Code 的自动模式。该攻击诱使代理解压一个包含恶意本地 struct.py 的压缩包，在导入 base64 时利用该文件遮蔽 Python 标准库并执行攻击者控制的代码。 这直接挑战了 Anthropic 关于自动模式的安全声明，而该模式现已成为 Claude Code 的默认设置。它表明基于 LLM 的安全分类器可以被绕过，凸显了 AI 编程代理需要沙箱和更严格安全实践的必要性。 该攻击的成功率约为 80%，在某些运行中，自动模式甚至在代理发现入侵后阻止了 Claude 自己的清理命令。Rehberger 建议在容器、虚拟机或操作系统沙箱中运行无人值守的编码代理，限制网络出口，并且不要向代理运行时暴露凭证。

rss · Simon Willison · Aug 27, 22:50

**背景**: Claude Code 是 Anthropic 的代理式编程工具，能够在开发者的环境中编辑文件、运行命令和执行代码。自动模式通过 LLM 分类器路由工具调用，阻止不可逆转、破坏性或超出环境范围的操作，取代了旧的--dangerously-skip-permissions 标志。该攻击利用了 Python 的导入行为：与标准库模块同名的本地文件会遮蔽真实模块。这说明了 AI 代理在处理不可信内容时面临更广泛的提示注入风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/engineering/claude-code-auto-mode">How we built Claude Code auto mode: a safer way to skip permissions \ Anthropic</a></li>
<li><a href="https://code.claude.com/docs/en/auto-mode-config">Configure auto mode - Claude Code Docs</a></li>
<li><a href="https://bobbyhadz.com/blog/python-importerror-cannot-import-name">ImportError: cannot import name X in Python [Solved] | bobbyhadz</a></li>

</ul>
</details>

**标签**: `#security`, `#prompt injection`, `#AI agents`, `#LLM`, `#Claude Code`

---

<a id="item-11"></a>
## [OpenAI 被曝开发常驻 Codex 代理，持续工作直至休眠](https://www.wired.com/story/openai-is-developing-a-persistent-ai-agent/) ⭐️ 8.0/10

据 WIRED 审查的代码，OpenAI 正在为 Codex CLI 添加「常驻模式」，让代理跨会话持续工作，直到用户将其休眠。OpenAI 确认正在测试该功能，但未给出上线时间。 常驻代理可能让 AI 编程工具从「一次性问答助手」转变为能主动规划并执行多步骤工程任务的长期协作者。这可能大幅提升开发效率，并加速整个行业向更自主的 AI 代理方向发展。 该模式内置「主动性」设定，代理在答完请求后可自行创建后续任务，并依据对用户的了解跨会话工作。常驻模式并不会扩大代理的权限：改动用户自身系统之外的任何内容仍需事先获得批准。

telegram · zaihuapd · Aug 28, 02:47

**背景**: Codex 是 OpenAI 的 AI 编程代理，2025 年 4 月以终端工具 Codex CLI 的形式发布，现已接入 ChatGPT、桌面应用和多个 IDE。目前的编程代理通常是反应式且无状态的——它们等待用户输入，并在会话结束后丢失上下文——因此持久化记忆与主动创建任务被视为迈向更自主代理的关键步骤。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.wired.com/story/openai-is-developing-a-persistent-ai-agent/">OpenAI Is Developing a ‘ Persistent ’ AI Agent | WIRED</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_Codex_(AI_agent)">OpenAI Codex (AI agent)</a></li>
<li><a href="https://learn.chatgpt.com/docs/codex/cli">Codex CLI | ChatGPT Learn</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#Codex`, `#AI agents`, `#software engineering`, `#AI tools`

---

<a id="item-12"></a>
## [腾讯开源 Hy4 preview：770B 参数 MoE 模型](https://mp.weixin.qq.com/s/ymr3X878B8oa2XP15CH8TQ) ⭐️ 8.0/10

腾讯于 2026 年 8 月 28 日发布并开源了 Hy4 preview，这是一款拥有 770B 总参数、49B 活跃参数的混合专家（MoE）模型。在 203 个工程任务的盲测中，它以 2.99 分略胜 GLM-5.3（2.92）和 Kimi K3（2.94）。 此次发布标志着开源 AI 迈出一大步：腾讯的模型在能力上与国内其他实验室的顶尖模型不相上下。开发者和研究者将获得具有 100 万 token 上下文窗口的前沿级模型，有望加速软件工程、文档处理和科学研究等领域的工作。 模型主干包含 78 层：第一层使用标准稠密 FFN，其余 77 层均为 MoE 层，每层包含 256 个路由专家和 1 个共享专家。API 定价为每百万输入 token 0.834 美元、每百万输出 token 2.501 美元，模型权重已上线腾讯云、GitHub、HuggingFace、ModelScope、AtomGit 和 OpenRouter 等平台。

telegram · zaihuapd · Aug 28, 06:11

**背景**: 混合专家（MoE）架构使得构建超大规模语言模型同时保持较低推理成本成为可能：每个 token 只会激活一部分“专家”参数。这就是 Hy4 preview 总参数达 770B 但每 token 仅激活 49B 的原因。ModelScope 是一个开源平台，提供“模型即服务”（MaaS），方便开发者部署和使用此类模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tencent.com/tencent-releases-and-open-sources-tencent-hy4-preview/">Tencent Releases and Open-Sources Tencent Hy4 preview</a></li>
<li><a href="https://github.com/Tencent-Hunyuan/Hy4-preview">Tencent-Hunyuan/Hy4-preview - GitHub</a></li>
<li><a href="https://www.ibm.com/think/topics/mixture-of-experts">What is mixture of experts? | IBM</a></li>

</ul>
</details>

**标签**: `#AI`, `#LLM`, `#Tencent`, `#open-source`, `#model release`

---

<a id="item-13"></a>
## [Z.ai 发布 GLM-5.3-Flash：320B 总参数、18B 激活，价格降至十分之一](https://t.me/zaihuapd/43471) ⭐️ 8.0/10

Z.ai 发布了 GLM-5 系列首个原生多模态模型 GLM-5.3-Flash，总参数 320B，激活参数仅 18B。它在多项编程和智能体基准上超过 GLM-5.2，价格约为上一代的十分之一，限时 API 输入价格仅为每百万 Tokens 0.075 美元。 此次发布标志着 Z.ai 在“以低成本实现前沿性能”上的重要布局：据称 GLM-5.3-Flash 在编程评测上接近 Claude Opus 4.8，但价格低一个数量级。过去需要高昂前沿模型支持的高批量编程与自动化任务，现在可以通过更实惠的 API 完成，可能重塑 API 定价竞争格局。 限时优惠价格为输入每百万 Tokens 0.075 美元、缓存输入 0.015 美元、输出 0.25 美元，缓存存储暂时免费。作为混合专家（MoE）模型，每个 Token 仅激活 320B 参数中的 18B，这是其高效的关键；该模型在正式发布前曾以匿名身份“Ox Alpha”接受测试。

telegram · zaihuapd · Aug 28, 15:32

**背景**: 混合专家（MoE）是一种神经网络架构，每个 Token 只激活一部分“专家”参数，从而在保持较大模型容量的同时降低计算量。GLM-5.3-Flash 采用了该设计：320B 总参数包含共享部分和专家，但每个 Token 仅使用 18B 激活参数。Z.ai 的 GLM-5.3 系列与 GLM-5.2 使用相同的基础模型，改进主要来自后训练（post-training）而非架构变化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://www.datacamp.com/blog/glm-5-3-flash">GLM-5.3-Flash: Features, Benchmarks, and Pricing | DataCamp</a></li>
<li><a href="https://docs.z.ai/guides/llm/glm-5.3">GLM-5.3 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>

</ul>
</details>

**标签**: `#AI`, `#GLM`, `#multimodal`, `#LLM`, `#API pricing`

---