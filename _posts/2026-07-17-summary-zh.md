---
layout: default
title: "Horizon Summary: 2026-07-17 (ZH)"
date: 2026-07-17
lang: zh
---

> From 37 items, 15 important content pieces were selected

---

1. [Firefox 被编译为 WebAssembly 并在另一浏览器中运行](#item-1) ⭐️ 9.0/10
2. [Kimi K3：2.8 万亿参数开源权重模型](#item-2) ⭐️ 9.0/10
3. [Inkling：975B 参数开源权重 MoE 多模态模型发布](#item-3) ⭐️ 9.0/10
4. [Linus Torvalds 声明 Linux 不反 AI](#item-4) ⭐️ 9.0/10
5. [Claude web_fetch 工具漏洞可通过嵌套链接窃取数据](#item-5) ⭐️ 9.0/10
6. [LM Studio 推出 Bionic，面向开源模型的 AI 代理](#item-6) ⭐️ 8.0/10
7. [交互式线性代数书籍通过沉浸式图形增强学习](#item-7) ⭐️ 8.0/10
8. [Roc 编译器从 Rust 到 Zig 的重写达到功能对等](#item-8) ⭐️ 8.0/10
9. [GOES-19 气象卫星进入安全保持模式](#item-9) ⭐️ 8.0/10
10. [GPT-5.6 Codex 漏洞：无沙箱时可能删除文件](#item-10) ⭐️ 8.0/10
11. [xAI 的 Grok CLI 隐私丑闻导致代码开源](#item-11) ⭐️ 8.0/10
12. [美国 ITC 启动 DRAM 设备 337 调查，三星、谷歌、英伟达被列被调查方](#item-12) ⭐️ 8.0/10
13. [日本拟购 2.75 万块英伟达 Rubin 芯片发展机器人 AI](#item-13) ⭐️ 8.0/10
14. [台积电再投千亿美元在美建厂，Q2 利润增 77%创新高](#item-14) ⭐️ 8.0/10
15. [Truth Social 将向华尔街出售特朗普帖子的快速访问权限](#item-15) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Firefox 被编译为 WebAssembly 并在另一浏览器中运行](https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/#atom-everything) ⭐️ 9.0/10

Puter 已将完整的 Firefox 浏览器编译为 WebAssembly，使其能在另一个浏览器窗口中运行。该演示加载了 233MB 的 gecko.wasm 文件，并使用 WebSocket 代理（Wisp 协议）处理网络流量。 这展示了跨平台浏览器执行的范式转变，证明了一个功能完整的浏览器可以被沙盒化并在任何现代浏览器中运行。它可能开启隔离浏览、测试和无需本地安装的旧版兼容性等新用例。 该项目估计使用了价值 25,000 美元的 Claude Opus 和 Fable 代币，但由于订阅计划实际成本更低。流量通过 Puter 的服务器经由 Wisp 协议路由，团队声称支持端到端加密。

rss · Simon Willison · Jul 16, 23:34

**背景**: WebAssembly (WASM) 是一种二进制指令格式，允许用 C++ 等语言编写的代码以接近原生的速度在 Web 浏览器中运行。将像 Firefox 这样的整个浏览器编译为 WASM 极具挑战性，因为浏览器是管理网络、图形和内存的复杂系统。Puter 是一个在浏览器中运行的云端桌面环境，因此是托管此类演示的天然平台。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://puter.com/">Puter</a></li>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/wisp-protocol: Wisp is a low-overhead, easy to implement protocol for proxying multiple TCP/UDP sockets over a single websocket. · GitHub</a></li>

</ul>
</details>

**标签**: `#WebAssembly`, `#Firefox`, `#Browser`, `#Compilation`, `#Cross-platform`

---

<a id="item-2"></a>
## [Kimi K3：2.8 万亿参数开源权重模型](https://simonwillison.net/2026/Jul/16/kimi-k3/#atom-everything) ⭐️ 9.0/10

月之暗面（Moonshot AI）发布了 Kimi K3，一个拥有 2.8 万亿参数的开源权重模型，在多项基准测试中超越了 GPT-5.5 和 Claude Opus 4.8。该模型已通过 API 和网站提供，开源权重预计在 2026 年 7 月 27 日前发布。 这标志着开源权重 AI 的一个重要里程碑，Kimi K3 是最大的开源权重模型（2.8 万亿参数），挑战了专有模型的领先地位。它表明中国 AI 实验室正在推动开放模型的边界，可能使高性能 AI 更加可及。 该模型支持 100 万 token 上下文，定价为每百万输入 token 3 美元、每百万输出 token 15 美元，是中国最贵的开源权重模型。它还在 Arena.ai 前端代码排行榜上排名第一，超越了 Claude Fable 5。

rss · Simon Willison · Jul 16, 20:19

**背景**: 开源权重模型允许用户下载并运行模型参数到自己的基础设施上，但通常不包括训练数据或代码。虽然密集模型有数十亿参数，但 Kimi K3 可能采用混合专家架构，以在 2.8T 总参数下保持合理的推理成本。'3 万亿参数级别'指的是大约 3T 参数的模型，此前最大的开源权重模型是 DeepSeek-V4 Pro（1.6T）。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://d-central.tech/mining-glossary/open-weight-model/">Open - Weight Model Meaning | Bitcoin Mining Glossary</a></li>
<li><a href="https://macaron.im/blog/deepseek-v4-moe-1-trillion">DeepSeek-V4 MoE: The 1- Trillion Parameter Breakthrough - Macaron</a></li>
<li><a href="https://www.buildfastwithai.com/blogs/qwen3-max-preview-trillion-parameter">Qwen 3 -Max-Preview: Alibaba’s Trillion - Parameter Breakthrough with...</a></li>

</ul>
</details>

**社区讨论**: 评论者注意到该模型的高成本（每任务 0.94 美元），与其他开源权重模型相比价格较高，并讨论了中国实验室是否在商品化 AI 智能。一些人对开源权重的标签以及如此大型模型的经济可行性表示怀疑。

**标签**: `#AI`, `#large language models`, `#open-source`, `#model release`, `#benchmarks`

---

<a id="item-3"></a>
## [Inkling：975B 参数开源权重 MoE 多模态模型发布](https://simonwillison.net/2026/Jul/16/inkling/#atom-everything) ⭐️ 9.0/10

由 Mira Murati 领导的 Thinking Machines Lab 发布了 Inkling，一个拥有 9750 亿参数、410 亿活跃参数的混合专家多模态模型，采用 Apache-2.0 许可证。该模型在 45 万亿个文本、图像、音频和视频 token 上训练而成。 此次发布增强了美国开源权重生态系统，为中国及 NVIDIA/Gemma 模型提供了有力竞争替代方案。它提供了强大的微调基础，可能使先进的多模态 AI 更加普及。 模型卡片异常简短，训练数据文档几乎不包含详细信息。Inkling 并非前沿模型，而是旨在作为通过其 Tinker 训练平台进行定制的强大基础模型；后期将发布更小的 276B（120 亿活跃参数）变体 Inkling-Small。

rss · Simon Willison · Jul 16, 15:35

**背景**: 混合专家（MoE）架构使用多个专门的子网络（'专家'），并通过路由机制为每个输入仅激活部分专家，从而在保持高效推理的同时实现更大的总参数量。开源权重模型公开发布训练后的参数，允许下载、微调和部署，但通常与完全开源不同，可能带有使用限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://datanorth.ai/blog/what-is-mixture-of-experts-moe-and-why-does-it-matter">What is mixture of experts (MoE) and why does it matter?</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>

</ul>
</details>

**标签**: `#open-weights`, `#multimodal`, `#Mixture-of-Experts`, `#AI model`, `#Thinking Machines Lab`

---

<a id="item-4"></a>
## [Linus Torvalds 声明 Linux 不反 AI](https://simonwillison.net/2026/Jul/16/linus-torvalds/#atom-everything) ⭐️ 9.0/10

Linux 内核的创建者和顶级维护者 Linus Torvalds 在 Linux Media 邮件列表中明确表示，Linux 项目不反 AI，他认为 AI 是一个有用的工具，并告诉反对者他们可以 fork 项目或离开。 来自 Linux 内核最高权威的这一声明为整个开源生态系统指明了方向，可能鼓励在开发中更广泛地使用 AI 工具，并减少社区内部的阻力。 Torvalds 承认一年前 AI 的用途还不明确，但现在已毋庸置疑，不过他指出经济问题仍然存在。他的言论是针对内核中 AI 使用的未指明的反对意见而发表的。

rss · Simon Willison · Jul 16, 13:26

**背景**: Linus Torvalds 是 Linux 内核的创建者和长期维护者，Linux 内核为服务器、嵌入式系统和 Android 设备提供支持。他的声明在开源社区中具有极大的影响力。关于 AI 在开源项目中的争论一直存在争议，一些开发者因担心质量、许可和道德问题而反对 AI 生成的代码。

**标签**: `#Linux`, `#AI`, `#Open Source`, `#Kernel Development`, `#Linus Torvalds`

---

<a id="item-5"></a>
## [Claude web_fetch 工具漏洞可通过嵌套链接窃取数据](https://simonwillison.net/2026/Jul/15/claude-web-fetch-exfiltration/#atom-everything) ⭐️ 9.0/10

安全研究员发现，Anthropic 的 Claude web_fetch 工具可通过跟随恶意网站中的嵌套链接来窃取敏感用户数据，绕过了预期的限制。 该漏洞展示了 AI 代理设计中的一个关键缺陷：通过社会工程与技术漏洞的结合，可以绕过数据窃取防护措施，凸显了 LLM 工具中持续存在的风险。 攻击者创建了一个诱饵页面，显示虚假的 Cloudflare 认证提示，诱使 AI 按字母顺序导航子页面以构建用户档案 URL，从而窃取了姓名、城市和雇主信息。Anthropic 已内部发现该问题，并通过阻止 web_fetch 跟随获取内容中的链接来修复了漏洞。

rss · Simon Willison · Jul 15, 14:21

**背景**: Claude 的 web_fetch 工具设计有限制：只能访问用户提供或来自 web_search 工具返回的精确 URL，从而防止直接数据窃取。但它可以跟随获取页面中的链接。此漏洞是“致命三重奏”攻击模式的例子，即 AI 代理可访问私有数据、处理不可信内容并能外部通信，从而通过提示注入窃取信息。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/">The lethal trifecta for AI agents: private data, untrusted content, and external communication</a></li>
<li><a href="https://simonwillison.net/2025/Sep/10/claude-web-fetch-tool/">Claude API: Web fetch tool</a></li>

</ul>
</details>

**标签**: `#AI security`, `#data exfiltration`, `#Claude`, `#prompt injection`, `#LLM vulnerabilities`

---

<a id="item-6"></a>
## [LM Studio 推出 Bionic，面向开源模型的 AI 代理](https://lmstudio.ai/blog/introducing-lm-studio-bionic) ⭐️ 8.0/10

LM Studio 推出了 Bionic，这是一个代理工作流工具，允许用户使用本地和托管的开源模型运行 AI 代理。它支持编码和文档创建，并具有自动检查点等功能。 这一发布将代理式 AI 能力带到了本地和开源模型，使更广泛的用户无需完全依赖云端 API 即可使用高级工作流。它使 LM Studio 成为注重隐私的企业和希望控制成本及数据的开发者的关键平台。 Bionic 支持 Qwen3.6 35B 等模型，并提供用于编码的 Code 项目和带有每次代理更改自动检查点的 Work 项目。创始人还提供了免费额度，以便用户试用 GLM 5.2 和 Kimi K2.6 等模型。

hackernews · minimaxir · Jul 16, 20:18 · [社区讨论](https://news.ycombinator.com/item?id=48939662)

**背景**: LM Studio 是一个流行的用户友好工具，用于在个人电脑上运行本地大语言模型（LLM），无需命令行专业知识。代理式工作流涉及 AI 代理自主规划和执行任务，几乎不需要人工干预，通常使用外部工具和 API。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lmstudio.ai/download">Download LM Studio - Mac, Linux, Windows</a></li>
<li><a href="https://www.ibm.com/think/topics/agentic-workflows">What are Agentic Workflows? | IBM</a></li>

</ul>
</details>

**社区讨论**: 早期用户给出了正面评价，有人指出使用 Qwen3.6 35B 性能流畅，且 UI 与 Codex 类似。创始人与社区直接互动，为特定模型提供免费额度。一些人担心商业模式向云服务转变，而另一些人则质疑其与现有代理框架的区别。

**标签**: `#LM Studio`, `#AI agent`, `#local LLMs`, `#open-source models`, `#coding assistant`

---

<a id="item-7"></a>
## [交互式线性代数书籍通过沉浸式图形增强学习](https://immersivemath.com/ila/) ⭐️ 8.0/10

一本 2015 年发布的免费在线线性代数书籍，内置交互式 3D 图形，读者可以在浏览器中直接操作和探索数学概念。 这本书展示了交互性如何使抽象的数学概念更直观，有可能改善学习效果，并启发其他 STEM 领域采用类似方法。 该书涵盖向量、矩阵、特征值和线性变换等标准线性代数主题，每个交互式图形都配有解释性文本和工具提示。

hackernews · srean · Jul 16, 15:32 · [社区讨论](https://news.ycombinator.com/item?id=48935951)

**背景**: 线性代数是数学的基础分支，广泛应用于计算机图形学、机器学习和工程学。传统教科书使用静态图表，而交互式可视化允许学生旋转、缩放和更改参数，从而增强空间理解。

**社区讨论**: 社区高度赞扬这本书，用户表示希望自己学习时也能有这样的资源，并建议扩展到统计学、概率学和机器人学。一些评论者指出，AI 和大语言模型的进步使得创建类似的交互式内容更容易，可能带来一波新的教育工具。

**标签**: `#linear algebra`, `#education`, `#interactive`, `#math`, `#visualization`

---

<a id="item-8"></a>
## [Roc 编译器从 Rust 到 Zig 的重写达到功能对等](https://rtfeldman.com/rust-to-zig) ⭐️ 8.0/10

Roc 编译器团队宣布，经过一年半的时间，他们用 Zig 重写编译器的工作已达到与原有 Rust 编译器相同的功能，涉及约 30 万行代码。 这一里程碑证明了将大型系统项目从 Rust 迁移到 Zig 的可行性，突显了 Zig 在更快的编译、更简单的交叉编译以及更灵活的 unsafe 代码处理方面的优势，对编译器开发者具有重要参考价值。 文章指出，编译器经常需要执行内存不安全操作（如热补丁），这是切换语言的原因之一。Zig 的 ReleaseSafe 模式通过运行时检查捕获 use-after-free 错误，但一些评论者质疑其效果。

hackernews · jorangreef · Jul 16, 11:39 · [社区讨论](https://news.ycombinator.com/item?id=48933149)

**背景**: Roc 是一种快速、友好的函数式编程语言。其编译器最初用 Rust 编写，但团队决定用 Zig 重写，以利用 Zig 的快速编译、优秀的交叉编译支持以及更直接的 unsafe 代码处理方式。重写耗时 1.5 年，最近达到了与原始编译器相同的功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.roc-lang.org/">The Roc Programming Language</a></li>
<li><a href="https://github.com/roc-lang/roc">GitHub - roc-lang/roc: A fast, friendly, functional language. The Roc Programming Language roc/docs/mini-tutorial-new-compiler.md at main · roc-lang/roc ROCm Software - AMD The Complete Roc Guide: From Zero to Expert - kodikra How Our Rust-to-Zig Rewrite is Going</a></li>

</ul>
</details>

**社区讨论**: steveklabnik 质疑了编译器必然需要内存不安全操作的说法，认为只有热补丁等特定特性才需要 unsafe 代码。landr0id 对 Zig 运行时 use-after-free 检测的有效性提出疑问，而 onlyrealcuzzo 称赞 Zig 的增量编译功能，但表达了对安全性的担忧。

**标签**: `#Rust`, `#Zig`, `#compilers`, `#memory safety`, `#systems programming`

---

<a id="item-9"></a>
## [GOES-19 气象卫星进入安全保持模式](https://www.spaceweather.gov/news/goes-19-safe-hold) ⭐️ 8.0/10

GOES-19 气象卫星于 2026 年 7 月 15 日进入安全保持模式，但工程师已恢复 DCS 和 SAR 服务，并计划在 1900Z 前恢复 ABI 成像。 GOES-19 是追踪大西洋飓风和墨西哥湾沿岸天气的主要卫星；即使短暂中断也可能影响飓风季的实时预报和公共安全。 恢复顺序为 ABI、GLM、SUVI 和 CCOR 仪器，恢复后第一小时图像导航可能略有降级。卫星在 24 小时内恢复服务。

hackernews · yabones · Jul 16, 13:30 · [社区讨论](https://news.ycombinator.com/item?id=48934286)

**背景**: 安全保持（或安全模式）是航天器的一种运行状态，非必要系统关闭，仅保留热控和通信等关键功能。GOES-19 是 NOAA GOES-R 系列的第四颗也是最后一颗卫星，从地球静止轨道提供连续气象监测。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Safe_mode_in_spacecraft">Safe mode in spacecraft - Wikipedia</a></li>
<li><a href="https://www.nola.com/news/hurricane/weather-satellite-goes-19-out/article_75a9d7be-1e36-4bf1-b55f-26ff9a369157.html">GOES 19 satellite used to track Gulf hurricanes is offline | Hurricane Center | nola.com</a></li>

</ul>
</details>

**社区讨论**: 一位前 GOES 工程师指出，整个 GOES 系列异常现象很常见，列举了 GOES-17 的热管异常和 GOES-13 的燃料箱问题等问题。评论者还表示恢复进展迅速，此次中断凸显了预报对卫星数据的依赖。

**标签**: `#weather satellite`, `#GOES-19`, `#safe hold mode`, `#NOAA`, `#hurricane tracking`

---

<a id="item-10"></a>
## [GPT-5.6 Codex 漏洞：无沙箱时可能删除文件](https://simonwillison.net/2026/Jul/16/bad-codex-bug/#atom-everything) ⭐️ 8.0/10

OpenAI 的 GPT-5.6 Codex 代理存在一个漏洞：当启用完全访问模式且未开启沙箱或自动审查时，模型可能意外删除文件。原因是模型尝试覆盖 $HOME 环境变量后，错误地删除了 $HOME 目录。 该漏洞对在生产环境中使用 Codex 的开发人员构成重大数据丢失风险，凸显了在自主部署 AI 编码代理时，沙箱和审查保护措施的至关重要性。 该漏洞具体发生在 Codex 以完全访问模式运行、无沙箱、无自动审查，且模型尝试通过覆盖 $HOME 环境变量设置临时目录，但错误地删除了 $HOME 目录时。

rss · Simon Willison · Jul 16, 17:45

**背景**: OpenAI Codex 是一个用于软件工程任务的 AI 编码代理，如编写代码和修复错误，于 2025 年 4 月以 Codex CLI 形式发布。它可以使用不同级别的系统访问权限；无沙箱的完全访问模式赋予代理不受限制的文件系统权限，这可能在模型出错时导致破坏性操作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_Codex_(AI_agent)">OpenAI Codex (AI agent) - Wikipedia</a></li>
<li><a href="https://www.docker.com/products/docker-sandboxes/">Sandboxes for Coding Agents - Docker</a></li>

</ul>
</details>

**标签**: `#codex`, `#coding-agents`, `#generative-ai`, `#ai-safety`, `#security`

---

<a id="item-11"></a>
## [xAI 的 Grok CLI 隐私丑闻导致代码开源](https://simonwillison.net/2026/Jul/15/grok-build/#atom-everything) ⭐️ 8.0/10

xAI 的 Grok CLI 工具被发现会上传整个用户目录到云端，包括 SSH 密钥和密码数据库。作为回应，xAI 删除了所有之前上传的用户数据，禁用了该功能，并以 Apache 2.0 许可证发布了 Grok Build 代码库。 这一事件严重损害了 AI 编码工具的信任，尤其是那些集成到开发者环境中的工具。被动的开源或许有助于重建信心，但它凸显了能够访问本地文件的云端 AI 智能体存在关键隐私风险。 Grok Build 代码库包含 844,530 行 Rust 代码（仅 3% 为第三方依赖），并以单个提交发布，因此看不到开发历史。它包含一个自包含的 Mermaid 图表终端渲染器，以及受 Codex 和 OpenCode 启发的工具实现。

rss · Simon Willison · Jul 15, 23:59

**背景**: Grok CLI 是一个在终端中运行的 AI 驱动编码代理，类似于 GitHub Copilot 等工具。默认情况下，它会将当前目录内容上传到 xAI 的服务器，导致用户无意中暴露敏感文件。社区的强烈反对促使 xAI 立即采取了行动。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.ai/cli">Grok Build | SpaceXAI</a></li>
<li><a href="https://lalatenduswain.medium.com/automate-your-terminal-with-grok-cli-a-developers-guide-to-xai-s-ai-powered-tool-eb8e2b0460bf">Automate Your Terminal with Grok CLI : A Developer’s Guide... | Medium</a></li>

</ul>
</details>

**社区讨论**: 社交媒体上的用户报告描述了 SSH 密钥、密码数据库和个人文档被上传的情况。整体情绪是对隐私侵犯的愤怒，许多人批评缺乏同意和透明度。一些人对开源表示赞赏，但对未来的信任仍持怀疑态度。

**标签**: `#privacy`, `#security`, `#open-source`, `#xAI`, `#CLI`

---

<a id="item-12"></a>
## [美国 ITC 启动 DRAM 设备 337 调查，三星、谷歌、英伟达被列被调查方](https://www.cls.cn/detail/2428105) ⭐️ 8.0/10

美国国际贸易委员会（ITC）于 7 月 15 日投票决定启动编号为 337-TA-1511 的 337 调查，针对特定 DRAM 设备及其下游产品和组件，该调查源于 Netlist 提出的专利侵权投诉。被调查方包括三星电子、谷歌、英伟达、博通和超微电脑等公司。 该调查涉及用于 AI 服务器和数据中心的 DDR5 DIMM 及高带宽内存（HBM），可能扰乱主要科技公司的供应链。如果 ITC 裁定 Netlist 胜诉，侵权产品的进口可能被禁止，从而影响云服务和 AI 算力成本。 投诉具体提及 DDR5 DIMM 模块、HBM 堆叠以及使用这些存储器的服务器、计算和存储系统。调查尚处于初期阶段，最终裁定可能需要 12-18 个月，短期内不太可能对消费电子产品价格产生影响。

telegram · zaihuapd · Jul 16, 08:34

**背景**: 《1930 年关税法》第 337 条授权美国 ITC 调查进口商品中的不公平贸易行为，包括专利侵权。如果认定违规，ITC 可以发布排除令，禁止涉案产品进入美国。DDR5 DIMM 是最新一代双列直插内存模块，而 HBM 是一种 3D 堆叠 DRAM 架构，为 AI 和高性能计算提供极高带宽。Netlist 是一家内存技术公司，此前曾与主要 DRAM 制造商发生过专利诉讼。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DDR5_SDRAM">DDR5 SDRAM - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://www.mti-worldwide.com/current-events-worldwide-logistics-blog/usitc-institutes-section-337-investigation-of-certain-vaporizer-devices-cartridges-used-therewith-and-components-thereof">USITC Institutes section 337 investigation of certain...</a></li>

</ul>
</details>

**标签**: `#DRAM`, `#专利调查`, `#供应链`, `#半导体`, `#美国ITC`

---

<a id="item-13"></a>
## [日本拟购 2.75 万块英伟达 Rubin 芯片发展机器人 AI](https://www.bloomberg.com/news/articles/2026-07-16/japan-to-buy-nvidia-rubin-chips-to-build-sovereign-ai-for-robots) ⭐️ 8.0/10

日本宣布计划购入 27500 块英伟达 Rubin 芯片，由新成立的公司 Noetra 牵头建设大型数据中心，用于开发面向机器人的本土 AI 模型，获得政府拨款 3873 亿日元（约 24 亿美元）。 该项目旨在减少日本对外国 AI 技术的依赖，并力争到 2040 年占据全球机器人市场 30%以上份额，在地缘政治 AI 主权竞争中具有重要意义。 Noetra 计划明年 3 月发布首个 AI 模型，并在数年内推出机器人专用版本。该联盟包括软银、丰田支持的 Preferred Networks 和 NEC。

telegram · zaihuapd · Jul 16, 10:59

**背景**: 英伟达 Rubin 是下一代 GPU 微架构，以天体物理学家 Vera Rubin 命名，于 2024 年发布。'主权 AI'指国家发展独立 AI 能力的努力，包括基础设施、数据和模型，以减少对外国供应商的依赖。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Rubin_(microarchitecture)">Rubin (microarchitecture) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Sovereign_AI">Sovereign AI</a></li>

</ul>
</details>

**标签**: `#nvidia`, `#rubin`, `#robotics`, `#sovereign AI`, `#japan`

---

<a id="item-14"></a>
## [台积电再投千亿美元在美建厂，Q2 利润增 77%创新高](https://www.reuters.com/world/asia-pacific/tsmcs-second-quarter-profit-seen-hitting-record-ai-boom-2026-07-15/) ⭐️ 8.0/10

台积电宣布再在亚利桑那州投资 1000 亿美元建厂，在美总投资达 1650 亿美元；同时公布二季度净利润同比飙升 77%至 7066 亿新台币（约 220 亿美元），创历史新高，受 AI 需求驱动。 这凸显出台积电为分散制造基地、降低地缘政治风险的战略扩张，以及在 AI 浪潮中的核心地位——创纪录的利润表明 AI 芯片需求持续强劲。 台积电将 2026 年资本支出预测上调至 600 亿-640 亿美元，并预计全年美元营收增长略超 40%。亚利桑那州目前已有 8 座工厂在建或规划中，未来可能再增 4 座。

telegram · zaihuapd · Jul 16, 12:29

**背景**: 台积电是全球最大的晶圆代工厂，为苹果、英伟达等公司生产先进芯片。由于地缘政治紧张，台积电一直在扩大在美国的布局。AI 热潮极大地增加了对其尖端半导体制造服务的需求。

**标签**: `#TSMC`, `#semiconductor`, `#AI`, `#investment`, `#profit`

---

<a id="item-15"></a>
## [Truth Social 将向华尔街出售特朗普帖子的快速访问权限](https://www.cnn.com/2026/07/16/business/truth-social-data-wall-street) ⭐️ 8.0/10

特朗普媒体科技集团（TMTG）于 2026 年 7 月 16 日宣布，将从 8 月 1 日起推出 Truth API，向机构客户提供毫秒级访问 Truth Social 平台排名前 10 账号（包括唐纳德·特朗普）实时帖子的权限。该服务明确面向寻求在金融市场中获得信息优势的高频算法交易者。 此举引发了重大的道德和市场诚信担忧，因为它将总统的社交媒体帖子货币化，让高速交易者直接获利，可能使他们能够在市场对特朗普政策公告做出反应之前抢先交易。这也模糊了公共沟通与私人商业利益之间的界限，尤其是考虑到特朗普曾利用 Truth Social 宣传自己刚刚投资的股票。 该 API 以毫秒级速度提供数据，针对依赖速度的高频算法交易策略。TMTG 尚未披露具体定价。特朗普的 Truth Social 账号已成为宣布关税、伊朗及霍尔木兹海峡等政策决定的主要渠道，这些帖子此前曾多次引发股市和油市剧烈波动。

telegram · zaihuapd · Jul 17, 01:02

**背景**: 算法交易使用计算机程序根据预定义规则自动执行交易，通常利用速度和数据优势来超越人类。高频交易（HFT）是其子集，需要极低延迟才能从微小价格波动中获利。Truth Social 是在特朗普被主流平台封禁后推出的，现已成为他的主要社交媒体渠道，其帖子经常影响市场。将实时数据直接出售给交易者，对于与政治人物相关的社交平台而言，是一种新颖且有争议的收入来源。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://marketchameleon.com/articles/b/2026/7/16/trump-media-launches-truth-api-institutional-market-impact">Trump Media Unveils Truth API: Real-Time Access to ...</a></li>
<li><a href="https://www.cnbc.com/2026/07/16/trump-truth-social-wall-street-traders-api.html">Truth Social launches service to give Wall Street traders an ...</a></li>

</ul>
</details>

**标签**: `#Truth Social`, `#data API`, `#algorithmic trading`, `#finance`, `#ethics`

---