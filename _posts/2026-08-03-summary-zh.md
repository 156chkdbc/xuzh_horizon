---
layout: default
title: "Horizon Summary: 2026-08-03 (ZH)"
date: 2026-08-03
lang: zh
---

> From 35 items, 7 important content pieces were selected

---

1. [OpenAI Astra 在十项数学难题上取得突破](#item-1) ⭐️ 9.0/10
2. [Karpathy 的鹈鹕推文引发 LLM 矢量图形基准讨论](#item-2) ⭐️ 8.0/10
3. [Kakehashi：在 Linux ARM 上运行 macOS 命令行程序的用户态层](#item-3) ⭐️ 8.0/10
4. [F*：面向证明的通用编程语言](#item-4) ⭐️ 8.0/10
5. [eBay 骚扰案：判赔 5600 万美元](#item-5) ⭐️ 8.0/10
6. [微软支持的公开信支持开放权重 AI 模型](#item-6) ⭐️ 8.0/10
7. [微软确认今年推出 Copilot『超级应用』](#item-7) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI Astra 在十项数学难题上取得突破](https://openai.com/index/ten-advances-in-mathematics/) ⭐️ 9.0/10

OpenAI 宣布，其下一代模型 Astra 的内部版本在十个长期未解决的数学与理论计算机科学问题上取得了新成果，按 GPT-5.6 Sol token 价格计算，每个问题的成本不到 2000 美元。AI 生成的论证由人类合作者整理成论文，并在 Lean 证明助手中完成形式化验证，发布在 openai/ten-proofs 仓库中。 这些成果是迄今为止最有力的证明之一，表明 AI 能够在困扰数学家数十年甚至更久的问题上取得原创性进展。如果得到验证，它们可能加速向‘大数学’——人机大规模协作研究——的转变，不过数学界尚未验证这些证明。 这十个问题涵盖高维球体堆积、非索菲克群的存在性、Connes 刚性猜想反例、算术电路下界、量子并行重复、最近向量问题的难度以及多色 Ramsey 数等。OpenAI 坦诚数学论证由 AI 生成，人类负责整理与形式化，并发布了 Lean 4 形式化证明、论文以及由 LLM 生成的推理过程说明。

telegram · zaihuapd · Aug 1, 07:59

**背景**: Lean 是一个开源的证明助手和函数式编程语言，基于归纳构造演算，数学家可以用它来形式化陈述定理并机械地验证证明。Astra 针对的问题是著名的开放性问题——例如，Connes 刚性猜想询问某些群 von Neumann 代数是否能唯一确定其底层群，而索菲克群则是一类可以被有限对称群逼近的群。使用证明助手意义重大，因为它提供了机器可检查的保证，但底层的数学论证仍需人工审查。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Lean_theorem_prover">Lean theorem prover</a></li>
<li><a href="https://math.ucsd.edu/seminar/connes-rigidity-conjecture">On Connes' rigidity conjecture | Department of Mathematics</a></li>
<li><a href="https://en.wikipedia.org/wiki/Sofic_group">Sofic group</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的评论者和观察者既兴奋又谨慎，将这一时刻比作深蓝（Deep Blue）战胜国际象棋冠军，并引用陶哲轩关于‘大数学’的愿景。一些数学家以一篇随笔所称的‘深刻的精神危机’作出反应，而另一些人则指出关于模型未能解决的问题的信息缺失，并要求 OpenAI 公布实际使用的提示词。

**标签**: `#OpenAI`, `#AI research`, `#mathematics`, `#theorem proving`, `#machine learning`

---

<a id="item-2"></a>
## [Karpathy 的鹈鹕推文引发 LLM 矢量图形基准讨论](https://twitter.com/karpathy/status/2083749667410727319) ⭐️ 8.0/10

Andrej Karpathy 在推文中提到 LLM 绘制鹈鹕的例子，以此强调矢量图形可作为测试模型对物理世界理解的新基准。该推文在 Hacker News 上迅速引发讨论，评论者就这类定性基准的价值和可复现性展开了辩论。 这一事件意义重大，因为它标志着从单纯追求生成图像的视觉美感，转向利用矢量图形来揭示模型是否真正理解物理概念。它可能影响 AI 社区未来如何设计基准，以评估 LLM 在文本之外的推理能力。 推文本身似乎只是 xcancel 镜像链接，原帖中并未包含 Karpathy 使用的具体提示词，因此引发了可复现性方面的担忧。评论者将其与 Simon Willison 的 pelican SVG 基准进行比较，并指出更早的例子，如微软在 GPT-4 评估中要求用 TikZ 画独角兽。

hackernews · delichon · Aug 2, 04:05 · [社区讨论](https://news.ycombinator.com/item?id=49140998)

**背景**: 矢量图形使用路径、形状等几何图元来描述图像，而 SVG 是一种广泛使用的基于文本的格式，因此 LLM 容易以代码形式生成。要用 SVG 画出可识别的鹈鹕，不仅需要语法知识，还需要对鸟类外形和比例的认知模型，这考验了物理推理能力。此前的工作如 Chat2SVG 和 LLM4SVG 已探索了基于 LLM 的矢量图形生成，而 Simon Willison 在 2025 年 11 月提出的 pelican SVG 基准则推广了将这类提示作为定性测试的想法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2025/Nov/25/llm-svg-generation-benchmark/">LLM SVG Generation Benchmark</a></li>
<li><a href="https://chat2svg.github.io/">Chat2SVG: Vector Graphics Generation with Large Language Models and Image Diffusion Models</a></li>

</ul>
</details>

**社区讨论**: 评论者意见不一：有人赞同 jmugan 的说法，认为糟糕的输出正是重点，这类基准能暴露模型对物理世界的理解；而 didibus 则质疑是否有 LLM 真正画出了正确的鹈鹕。consumer451 指出缺少提示词导致 Karpathy 的演示无法复现，iDon 则提到微软早前用 TikZ 画独角兽评估 GPT-4 是更早的先例。

**标签**: `#AI`, `#LLM`, `#benchmarks`, `#vector graphics`, `#Karpathy`

---

<a id="item-3"></a>
## [Kakehashi：在 Linux ARM 上运行 macOS 命令行程序的用户态层](https://github.com/wie-project/kakehashi) ⭐️ 8.0/10

Kakehashi 是一个实验性的用户态翻译层，能够在 Linux aarch64 上原生运行 macOS ARM64 命令行二进制文件。目前可用的原型包括 7-Zip、curl 和 Xcode 的 Git，并已在 Docker/Colima 和 UTM 上验证。 它填补了长期存在的兼容性空白，无需像 Darling 那样完整的系统模拟层，就能把 macOS 二进制文件带到 Linux ARM 上。这可能像 Wine/Proton 对 Windows 应用那样，为 Linux ARM 用户（如 Apple Silicon 时代的二进制文件）打开 macOS 命令行工具和工作流。 该项目以 CLI 优先、无 JIT；它在 Linux aarch64 上加载 Darwin Mach-O 二进制文件，映射一个独立的 libSystem，并翻译 BSD 系统调用。目前 7-Zip 性能比原生 Linux 慢约 5.2 倍，项目已制定了缩小差距的优化路线图。

hackernews · vlad_kalinkin · Aug 2, 16:26 · [社区讨论](https://news.ycombinator.com/item?id=49145937)

**背景**: Mach-O 是 macOS 和 iOS 使用的可执行文件格式，而 Linux 使用 ELF，因此两种二进制文件无法直接互换。兼容层通过翻译外部系统调用并提供库垫片，使外部二进制文件能够在宿主机操作系统上运行。Kakehashi 与 Darling、Wine 的思路类似，但专注于在 Linux ARM64 上运行 macOS 命令行二进制文件，并且作为通过 Cargo 安装的用户态工具实现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/wie-project/kakehashi">GitHub - wie-project/kakehashi: Userspace macOS translation layer for Linux ARM64 · GitHub</a></li>
<li><a href="https://news.ycombinator.com/item?id=49145937">Show HN: Kakehashi – Experimental userspace to run macOS binaries on Linux ARM | Hacker News</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mach-O">Mach-O - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者表现出浓厚兴趣，并将 Kakehashi 与 Darling 进行比较，询问在 Darling 已有 ARM64 PR 的情况下是否可以合并力量。也有人对项目命名提出质疑，并表示项目仍处于早期阶段；还有用户询问类似 ROM 样式的方法——即直接执行原始二进制文件而不重新分发重写库。

**标签**: `#macOS`, `#Linux`, `#ARM`, `#compatibility`, `#userspace`

---

<a id="item-4"></a>
## [F*：面向证明的通用编程语言](https://fstar-lang.org/) ⭐️ 8.0/10

一篇关于 F*（一种面向证明的通用编程语言，用于形式化验证）的 Hacker News 帖子引发了社区的热烈关注，获得了 159 个点赞和 69 条评论。讨论强调了 F* 的成熟度，以及它在将现有 C 代码库迁移到经过验证的代码方面的实际用途。 F* 是一种重要且成熟的面向证明的语言，广泛用于形式化验证和安全研究，例如 Project Everest 项目。Hacker News 上的热烈讨论表明，人们对能够提高软件安全性和正确性的实用形式化验证工具越来越感兴趣。 F* 将依赖类型与 SMT 求解和基于策略的交互式定理证明相结合，默认编译为 OCaml。它还可以通过 KaRaMeL 将代码提取为 C 或 WebAssembly，通过 Vale 提取为汇编代码，但默认情况下 F* 只验证输入的代码，而不执行它。

hackernews · ducktective · Aug 2, 12:31 · [社区讨论](https://news.ycombinator.com/item?id=49143925)

**背景**: 形式化验证是指证明程序满足其行为的形式化规范，从而提供强正确性保证。F* 是一种受 ML 和 OCaml 启发的高级多范式函数式编程语言，专为程序验证和安全软件开发而设计。其富有表现力的依赖类型核心逻辑使得在不同范式中都能进行面向证明的编程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/F*_(programming_language)">F* (programming language) - Wikipedia</a></li>
<li><a href="https://fstar-lang.org/">F*: A Proof-Oriented Programming Language</a></li>
<li><a href="https://github.com/FStarLang/FStar">GitHub - FStarLang/FStar: A Proof-oriented Programming ... Proof-oriented Programming in F* - fstar-lang.org F* (programming language) - Wikipedia F*: A general-purpose proof-oriented programming language ... FStar/README.md at master · FStarLang/FStar · GitHub Proof-Oriented Programming in F* - mtzguido.github.io</a></li>

</ul>
</details>

**社区讨论**: 评论者的反应不一：有人批评 F* 主页缺少代码示例，希望更直接地展示语法和用例；也有人称赞 F* 能在逐步迁移 C 代码库时表达外部库；还有初学者询问 F* 是否在工业界使用以及用于什么软件；此外还出现了一个关于响应式样式表和副作用的玩笑。

**标签**: `#formal verification`, `#programming languages`, `#proof assistants`, `#security`, `#functional programming`

---

<a id="item-5"></a>
## [eBay 骚扰案：判赔 5600 万美元](https://www.ft.com/content/06ec1b03-d4af-40cf-b12a-4ba5a410f6d2) ⭐️ 8.0/10

eBay 高管对一对批评该公司的夫妇（Steiner 夫妇）策划了一场骚扰与恐吓活动。这一事件最终导致 5600 万美元赔偿，以及多名 eBay 安全团队成员被判入狱，其中前高级总监 Jim Baugh 被判处 57 个月监禁。 此案凸显了企业安全团队越权报复批评者所带来的危险。它向科技公司发出强烈信号：此类行为将带来严重的法律和财务后果，并强化了企业安全运营中问责与监督的必要性。 根据检方说法，eBay 安全团队七名成员（包括前警察局长）参与了此次骚扰行动。判决各不相同：前高级经理 Brian Gilbert 被判已服刑时间、一年监督释放和 2 万美元罚款；Jim Baugh 被判 57 个月监禁。

hackernews · JumpCrisscross · Aug 2, 19:19 · [社区讨论](https://news.ycombinator.com/item?id=49147435)

**背景**: eBay 是一个全球在线交易平台。本案涉及 eBay 的全球安全团队——该部门本应负责保护公司安全——但检察官称，该团队却共同对批评 eBay 的 Steiner 夫妇进行骚扰和恐吓。行动包括威胁和监视，案件最终导致刑事判决和向受害者支付 5600 万美元赔偿。

**社区讨论**: 评论者质疑骚扰行为是否仅限于一对夫妇，暗示其他批评者也可能被针对。他们还对前警察局长的参与表示担忧，希望其职业生涯受到调查。部分人转而批评 eBay 的商业做法（如高额收费），另有人引用一条通则：缺乏监督时人们可能会做出不良行为。

**标签**: `#security`, `#corporate ethics`, `#legal`, `#eBay`, `#accountability`

---

<a id="item-6"></a>
## [微软支持的公开信支持开放权重 AI 模型](https://simonwillison.net/2026/Aug/2/open-letters/#atom-everything) ⭐️ 8.0/10

西蒙·威利森重点介绍了近期一系列关于 AI 发展的公开信，其中由微软主导的《开放权重与美国 AI 领导力》公开信获得了包括 NVIDIA、亚马逊和 OpenAI 在内的 235 家公司的签署。Anthropic 发布了相反的回应，另一封名为《Pacing the Frontier》的公开信则聚集了 1324 名前沿 AI 公司员工。 这标志着行业在支持开放权重 AI 模型方面形成了重大共识，直接反对美国政府可能以安全为由施加的限制。Anthropic 与微软支持的签署方之间的分歧凸显了 AI 开放性与风险问题上日益加深的政策分裂。 微软的公开信明确将蒸馏辩护为合法的模型开发技术，而 Anthropic 的回应则呼吁打击工业规模的蒸馏操作。《Pacing the Frontier》公开信由 OpenAI 的 Jakub Pachocki 和 Anthropic 的 Dario Amodei 等人签署，呼吁通过国际治理来调控自动化 AI 发展的节奏。

rss · Simon Willison · Aug 2, 04:16

**背景**: 开放权重 AI 模型会公开其训练后的参数（权重），允许任何人检查、微调和部署，而封闭模型仅通过 API 提供。支持者认为这种透明度能促进创新和分布式审查；批评者则警告，同样的访问权限可能助长恶意行为者或威权政府。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/open-weight-ai-models-why-every-enterprise-should-paying-misra-gi2qc">Open - Weight AI Models : Why Every Enterprise Should Be Paying...</a></li>
<li><a href="https://infercom.ai/blog/open-weight-models-explained/">Open - Weight AI Models : Why They're a Strategic Advantage | Infercom</a></li>

</ul>
</details>

**标签**: `#AI`, `#open source`, `#policy`, `#AI safety`, `#Microsoft`

---

<a id="item-7"></a>
## [微软确认今年推出 Copilot『超级应用』](https://www.theverge.com/tech/972927/microsoft-copilot-super-app-confirmed) ⭐️ 8.0/10

微软 CEO 萨蒂亚·纳德拉在周三的财报电话会议上确认，公司将于今年推出一款 AI『超级应用』，将 Copilot 的聊天、编程和智能体能力整合在一起，同时面向消费者和商用场景。本季度将把这些体验（包括代码功能）合并进一个超级应用中。 此举将微软分散的 AI 工具整合到一个工作空间中，直接对标 OpenAI 的 ChatGPT Work，并标志着行业正转向一体化 AI 平台。它可能重塑开发者工作流，并改变企业大规模部署 AI 智能体的方式。 据纳德拉引用的《财富》报道，该超级应用将整合 Copilot 聊天、GitHub Copilot、Copilot Cowork 和 Autopilot 系统。微软上季度营收增至 900 亿美元，主要由 AI 与云业务推动。

telegram · zaihuapd · Aug 1, 13:18

**背景**: 微软的 Copilot 正从纯粹的聊天助手演变为『Cowork』和『Autopilot』——即能够规划、执行并交付工作的智能体系统，且需经用户批准。Agentic AI 指能够追求目标、使用工具并具有一定自主性的智能体。竞争对手 OpenAI 近期推出了 ChatGPT Work，将 ChatGPT 与 Codex 整合为面向团队的工作空间，凸显了 AI 能力整合的行业趋势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Agentic_AI">Agentic AI</a></li>
<li><a href="https://www.microsoft.com/en-us/microsoft-365/blog/2026/03/09/copilot-cowork-a-new-way-of-getting-work-done/">Copilot Cowork: A new way of getting work done | Microsoft ...</a></li>
<li><a href="https://openai.com/chatgpt-work/">ChatGPT Work for every team | OpenAI</a></li>

</ul>
</details>

**标签**: `#Microsoft`, `#Copilot`, `#AI`, `#Super App`, `#Developer Tools`

---