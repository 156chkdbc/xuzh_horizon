---
layout: default
title: "Horizon Summary: 2026-07-09 (ZH)"
date: 2026-07-09
lang: zh
---

> From 38 items, 14 important content pieces were selected

---

1. [TypeScript 7 发布，基于 Rust 重写](#item-1) ⭐️ 9.0/10
2. [Cloudflare Meerkat：首个生产级异步共识算法](#item-2) ⭐️ 9.0/10
3. [Bun 从 Zig 重写为 Rust：AI 辅助代码迁移案例](#item-3) ⭐️ 9.0/10
4. [安卓全版本高危漏洞链实现远程 Root](#item-4) ⭐️ 9.0/10
5. [约翰迪尔与 FTC 达成和解，推进维修权](#item-5) ⭐️ 8.0/10
6. [OpenAI 关于去除编码基准中的噪声](#item-6) ⭐️ 8.0/10
7. [Mistral 推出 Robostral Navigate，实现无地图机器人导航](#item-7) ⭐️ 8.0/10
8. [微软发布 Flint，面向 AI 代理的可视化语言](#item-8) ⭐️ 8.0/10
9. [xAI 发布 Grok 4.5：低成本高效能但饱受争议](#item-9) ⭐️ 8.0/10
10. [OpenAI 推出 GPT-Live 语音模式，可委托 GPT-5.5 推理](#item-10) ⭐️ 8.0/10
11. [sqlite-utils 4.0 发布，支持数据库模式迁移](#item-11) ⭐️ 8.0/10
12. [华为 5G 旗舰重返海外，峰值速率超 1100Mbps](#item-12) ⭐️ 8.0/10
13. [Cloudflare 与 OpenAI 合作试点全球网络数据优化 AI 搜索](#item-13) ⭐️ 8.0/10
14. [通过电磁信号识别手机应用，准确率达 99.07%](#item-14) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [TypeScript 7 发布，基于 Rust 重写](https://devblogs.microsoft.com/typescript/announcing-typescript-7-0/) ⭐️ 9.0/10

微软发布了 TypeScript 7.0，这是一个重大版本，其全新架构基于 Rust 重写，与 TypeScript 6 相比，构建速度最高提升 11.9 倍。 这一性能飞跃解决了 TypeScript 编译速度长期存在的问题，使其对 VS Code、Sentry 和 Playwright 等大型代码库更加高效，并可能推动类型化 JavaScript 的更广泛采用。 基准测试显示，不同代码库的加速效果在 7.7 倍到 11.9 倍之间；用 Rust 重写取代了之前基于 TypeScript 的编译器，通过原生性能和并行化实现了这些提升。

hackernews · DanRosenwasser · Jul 8, 16:06 · [社区讨论](https://news.ycombinator.com/item?id=48833715)

**背景**: TypeScript 是 JavaScript 的类型化超集，可编译为纯 JavaScript。其编译器（tsc）历史上一直用 TypeScript 自身编写，导致大型项目出现性能瓶颈。多年来一直有关于用 Rust 重写的猜测，社区项目如 STC 也曾尝试过，但微软的官方努力现在带来了显著的改进。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.totaltypescript.com/rewriting-typescript-in-rust">Rewriting TypeScript in Rust? You'd have to be... | Total TypeScript</a></li>
<li><a href="https://medium.com/nerd-for-tech/curious-why-microsoft-did-not-use-rust-to-rewrite-the-typescript-compiler-16f1611bfd1d">Curious why Microsoft did not use Rust to rewrite the TypeScript Compiler? | by Olenin Slava | Nerd For Tech | Medium</a></li>

</ul>
</details>

**社区讨论**: 社区表达了兴奋和祝贺，许多人注意到同时维护两个代码库的工程壮举令人印象深刻。一些用户强调了 JSDoc 类型语法的持续支持以及对开发者体验的影响。

**标签**: `#TypeScript`, `#performance`, `#programming languages`, `#compiler`, `#Microsoft`

---

<a id="item-2"></a>
## [Cloudflare Meerkat：首个生产级异步共识算法](https://blog.cloudflare.com/meerkat-introduction/) ⭐️ 9.0/10

Cloudflare 推出了 Meerkat，这是 QuePaxa 异步共识算法的首个生产实现，专为全球分布式系统设计。 这是一个突破性进展，它将能够抵御网络延迟和超时的异步共识从理论带入实际部署，有望提高在恶劣网络条件下运行的分布式系统的可靠性。 Meerkat 是无领导且不依赖超时的，与 Paxos 和 Raft 等传统共识算法不同。然而，它需要对每次读取操作进行全局共识，这可能会引入额外的延迟。

hackernews · bobnamob · Jul 8, 13:18 · [社区讨论](https://news.ycombinator.com/item?id=48831565)

**背景**: 共识算法对于分布式系统在故障情况下达成一致至关重要。传统的 Paxos 和 Raft 等算法是部分同步的，依赖超时来保证活性，在不稳定的网络中可能引发问题。异步共识算法（如 QuePaxa）不依赖超时，因此更具鲁棒性，但实现高效难度较大。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bford.info/pub/os/quepaxa/">QuePaxa: Escaping the Tyranny of Timeouts in Consensus – Bryan Ford's Home Page</a></li>
<li><a href="https://en.wikipedia.org/wiki/Consensus_(computer_science)">Consensus (computer science) - Wikipedia</a></li>
<li><a href="https://github.com/dedis/quepaxa">GitHub - dedis/quepaxa: This is the code repository for QuePaxa project (formerly Raxos or QSCOD) · GitHub</a></li>

</ul>
</details>

**社区讨论**: 社区评论既表达了兴奋也表达了怀疑。一些人赞赏生产级异步共识实现的新颖性，而另一些人则质疑其与无领导协议相比的性能，并指出读取操作需要共识，可能限制使用场景。还有关于与 Raft 比较是否公平的争论，因为 Raft 是专门基于领导的。

**标签**: `#distributed systems`, `#consensus algorithms`, `#asynchronous consensus`, `#QuePaxa`, `#Cloudflare`

---

<a id="item-3"></a>
## [Bun 从 Zig 重写为 Rust：AI 辅助代码迁移案例](https://simonwillison.net/2026/Jul/8/rewriting-bun-in-rust/#atom-everything) ⭐️ 9.0/10

Jarred Sumner 宣布 Bun 已从 Zig 重写为 Rust，使用了 AI 编码代理，带来了改进的稳定性、5% 的性能提升和 20% 的二进制体积缩小。 这表明传统上被认为风险过大的大规模重写现在借助 AI 变得可行，并且验证了 Rust 的内存安全性对像 Bun 这样的性能关键型运行时的优势。 重写花费了约 165,000 美元的 API 代币（59 亿未缓存输入代币、6.9 亿输出代币），由一名工程师使用 Claude Code 和 Fable 在 11 天内完成，TypeScript 测试套件充当了符合性测试套件。

rss · Simon Willison · Jul 8, 23:57

**背景**: Bun 是一个快速的 JavaScript 运行时和工具链，最初用 Zig 编写。Zig 是一种提供手动内存管理的底层语言，而 Rust 通过其所有权模型提供内存安全性。在 Zig 中混合垃圾回收的 JavaScript 与手动内存管理导致了释放后使用和双重释放等 bug，促使了这次重写。重写利用了代理工程（agentic engineering），即 AI 代理在测试套件的指导下自主执行编码任务，这种方法在 2026 年得到了广泛应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/guides/agentic-engineering-patterns/what-is-agentic-engineering/">What is agentic engineering? - Agentic Engineering Patterns - Simon Willison's Weblog</a></li>
<li><a href="https://www.langchain.com/blog/agentic-engineering-redefining-software-engineering">Agentic Engineering: How Swarms of AI Agents Are Redefining Software Engineering</a></li>
<li><a href="https://en.wikipedia.org/wiki/Garbage_collection_(computer_science)">Garbage collection (computer science) - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论强调，这次重写是对 Rust 内存安全性的强烈认可，并显示了与雇佣工程师相比，AI 辅助重写的成本效益。一些人指出，单纯的重写就改善了稳定性和性能，这对 Zig 来说不是好事；其他人则注意到强大的测试套件在启用基于 LLM 的代码生成方面的作用。

**标签**: `#Bun`, `#Rust`, `#Zig`, `#JavaScript runtime`, `#software engineering`

---

<a id="item-4"></a>
## [安卓全版本高危漏洞链实现远程 Root](https://www.coolapk.com/feed/72700258?s=ZGQ2MTVlZjYxMDYyNTM3ZzZhNGUzOThjega1640) ⭐️ 9.0/10

安全公司 Nebula 披露了一个影响所有安卓版本（包括安卓 17）的远程 Root 漏洞链，该链结合了 Firefox 浏览器漏洞和一个潜伏 15 年的 Linux 内核漏洞（CVE-2026-43499，GhostLock）。概念验证代码已发布在 GitHub 上，厂商已收到通知。 此漏洞链允许攻击者仅通过诱使用户点击恶意链接即可在任意安卓设备上获得持久 Root 权限，对数亿用户构成巨大威胁。这凸显了及时修复补丁的重要性以及移动平台中遗留内核漏洞的风险。 该漏洞链利用 Firefox 浏览器漏洞（影响 151.0.2 及更早版本）实现代码执行，然后利用 GhostLock（CVE-2026-43499）进行内核级权限提升至 Root。攻击在一分钟内完成，并通过 ADB 获得设备完全控制权；Linux 内核已发布修复，但安卓补丁尚未就绪。

telegram · zaihuapd · Jul 8, 13:01

**背景**: Android Debug Bridge (ADB) 是一种命令行工具，允许开发者与安卓设备通信以进行调试和控制。"远程 Root" 漏洞使攻击者无需物理接触设备即可获取超级用户（Root）权限。GhostLock（CVE-2026-43499）是 Linux 内核实时互斥锁（rt-mutex）代码中的一个存在 15 年的释放后使用漏洞，于 2011 年引入，影响此后大多数 Linux 发行版。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://threat-modeling.com/cve-2026-43499-ghostlock-linux-kernel-root-container-escape/">CVE-2026-43499 "GhostLock": 15-Year-Old Linux Kernel Flaw Gives Local Users Root Access and Container Escape — Public PoC Released - Threat-Modeling.com</a></li>
<li><a href="https://thehackernews.com/2026/07/15-year-old-ghostlock-flaw-enables-root.html">15-Year-Old GhostLock Flaw Enables Root and Container Escape on Most Linux Distros</a></li>
<li><a href="https://developer.android.com/tools/adb">Android Debug Bridge (adb) | Android Studio | Android Developers</a></li>

</ul>
</details>

**标签**: `#Android`, `#security`, `#vulnerability`, `#Linux kernel`, `#remote root`

---

<a id="item-5"></a>
## [约翰迪尔与 FTC 达成和解，推进维修权](https://apnews.com/article/john-deere-right-to-repair-agriculture-equipment-cb7514ffedb95c130a976af661f2bc02) ⭐️ 8.0/10

约翰迪尔与联邦贸易委员会（FTC）及五个州达成和解，同意允许设备所有者和独立维修店自行修理其设备。 这一和解是维修权运动的一个里程碑式胜利，可能减少修理垄断，降低农民和消费者的成本。 作为和解的一部分，约翰迪尔将向五个州合计支付 100 万美元，并在 10 年内接受合规监督。

hackernews · djoldman · Jul 8, 23:37 · [社区讨论](https://news.ycombinator.com/item?id=48838876)

**背景**: 维修权运动倡导消费者自行修理所购产品的能力，而制造商常通过专有工具和软件锁来限制。约翰迪尔因限制维修手册和零件的获取而成为主要目标。

**社区讨论**: 评论者赞扬了像路易斯·罗斯曼这样的活动家，并指出罚款相对于约翰迪尔的利润来说很小，质疑执法的威慑效果。有人对这类基本自由需要诉讼感到沮丧，而另一些人则指出了科技行业在类似做法上的虚伪辩护。

**标签**: `#right-to-repair`, `#FTC`, `#John Deere`, `#consumer rights`, `#hardware`

---

<a id="item-6"></a>
## [OpenAI 关于去除编码基准中的噪声](https://openai.com/index/separating-signal-from-noise-coding-evaluations/) ⭐️ 8.0/10

OpenAI 发布了一项分析，指出许多编码基准测试任务存在误导性提示或无意中测试指令遵循等缺陷，并手动清理了 SWE-bench 中超过 800 个任务以提高信号准确性。 这项工作凸显了当前 AI 编码评估的脆弱性，并推动该领域走向更严格、更有意义的基准测试，这对于准确衡量模型能力和避免结果虚高至关重要。 分析发现 SWE-bench 中约 20% 的任务存在问题，如误导性提示、无需正确代码即可通过的测试，或隐藏的预训练数据污染；OpenAI 利用模型自身来帮助发现这些问题。

hackernews · sk4rekr0w · Jul 8, 21:03 · [社区讨论](https://news.ycombinator.com/item?id=48837396)

**背景**: 像 SWE-bench 这样的编码评估基准用于衡量 AI 模型解决实际软件工程任务的能力。然而，许多基准存在“噪声”，例如模糊的提示或有缺陷的测试用例，这可能导致误导性的性能分数。OpenAI 的文章表明，随着模型能力的提升，它们也可以帮助检测这些缺陷，从而实现更可靠的评估。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/separating-signal-from-noise-coding-evaluations/">Separating signal from noise in coding evaluations | OpenAI</a></li>

</ul>
</details>

**社区讨论**: 社区评论提出了对基准操纵、效率指标和任务模糊性的担忧。有用户建议用 100 美元 API 花费来衡量性价比的新基准；另一用户指出任务数量少于 800，人工审查可行，批评原始作者未检查。还有人认为误导性提示无意中测试了模型处理噪声的能力，这本身可以成为一个基准。

**标签**: `#AI`, `#Benchmarks`, `#Coding Evaluations`, `#OpenAI`, `#Software Engineering`

---

<a id="item-7"></a>
## [Mistral 推出 Robostral Navigate，实现无地图机器人导航](https://mistral.ai/news/robostral-navigate/) ⭐️ 8.0/10

Mistral AI 发布了 Robostral Navigate，这是一个 80 亿参数的模型，让机器人仅凭单个 RGB 摄像头即可在复杂室内环境中导航，无需预先构建地图。该模型能理解自然语言指令，例如“离开大厅，进入储藏室”。 这一进展大幅简化了机器人在动态或非结构化环境中的部署，省去了昂贵的地图构建基础设施。它为爱好者和商业机器人应用打开了可能性，可能加速在仓库、家庭和农场的采用。 Robostral Navigate 与硬件无关，可适配任何机器人平台，但当前似乎仅为研究演示，并未公开提供模型。该系统采用基于视觉的方法，类似于斯坦福大学的 PIGEON 等项目，但专注于室内环境。

hackernews · ottomengis · Jul 8, 14:09 · [社区讨论](https://news.ycombinator.com/item?id=48832212)

**背景**: 传统机器人导航通常需要预先构建的地图（如 SLAM）或外部信标，当机器人被“绑架”（即移动到未知位置且无法定位）时就会失败。相比之下，无地图导航允许机器人通过原始摄像头输入理解周围环境，并在不了解空间的情况下执行指令。这种方法已在户外得到验证，但由于视觉歧义性，在室内仍然具有挑战性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mistral.ai/news/robostral-navigate/">Robostral Navigate: single-camera AI navigation | Mistral AI</a></li>
<li><a href="https://news.ycombinator.com/item?id=48832212">Mistral's Robostral Navigate: a state of the art robotics navigation model</a></li>
<li><a href="https://www.reddit.com/r/AIGuild/comments/1ur9vyz/mistral_launched_robostral_navigate_an_8b_model/">Mistral launched Robostral Navigate, an 8B model for robot navigation</a></li>

</ul>
</details>

**社区讨论**: 社区对无地图能力感到兴奋，认为它解决了“绑架机器人”问题。评论者表达了将其用于业余爱好者项目的兴趣，但遗憾该模型未公开可用。有人将其与斯坦福大学的 PIGEON 相提并论，并讨论了此类技术潜在的隐私问题。

**标签**: `#robotics`, `#navigation`, `#Mistral AI`, `#AI`, `#map-less navigation`

---

<a id="item-8"></a>
## [微软发布 Flint，面向 AI 代理的可视化语言](https://microsoft.github.io/flint-chart/#/) ⭐️ 8.0/10

微软发布了 Flint，这是一个开源的视觉化中间语言，旨在提高 AI 代理生成图表的可靠性和质量。Flint 引入了基于语义类型的规范和一个布局优化引擎，可以从简单的高层次输入生成高质量的图表。 Flint 解决了 AI 生成可视化中可靠性与质量之间的基本权衡，使代理能够更一致地生成可发表级别的图表。这可能加速 AI 代理在数据分析和报告中的采用，通过引入确定性层来提高输出的可靠性。 Flint 已经用于微软的 Data Formulator 项目，并作为开源的 MCP（模型上下文协议）服务器提供，可以插入到代理应用程序中。该语言抽象了诸如比例尺、坐标轴和布局等低级视觉决策，将这些决策委托给基于编译器的优化引擎。

hackernews · chenglong-hn · Jul 8, 17:46 · [社区讨论](https://news.ycombinator.com/item?id=48834924)

**背景**: 当前的可视化语言迫使 AI 代理要么使用简单但质量低的规范，要么使用复杂且冗长的规范，这损害了可靠性。Flint 充当类似于编译器 IR 的中间表示，允许代理表达高层次意图，而由引擎处理视觉细节。这种将 LLM 生成与确定性编译器层结合的模式正在成为代理系统中的最佳实践。

**社区讨论**: 评论者指出 Flint 遵循了一种将 LLM 与确定性编译器层结合的新兴模式。有人质疑 Flint 与知名可视化 DSL Vega 有何不同，而另一些人则对 LLM 需要更简单规范的说法表示怀疑，认为 LLM 处理冗长代码没问题，但难以处理空间组成。总体而言，讨论内容充实，既有赞赏也有技术批评。

**标签**: `#visualization`, `#AI agents`, `#Microsoft`, `#data visualization`, `#programming languages`

---

<a id="item-9"></a>
## [xAI 发布 Grok 4.5：低成本高效能但饱受争议](https://x.ai/news/grok-4-5) ⭐️ 8.0/10

xAI 宣布发布 Grok 4.5，这是一款大型语言模型，能以显著低于 GPT-4.5 和 Opus 4.8 等竞品的成本提供有竞争力的性能，定价为每百万输入 tokens $2，每百万输出 tokens $6。 Grok 4.5 的发布可能加剧 AI 模型市场的价格竞争，使更多企业和开发者能够负担得起先进 AI。然而，该模型因被指存在政治偏见和伦理问题而面临严重的信任危机，这可能限制其在企业环境中的采用。 根据社区基准测试，Grok 4.5 的性能大致相当于 Opus 4.7，同时推理效率提高 4 倍。该模型使用了数万亿 tokens 的 Cursor 数据进行训练，捕捉了真实世界的开发者交互和软件工作流程。

hackernews · BoumTAC · Jul 8, 18:00 · [社区讨论](https://news.ycombinator.com/item?id=48835111)

**背景**: Grok 是 xAI（由埃隆·马斯克创立的公司）开发的一系列大型语言模型。Grok 4.5 是最新版本，定位为 OpenAI、Anthropic 等公司模型的高性价比替代品。xAI 因其内容审核和政治中立性问题受到批评，从而引发了对该模型可靠性的质疑。

**社区讨论**: 评论者对 xAI 表达了强烈的不信任，担心其存在政治偏见和伦理问题，尤其是关于 CSAM 的处理。一些人称赞该模型的成本效益和基准性能，将其与竞品进行了有利比较。另一些人则质疑在目前市场盈利困难的背景下，训练如此昂贵的模型是否具有经济可行性。

**标签**: `#AI`, `#machine learning`, `#Grok`, `#xAI`, `#model release`

---

<a id="item-10"></a>
## [OpenAI 推出 GPT-Live 语音模式，可委托 GPT-5.5 推理](https://openai.com/index/introducing-gpt-live/) ⭐️ 8.0/10

OpenAI 发布了 GPT-Live，一种实时语音模式，可在后台将复杂推理任务委托给 GPT-5.5，相比以往的语音模型大幅提升了响应质量。 这一整合将自然语音交互与前沿推理能力结合，使 AI 对话更加实用和逼真，可能提高语音 AI 的采用率，同时也引发了关于替代人际互动的讨论。 初始版本名为 GPT-Live-1。有用户报告称模型会在无意时打断并发笑，且目前该功能缺乏工具或连接器集成，限制了其在生产力场景中的应用。

hackernews · logickkk1 · Jul 8, 17:03 · [社区讨论](https://news.ycombinator.com/item?id=48834405)

**背景**: 此前，由于实时语音的延迟限制，AI 语音模式只能使用较老、能力较弱的模型。GPT-Live 通过将繁重推理委托给 GPT-5.5，同时保持低延迟语音流，实现了更复杂的对话。

**社区讨论**: 社区反应不一：一些用户称赞其质量和自然性（simonw 报告了一小时的富有成效的散步对话），而另一些用户则对替代人际关系表示伦理担忧（jonstaab, overgard）。一个常见的需求是工具集成（artdigital），OpenAI 员工（athyuttamre）澄清版本为 GPT-Live-1。

**标签**: `#OpenAI`, `#voice mode`, `#AI product launch`, `#ethical concerns`, `#GPT-5`

---

<a id="item-11"></a>
## [sqlite-utils 4.0 发布，支持数据库模式迁移](https://simonwillison.net/2026/Jul/7/sqlite-utils/#atom-everything) ⭐️ 8.0/10

sqlite-utils 4.0 已发布，首次引入数据库模式迁移功能。 这一新特性使 sqlite-utils 成为更完整的 SQLite 数据库管理工具，允许用户以编程方式演化数据库模式。 迁移系统可能允许对数据库模式进行增量更改，类似于其他迁移框架。

rss · Simon Willison · Jul 7, 15:42

**背景**: sqlite-utils 是一个用于创建和操作 SQLite 数据库的 Python 库和命令行工具，常用于数据分析和 ETL 工作流。模式迁移的加入填补了其功能集的一个长期空白。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sqlite-utils.datasette.io/">sqlite-utils</a></li>
<li><a href="https://github.com/simonw/sqlite-utils">simonw/sqlite-utils: Python CLI utility and library for ... - GitHub</a></li>

</ul>
</details>

**标签**: `#sqlite`, `#python`, `#database`, `#migrations`

---

<a id="item-12"></a>
## [华为 5G 旗舰重返海外，峰值速率超 1100Mbps](https://finance.sina.com.cn/tech/roll/2026-07-08/doc-inihapna8035781.shtml) ⭐️ 8.0/10

华为 Pura 90 Pro Max 国际版实测峰值 5G 下载速率超过 1100 Mbps，标志着华为 5G 旗舰手机在美国制裁七年后正式重返海外市场。 这一里程碑表明华为有能力克服技术限制并重新进入全球 5G 智能手机市场，可能加剧高端市场竞争并影响供应链格局。 国际版原生支持 5G，状态栏显示 5G 标识，实测峰值下载速率超过 1100 Mbps。今年早些时候，华为旗舰设备升级至 HarmonyOS 6.0.0.125，实装了 5A 通信技术，为此次国际上市奠定了基础。

telegram · zaihuapd · Jul 8, 12:17

**背景**: 自 2019 年以来，美国制裁禁止华为在全球销售 5G 智能手机。2023 年，Mate 60 系列突破了部分技术限制，而 HarmonyOS 6.0.0.125 更新引入了 5A 通信技术。Pura 90 Pro Max 现在将 5G 能力带到国际市场，标志着重大的转折。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://betawiki.net/wiki/HarmonyOS_6">HarmonyOS 6 - BetaWiki</a></li>
<li><a href="https://www.reddit.com/r/Huawei/comments/1q8v34v/celia_keyboard_hits_the_primetime_letsgoooo_hos/">Celia Keyboard Hits the Prime-Time, Letsgoooo! (HOS 6.0.0.125) - Reddit</a></li>

</ul>
</details>

**标签**: `#Huawei`, `#5G`, `#smartphones`, `#telecommunications`, `#sanctions`

---

<a id="item-13"></a>
## [Cloudflare 与 OpenAI 合作试点全球网络数据优化 AI 搜索](https://36kr.com/newsflashes/3886946347694593) ⭐️ 8.0/10

7 月 8 日，Cloudflare 与 OpenAI 宣布启动一项研究试点项目，利用 Cloudflare 全球网络的实时网站洞察数据，帮助 AI 搜索引擎更高效地发现和索引开放网络上的内容。 此次合作通过引入内容新鲜度、流量质量等实时网络信号，有望显著提升 AI 回答的准确性和时效性，为 AI 搜索索引树立新标准。 该试点项目利用 Cloudflare 对实际页面变动和流量模式的可见性来优化抓取效率，但目前仍处于实验阶段，尚未宣布生产部署。

telegram · zaihuapd · Jul 8, 15:27

**背景**: AI 搜索引擎依赖网络爬虫来索引内容，但传统爬虫可能效率低下且错过更新。Cloudflare 的全球网络处理了很大一部分网络流量，能够提供关于网站变化和流行度的独特实时数据。这些数据可以帮助 AI 系统优先抓取新鲜、高质量的页面。

**标签**: `#Cloudflare`, `#OpenAI`, `#AI Search`, `#Web Indexing`, `#Data Optimization`

---

<a id="item-14"></a>
## [通过电磁信号识别手机应用，准确率达 99.07%](https://www.scmp.com/news/china/science/article/3359688/chinese-researchers-find-peephole-any-smartphone-its-leaked-radio-signal) ⭐️ 8.0/10

研究人员开发出一种非接触式技术，通过分析智能手机泄漏的低频电磁信号，以高达 99.07%的准确率识别正在运行的应用及操作。该方法即使在设备离线、飞行模式、加密或锁定状态下也能工作。 这种侧信道攻击带来了重大的隐私和安全风险，因为它能在无需直接访问设备的情况下推断出应用使用模式。这凸显了电磁辐射作为信息泄露途径的脆弱性。 测试在 iPhone 15 Pro、小米 15 Pro 和 OPPO Reno 13 上进行，涵盖抖音、微信视频通话、百度地图、短信、浏览器、相机和云存储等应用。最高准确率达到 99.07%。

telegram · zaihuapd · Jul 8, 16:05

**背景**: 智能手机在运行时会因内部电路活动而产生低频电磁信号。这些信号通常是意外的副产品，但可以通过专业设备远程捕获并分析，从而推断用户活动。这类技术被称为侧信道攻击，利用物理辐射来提取本应由软件安全措施保护的信息。

**标签**: `#security`, `#side-channel`, `#smartphone`, `#privacy`, `#forensics`

---