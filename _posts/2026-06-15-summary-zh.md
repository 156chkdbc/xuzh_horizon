---
layout: default
title: "Horizon Summary: 2026-06-15 (ZH)"
date: 2026-06-15
lang: zh
---

> From 32 items, 8 important content pieces were selected

---

1. [Pyodide 314.0 允许将 WASM wheels 发布到 PyPI](#item-1) ⭐️ 9.0/10
2. [里约热内卢'自主研发'的大模型被曝是现有模型的权重合并](#item-2) ⭐️ 8.0/10
3. [形式验证对 AI 生成代码验证至关重要](#item-3) ⭐️ 8.0/10
4. [对 JavaScript 命运的惊人预言式讽刺演讲](#item-4) ⭐️ 8.0/10
5. [为什么 AI 没有取代软件工程师，而且不会](#item-5) ⭐️ 8.0/10
6. [美一季度 75 个数据中心项目被阻，总值 1300 亿美元](#item-6) ⭐️ 8.0/10
7. [华为开源盘古 2.0 模型，参数达 505B](#item-7) ⭐️ 8.0/10
8. [美国政府以国家安全为由限制 Anthropic 的 Mythos 模型](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Pyodide 314.0 允许将 WASM wheels 发布到 PyPI](https://simonwillison.net/2026/Jun/13/publishing-wasm-wheels/#atom-everything) ⭐️ 9.0/10

Pyodide 314.0 现在允许包维护者将针对 WebAssembly 构建的 Python 包（WASM wheels）直接发布到 PyPI，使用 PEP 783 中定义的新的 PyEmscripten 平台标签。此前这一功能仅限于 Pyodide 维护者。 这大大减轻了 Pyodide 核心维护者的负担，并使更广泛的 Python 社区能够为浏览器中的 Python 贡献软件包。这是一个期待已久的功能，可能加速 Python WASM 运行时的采用。 新的平台标签是 `pyemscripten_2026_0_wasm32`（PEP 783）。Simon Willison 发布了一个演示包 luau-wasm，展示了如何将 C++ 扩展编译为 WASM 并通过 PyPI 分发，使用了 GitHub Actions 和 cibuildwheel。

rss · Simon Willison · Jun 13, 23:55

**背景**: Pyodide 是一个用于 WebAssembly 的 Python 发行版，可在浏览器中运行。此前，Pyodide 维护者必须手动构建和托管超过 300 个包，形成了瓶颈。2025 年最终确定的 PEP 783 定义了 PyEmscripten 平台标签，使得 WASM wheels 能够在 PyPI 上发布。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jun/13/publishing-wasm-wheels/">Publishing WASM wheels to PyPI for use with Pyodide</a></li>
<li><a href="https://peps.python.org/pep-0783/">PEP 783 – Emscripten Packaging | peps.python.org</a></li>
<li><a href="https://pyodide.org/en/stable/console.html">pyodide .org/en/stable/console.html</a></li>

</ul>
</details>

**标签**: `#Pyodide`, `#WASM`, `#PyPI`, `#Python packaging`, `#web assembly`

---

<a id="item-2"></a>
## [里约热内卢'自主研发'的大模型被曝是现有模型的权重合并](https://github.com/nex-agi/Nex-N2/issues/4) ⭐️ 8.0/10

一项调查发现，里约热内卢的大模型 Rio-3.5-Open-397B 并非全新的微调模型，而是现有模型（60% Nex-N2 Pro + 40% Qwen3.5-397B-A17B）的权重合并，几乎没有修改，与'自主研发'的说法相矛盾。 这一事件引发了对开源 AI 开发透明度和归属问题的质疑，尤其是当公共机构声称拥有实际上是现有模型合并的成果时。 分析显示，Rio 模型中的每个权重张量都是两个源模型的线性组合，偏差在数千个标准差以内，这与典型的微调模型（变化更大）不同。

hackernews · unrvl22 · Jun 14, 15:37 · [社区讨论](https://news.ycombinator.com/item?id=48528371)

**背景**: 模型合并是一种技术，将多个预训练大模型的参数组合成一个新模型，无需额外训练，常用方法包括加权平均或 SLERP。这已成为低成本创建新模型的常见方式，但当其被宣称是原创工作时，会引发伦理和归属问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/blog/mlabonne/merge-models">Merge Large Language Models with mergekit</a></li>
<li><a href="https://developer.nvidia.com/blog/an-introduction-to-model-merging-for-llms/">An Introduction to Model Merging for LLMs | NVIDIA Technical Blog</a></li>

</ul>
</details>

**社区讨论**: 社区评论者对缺乏透明度表示担忧，有人推测该模型本应包含蒸馏步骤但未上传。其他人则注意到深度学习模型对权重线性组合的鲁棒性。

**标签**: `#LLM`, `#open-source`, `#model merging`, `#ethics`, `#AI transparency`

---

<a id="item-3"></a>
## [形式验证对 AI 生成代码验证至关重要](https://blog.janestreet.com/formal-methods-at-jane-street-index/?from_theconsensus=1) ⭐️ 8.0/10

Jane Street 的博客文章讨论了随着 AI 生成大量需要验证的代码，形式方法（包括证明自动化和表达力强的类型系统）将变得更加关键。 这一转变强调验证而非编写代码，可能改变程序员的角色，并在 AI 生成代码的时代提高软件可靠性。 文章比较了历史上如 Boyer-Moore 证明器等证明自动化工具与现代方法，社区评论则强调了在 Scala 3 中使用表达力强的类型来防止代码质量问题的实际应用。

hackernews · eatonphil · Jun 14, 12:35 · [社区讨论](https://news.ycombinator.com/item?id=48526633)

**背景**: 形式方法是用于规范、开发和验证软件系统的数学严谨技术。它们使用逻辑、形式语言和类型系统来确保正确性。随着 AI 生成大量代码，人工验证变得不切实际，形式方法因此变得越来越重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Formal_methods">Formal methods</a></li>
<li><a href="https://www.galois.com/what-are-formal-methods">What Are Formal Methods? | Galois</a></li>
<li><a href="https://en.wikipedia.org/wiki/Proof_automation">Proof automation</a></li>

</ul>
</details>

**社区讨论**: 社区评论展示了各种观点：Animats 回忆起早期证明自动化的成功；winwang 在 Scala 3 中使用表达力强的类型来防止 AI 生成代码中的“名词堆积”；brap 质疑形式规范是否只是重复测试或实现。总体而言，讨论热烈但观点多样。

**标签**: `#formal methods`, `#programming`, `#software verification`, `#AI`, `#type systems`

---

<a id="item-4"></a>
## [对 JavaScript 命运的惊人预言式讽刺演讲](https://www.destroyallsoftware.com/talks/the-birth-and-death-of-javascript) ⭐️ 8.0/10

Gary Bernhardt 在 2014 年的一场讽刺演讲中预测，JavaScript 将成为 Web 应用的通用编译目标，并导致 2020 年代的灾难性系统崩溃。鉴于后来 WebAssembly 等发展以及 JavaScript 扩展到多种环境，该演讲被认为具有惊人的前瞻性。 这场演讲已成为 JavaScript 社区的文化试金石，引发关于语言演进、编译目标和单一文化风险的讨论。其预测部分成真，JavaScript 在浏览器、服务器（Node.js）和桌面应用（Electron）中占据主导地位，凸显了其批判的持久相关性。 该演讲于 2014 年进行，早于 WebAssembly 的宣布（2015 年）和 TypeScript 的广泛采用。它特别提到了 asm.js 作为编译目标，而 asm.js 是 WebAssembly 的前身。标题“JavaScript 的诞生与死亡”是对编程语言生命周期的戏谑解读。

hackernews · subset · Jun 14, 12:38 · [社区讨论](https://news.ycombinator.com/item?id=48526661)

**背景**: 编译目标是编译器输出的语言或格式。在 Web 开发中，JavaScript 是浏览器的原生语言。要在 Web 上运行其他语言，必须将其编译为 JavaScript。2014 年，asm.js 是一种早期优化，将 C/C++编译为 JavaScript 的子集以提高性能，后来演变为 WebAssembly（Wasm）——一种在浏览器中以接近原生速度运行的低级二进制格式。该演讲讽刺性地夸大了这些趋势，预言了一个将所有代码都编译为 JavaScript 的脆弱生态系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Compiler">Compiler - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/WebAssembly">WebAssembly</a></li>

</ul>
</details>

**社区讨论**: 评论者注意到该演讲的预见性，有人评论说预测的 2020-2025 年灾难在类型上准确但具体原因不同。其他人观察到 JavaScript 确实通过 WebAssembly 成为编译目标，TypeScript 和 Electron 等技术扩大了其应用范围。总体情绪是对演讲的幽默和前瞻性表示赞赏。

**标签**: `#javascript`, `#webassembly`, `#programming-humor`, `#predictions`, `#compilation-target`

---

<a id="item-5"></a>
## [为什么 AI 没有取代软件工程师，而且不会](https://simonwillison.net/2026/Jun/14/why-ai-hasnt-replaced-software-engineers/#atom-everything) ⭐️ 8.0/10

Arvind Narayanan 和 Sayash Kapoor 认为，数据否定了 AI 导致软件工程大规模裁员的说法，并指出纽约州第一年内没有一家公司在 WARN Act 文件中勾选 AI 披露框。他们确定了抵抗自动化的三个真正瓶颈：决定构建什么、验证交付的内容，以及对代码库和业务的深入人类理解。 这挑战了普遍认为 AI 将很快自动化软件工程工作的看法，表明软件工程师比通常假设的更受保护，而其他职业甚至更能抵御 AI 的颠覆。这一分析为有关 AI 取代工作的炒作提供了基于证据的反叙事。 该文章引用了纽约州 WARN Act 的 AI 披露要求，第一年（2025 年 3 月至 2026 年 3 月）没有任何公司报告与 AI 相关的裁员。它还强调软件工程远不止是编写代码，还包括会议和调试等需要深厚上下文理解的活动。

rss · Simon Willison · Jun 14, 23:54

**背景**: WARN Act（《工人调整和再培训通知法案》）是美国的一项法律，要求拥有 100 名或以上员工的雇主在计划大规模裁员或工厂关闭前提前 60 天通知。2025 年 3 月，纽约州成为第一个在 WARN 申报表中添加 AI 披露复选框的州，允许公司说明裁员是否由 AI 导致。第一年内没有公司勾选此框，表明 AI 尚未在软件工程领域造成广泛的失业。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WARN_Act">WARN Act</a></li>

</ul>
</details>

**标签**: `#AI`, `#software engineering`, `#job displacement`, `#labor market`, `#data analysis`

---

<a id="item-6"></a>
## [美一季度 75 个数据中心项目被阻，总值 1300 亿美元](https://www.tomshardware.com/tech-industry/artificial-intelligence/more-than-75-data-center-build-outs-worth-usd130-billion-have-been-successfully-blocked-in-the-first-four-months-of-2026-bipartisan-opposition-mounts-nationwide-over-fears-of-soaring-power-and-water-costs) ⭐️ 8.0/10

2026 年第一季度，美国全国超过 75 个数据中心建设项目被阻止或推迟，总价值约 1300 亿美元，原因是两党和社区对其能源与水消耗的反对声浪日益高涨。 这一反对浪潮可能减缓 AI 和云计算基础设施的扩张，可能增加科技公司的成本和延迟，并对国家数字经济产生影响。 活跃的草根反对组织数量在三个月内从 396 个激增至 833 个，遍布 49 个州，各州议会及部分联邦议员已提出暂停或监管新建数据中心的法案。

telegram · zaihuapd · Jun 14, 03:03

**背景**: 数据中心是容纳数千台服务器的大型设施，随着 AI 工作负载增加，其电力和冷却用水消耗巨大。这引发了对电网压力、公用事业成本上升和环境影响担忧，导致地方官员和居民形成两党联盟反对新项目。

**标签**: `#data centers`, `#energy`, `#infrastructure`, `#regulation`, `#AI`

---

<a id="item-7"></a>
## [华为开源盘古 2.0 模型，参数达 505B](https://t.me/zaihuapd/41948) ⭐️ 8.0/10

在华为开发者大会 2026 上，华为宣布开源盘古 2.0 模型（openPangu 2.0），包括 505B 参数的 Pro 版和 92B 参数的 Flash 版，均支持 512K token 上下文窗口。公司计划从 6 月 30 日起陆续开源预训练代码等七大组件。 此次发布标志着华为在推进大语言模型技术民主化方面的重要举措，可能挑战 OpenAI 和谷歌等主导者。凭借对昇腾 AI 芯片和鸿蒙的原生优化，开源盘古 2.0 可能加速中国乃至全球的 AI 应用。 505B Pro 版本提供了业界领先的参数规模，而 92B Flash 版本则提供了更高效的选项。两款模型都针对昇腾算力进行了优化，并适配鸿蒙系统，组件开源从 6 月 30 日开始。

telegram · zaihuapd · Jun 14, 08:05

**背景**: 华为的昇腾 AI 芯片是专为高性能 AI 计算设计的神经网络处理器（NPU），用于数据中心和边缘设备。512K 上下文窗口允许模型一次性处理大量文本，支持长文档分析、多轮对话等应用。盘古是华为的基础大模型系列，首次发布于 2021 年。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://e.huawei.com/cn/products/computing/ascend">昇腾计算-华为Ascend-AI计算-华为企业业务</a></li>
<li><a href="https://devtk.ai/zh/blog/llm-context-window-explained/">LLM 上下文窗口详解：从 4K 到 1M Token（2026） - DevTk.AI</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/1913660152676094004">一文看懂华为昇腾芯片 - 知乎 - 知乎专栏</a></li>

</ul>
</details>

**标签**: `#open-source`, `#large language model`, `#Huawei`, `#AI`, `#Pangu`

---

<a id="item-8"></a>
## [美国政府以国家安全为由限制 Anthropic 的 Mythos 模型](https://t.me/zaihuapd/41949) ⭐️ 8.0/10

美国政府向 Anthropic 发出出口管制函件，要求暂停外国公民在美国境内外访问 Fable 5 和 Mythos 5 模型。Anthropic 已遵照执行，关闭了这两款模型对所有客户的访问。 这标志着美国对高级 AI 模型的出口管制显著升级，直接影响模型可用性，并为未来 AI 监管树立先例。它凸显了国家安全对 AI 能力及通过越狱可能被滥用的担忧日益加剧。 商务部此举据称与模型可能被越狱从而带来安全风险的担忧有关。Anthropic 澄清其他 Claude 模型不受影响，并称正在争取尽快恢复访问。

telegram · zaihuapd · Jun 14, 09:06

**背景**: AI 越狱是指绕过 AI 系统伦理护栏、使其执行受限操作的技术。美国工业安全局（BIS）越来越多地将出口管制应用于高级 AI 模型权重，例如 2025 年 1 月的法规。Claude Mythos 是 Anthropic 开发的模型，用于网络安全漏洞发现等任务，尚未公开发布。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Mythos">Claude Mythos - Wikipedia</a></li>
<li><a href="https://www.anthropic.com/claude/mythos">Claude Mythos - Anthropic</a></li>
<li><a href="https://www.sidley.com/en/insights/newsupdates/2025/01/new-us-export-controls-on-advanced-computing-items-and-artificial-intelligence-model-weights">New U.S. Export Controls on Advanced Computing Items and ...</a></li>

</ul>
</details>

**标签**: `#AI regulation`, `#export controls`, `#Anthropic`, `#national security`, `#model access`

---