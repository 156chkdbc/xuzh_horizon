---
layout: default
title: "Horizon Summary: 2026-07-15 (ZH)"
date: 2026-07-15
lang: zh
---

> From 33 items, 15 important content pieces were selected

---

1. [2026 年菲尔兹奖得主通过 ICM 官网代码泄露](#item-1) ⭐️ 9.0/10
2. [高德发布世界模型工坊，内置时空任意门](#item-2) ⭐️ 9.0/10
3. [Bonsai 27B：首个能在手机上运行的 270 亿参数模型](#item-3) ⭐️ 8.0/10
4. [文章警告 AI 代理削弱软件组合性](#item-4) ⭐️ 8.0/10
5. [Cursor 零日漏洞引发全面披露](#item-5) ⭐️ 8.0/10
6. [我们是否过度将思考外包给 AI？](#item-6) ⭐️ 8.0/10
7. [Lobste.rs 从 MariaDB 迁移到 SQLite，降低成本](#item-7) ⭐️ 8.0/10
8. [Armin Ronacher：AI 代理可能侵蚀软件项目的共同理解](#item-8) ⭐️ 8.0/10
9. [Cloudflare 推出 Precursor：持续行为验证检测 AI 机器人](#item-9) ⭐️ 8.0/10
10. [DeepSeek 完成超 500 亿元首轮融资，采用特殊架构维持创始人控制](#item-10) ⭐️ 8.0/10
11. [Telegram 短域名 t.me 被注册局冻结](#item-11) ⭐️ 8.0/10
12. [DeepMind CEO 呼吁美国主导全球 AI 监管机构](#item-12) ⭐️ 8.0/10
13. [DeepSeek 寻求 710 亿美元估值新一轮融资，自研 AI 芯片](#item-13) ⭐️ 8.0/10
14. [白宫将召集电力公司讨论 AI 用电成本](#item-14) ⭐️ 8.0/10
15. [美国批准英伟达 H200 对约 10 家中国企业销售](#item-15) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [2026 年菲尔兹奖得主通过 ICM 官网代码泄露](https://www.reddit.com/r/math/comments/1urv4id/fields_medal_26_predictionsdiscussion/) ⭐️ 9.0/10

国际数学家大会（ICM）官网前端代码中隐藏的一份日程可能泄露了 2026 年菲尔兹奖得主：邓宇、John Pardon、Jacob Tsimerman 和王虹。 如果泄露属实，这将抢先披露数学界最高荣誉之一，加剧对 ICM 安全性的审视，并凸显学界对评选结果的强烈关注。 有用户通过抓取 ICM 网站代码发现了标记为“HIDDEN”的名字；Polymarket 上对此结果的预测概率已达到 95%。

telegram · zaihuapd · Jul 14, 05:51

**背景**: 菲尔兹奖每四年颁发一次，表彰 40 岁以下数学家的杰出成就。王虹因解决三维 Kakeya 猜想（调和分析中的一个重大问题）而备受瞩目。Polymarket 是一个基于加密货币的预测市场，用户可对各类未来事件下注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kakeya_conjecture">Kakeya conjecture</a></li>
<li><a href="https://arxiv.org/abs/2512.09842">The Kakeya Conjecture: where does it come from and why is it important?</a></li>
<li><a href="https://en.wikipedia.org/wiki/Polymarket">Polymarket</a></li>

</ul>
</details>

**标签**: `#Fields Medal`, `#mathematics`, `#leak`, `#ICM`, `#academia`

---

<a id="item-2"></a>
## [高德发布世界模型工坊，内置时空任意门](https://www.ithome.com/0/976/538.htm) ⭐️ 9.0/10

高德（阿里巴巴）发布了通用世界模型工坊 ABot-WorldStudio，用户输入文字或图片即可生成可实时交互的 3D 世界，并内置“时空任意门”功能，可在不同世界间穿梭。底层 ABot-World 系列模型已全面开源。 该发布意义重大，因为实现了无上限推理时长且质量不衰减，远超同类产品约 1 分钟的限制。它将交互式视频生成与 3DGS 场景输出统一，对具身智能仿真、游戏开发和虚拟制作等领域具有深远影响。 ABot-WorldStudio 可在单张 RTX 5090 上本地部署，官方实测连续推理超 1 小时无崩溃、无质量衰减。它原生输出的 3DGS 资产具备真实几何结构与照片级视觉保真度。

telegram · zaihuapd · Jul 14, 12:22

**背景**: AI 中的世界模型是一种学习环境内部表示以模拟动态并预测结果的系统。3D 高斯泼溅（3DGS）是一种光栅化技术，可从稀疏的 2D 图像实时渲染照片级 3D 场景，于 2023 年重新兴起。具身 AI 将 AI 集成到物理系统中以与现实世界互动，如机器人和自动驾驶。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/3D_Gaussian_splatting">3D Gaussian splatting</a></li>
<li><a href="https://en.wikipedia.org/wiki/World_model_(artificial_intelligence)">World model (artificial intelligence)</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/embodied-ai/">Embodied AI: What Is It and How to Build It?</a></li>

</ul>
</details>

**标签**: `#world model`, `#3DGS`, `#AI generation`, `#open source`, `#embodied AI`

---

<a id="item-3"></a>
## [Bonsai 27B：首个能在手机上运行的 270 亿参数模型](https://prismml.com/news/bonsai-27b) ⭐️ 8.0/10

PrismML 发布了 Bonsai 27B，这是一个基于 Qwen3.6 27B 的 270 亿参数多模态模型，通过量化到 1 比特或三值权重，使得模型体积缩减至 4GB，从而能够在手机上运行。 1 比特版本实现了手机端推理，这标志着首个 270 亿参数级别模型可部署于移动设备。 这一极端量化突破表明，大型语言模型可以在消费级硬件上本地运行，从而实现无需依赖云的隐私保护 AI。它挑战了“低于 4 比特量化会严重降低性能”的假设，因为 Bonsai 27B 保留了高达 94.6% 的 FP16 精度。 Bonsai 27B 在所有语言组件上使用 1 比特和三值权重，并配有单独的 4 比特视觉塔。三值版本占用 5.9GB，在基准测试中保留了 FP16 性能的 94.6%；1 比特版本占用 3.9GB，保留了 89.5%。

hackernews · xenova · Jul 14, 17:50 · [社区讨论](https://news.ycombinator.com/item?id=48910545)

**背景**: 量化通过降低神经网络权重的精度（例如从 16 位浮点数降至 1 位二进制）来缩小模型体积并加速推理，从而能够在内存有限的设备（如智能手机）上部署。传统的低于 4 比特量化往往会导致显著的精度损失，但 PrismML 采用的新技术旨在最小化精度下降的同时实现极端压缩。设备端 AI 消除了基于云模型的延迟和隐私问题，使得无需联网即可使用强大的 AI。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://prismml.com/news/bonsai-27b">PrismML — Announcing Bonsai 27B: The First 27B-Class Model to ...</a></li>
<li><a href="https://www.marktechpost.com/2026/07/14/prismml-releases-bonsai-27b-1-bit-and-ternary-builds-of-qwen3-6-27b-that-run-on-laptops-and-phones/">PrismML Releases Bonsai 27B: 1-bit and Ternary Builds of ...</a></li>
<li><a href="https://docs.prismml.com/models/bonsai-27b">Bonsai 27B - Bonsai - docs.prismml.com</a></li>

</ul>
</details>

**社区讨论**: 评论者将 Bonsai 27B 与 Gemma 4 12B QAT 进行比较，质疑在极低比特宽度下会损失多少智能。一些用户报告称在 LM Studio 中运行模型时遇到困难，而另一些用户则对模型的实际表现表示怀疑（例如，一个食谱演示中营养计算错误）。

**标签**: `#AI`, `#quantization`, `#on-device AI`, `#model compression`, `#machine learning`

---

<a id="item-4"></a>
## [文章警告 AI 代理削弱软件组合性](https://lucumr.pocoo.org/2026/7/13/the-tower-keeps-rising/) ⭐️ 8.0/10

Armin Ronacher 的文章《不断升高的塔楼》警告，过度依赖 AI 编码代理会削弱软件的组合性和架构控制，这与 Lisp 诅咒的现象类似。 随着 AI 编码工具的普及，开发者可能失去构建可维护、可组合系统的能力，从而威胁长期软件质量和团队协作。 文章将当前趋势与 Lisp 诅咒相类比，后者指出语言的强大功能导致开发者孤立工作、库碎片化。Ronacher 认为 AI 代理放大了这一效应，让个人编码更快但架构一致性更低。

hackernews · cdrnsf · Jul 14, 16:57 · [社区讨论](https://news.ycombinator.com/item?id=48909785)

**背景**: Lisp 诅咒描述的是 Lisp 的强大功能让开发者能轻易独自构建定制方案，从而减少协作，导致生态系统更贫瘠。AI 编码代理是能自动编写、修改和调试多文件代码的软件工具，但通常缺乏深入的架构理解。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.freshcodeit.com/blog/myths-of-lisp-curse">What is the Curse of Lisp: Challenges and Opportunities</a></li>
<li><a href="https://agentic.ai/best/coding-agents">20 Best AI Coding Agents in 2026 — Agentic.ai</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，天真地使用代理会破坏组合性，类似于玩不好俄罗斯方块。有人建议手动修复小问题以保持架构控制，另有人将这种情况类比为双极性 Lisp 程序员现象。

**标签**: `#software engineering`, `#AI agents`, `#composability`, `#programming philosophy`

---

<a id="item-5"></a>
## [Cursor 零日漏洞引发全面披露](https://mindgard.ai/blog/cursor-0day-when-full-disclosure-becomes-the-only-protection-left) ⭐️ 8.0/10

一名研究人员披露了 AI 代码编辑器 Cursor 中存在一个长达一年未修复的漏洞，该漏洞允许在没有用户确认的情况下运行任意可执行文件。此前多次向供应商报告，但超过半年未得到解决。 此漏洞突显了隐式执行代码的 AI 编码工具中的安全风险，并在供应商不作为的情况下重新引发了关于负责任披露与全面披露的争论。Cursor 用户可能因工作区中的恶意文件而面临风险。 该漏洞利用了 Windows 的一个特性：搜索可执行文件时优先查找当前目录而非系统 PATH；攻击者只需将恶意 git.exe 放入项目文件夹。Cursor 随后会在没有任何用户提示的情况下执行它，这不同于通常的 ACL 行为。

hackernews · Synthetic7346 · Jul 14, 17:58 · [社区讨论](https://news.ycombinator.com/item?id=48910676)

**背景**: 零日漏洞是指供应商未知且尚无补丁的安全缺陷，使用户面临潜在攻击。全面披露是研究人员在供应商未能及时修复漏洞时公开发布详细信息的一种做法。Cursor 是从 Visual Studio Code 分支出来的 AI 代码编辑器，因其智能编码辅助而广泛使用。此处报告的漏洞涉及 Cursor 与 Git 的集成，它在调用系统 PATH 之前优先在当前工作目录中搜索 git.exe。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zero-day_vulnerability">Zero-day vulnerability - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)">Full disclosure (computer security) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cursor_(code_editor)">Cursor (code editor)</a></li>

</ul>
</details>

**社区讨论**: 评论者意见不一：有人认为该漏洞影响不大，因为攻击者需要事先放置恶意可执行文件；而另一些人则强调缺少用户提示是危险的。普遍认为 Cursor 供应商的回应不足，尽管问题持续数月，最初仍将报告标记为“信息性”并关闭。

**标签**: `#security`, `#vulnerability`, `#cursor`, `#disclosure`, `#code-editor`

---

<a id="item-6"></a>
## [我们是否过度将思考外包给 AI？](https://www.artfish.ai/p/offloading-thinking-to-ai) ⭐️ 8.0/10

ArtFish 上一篇高分文章引发了关于过度依赖 AI 进行认知任务是否有害的辩论，获得了 384 个点赞和 387 条评论，吸引了技术社区的积极参与。 随着 LLM 等 AI 工具在知识工作中普及，这场辩论凸显了削弱批判性思维和深度理解的风险，可能影响生产力和创新。 讨论中包含真实案例，例如一名初级开发人员无法解释 AI 生成的计算过程，以及评论者认为深层技术理解对于有效使用 AI 仍然有价值。

hackernews · yenniejun111 · Jul 14, 15:18 · [社区讨论](https://news.ycombinator.com/item?id=48908178)

**背景**: 认知外包是指使用外部工具减少脑力劳动的做法，从计算器到 GPS 都是如此。随着 LLM 等先进 AI 的出现，这种做法已扩展到推理和决策，引发了技能退化和依赖性的担忧。

**社区讨论**: 社区评论普遍对过度依赖持批评态度，用户分享了初级人员缺乏基本理解的轶事，并担心 AI 使用正在取代真正的学习。尽管有人为 AI 作为生产力工具辩护，但主流情绪是谨慎的。

**标签**: `#AI ethics`, `#critical thinking`, `#software engineering`, `#knowledge work`, `#AI dependence`

---

<a id="item-7"></a>
## [Lobste.rs 从 MariaDB 迁移到 SQLite，降低成本](https://simonwillison.net/2026/Jul/14/lobsters-sqlite/#atom-everything) ⭐️ 8.0/10

社区新闻网站 Lobsters 在上周末完成了从 MariaDB 到 SQLite 的迁移，实现了更低的 CPU 和内存使用率，网站响应更快，并且 VPS 成本减半。 这次实际迁移为在生产 Web 应用中使用 SQLite 提供了令人信服的案例研究，展示了显著的性能提升和成本节约，并挑战了中等流量站点默认选择客户端-服务器数据库的做法。 Lobsters 的 Rails 应用现在运行在一个单一的 VPS 上，主 SQLite 数据库约 3.8GB，另有独立的缓存（1.1GB）、队列（218MB）和 rack_attack（555MB）数据库。迁移 PR 在 30 个提交中增加了 735 行并删除了 593 行。

rss · Simon Willison · Jul 14, 19:44

**背景**: SQLite 是一种轻量级嵌入式关系数据库引擎，将数据存储在单个文件中，不像 MariaDB 这样的客户端-服务器数据库需要独立的服务器进程。它广泛应用于移动和桌面应用，但在 Web 应用中较少见。MariaDB 是从 MySQL 分支出来的流行开源关系数据库。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/SQLite">SQLite</a></li>
<li><a href="https://en.wikipedia.org/wiki/MariaDB">MariaDB</a></li>

</ul>
</details>

**社区讨论**: Lobsters 的讨论线程报告了积极的结果，原发帖人指出 CPU 和内存使用率下降，网站更灵敏，并计划通过移除 MariaDB VPS 将成本减半。还分享了关于数据库大小和架构的更多细节。

**标签**: `#SQLite`, `#Rails`, `#database migration`, `#performance`, `#web development`

---

<a id="item-8"></a>
## [Armin Ronacher：AI 代理可能侵蚀软件项目的共同理解](https://simonwillison.net/2026/Jul/14/armin-ronacher/#atom-everything) ⭐️ 8.0/10

Armin Ronacher 发表了一篇文章，指出软件项目的共同语言——对概念、边界、不变量和归属的共同理解——是通过代码审查和跨团队协调等过程中的摩擦来维系的，而 AI 代理可能会破坏这种同步。 这一观点意义重大，因为它揭示了 AI 辅助编程中一个微妙且常被忽视的代价：虽然代理提高了个人生产力，但它们可能会减少跨团队的意识和共同的心理模型，而这些正是大型项目保持连贯性的关键。它挑战了“代码生成越快越好”的假设。 Ronacher 的核心论断是“摩擦使人同步”——阅读他人代码、提问和协调过程中的刻意缓慢并非全是浪费；它是理解传播和共识保持的方式。跳过这些步骤的 AI 代理有可能使团队共享知识碎片化。

rss · Simon Willison · Jul 14, 18:04

**背景**: 在大型软件项目中，团队的共同理解通常是隐式的，嵌入在代码审查、讨论以及解释变更的经验中。这种“共同语言”超越了编程语言和文档。摩擦——例如修改另一个团队拥有的组件所需的工作量——迫使开发者进行沟通和协调，确保系统连贯地演进。AI 代理独立生成和修改代码可能会绕过这种摩擦，从而可能破坏集体理解。

**标签**: `#software engineering`, `#shared understanding`, `#AI agents`, `#code review`, `#software design`

---

<a id="item-9"></a>
## [Cloudflare 推出 Precursor：持续行为验证检测 AI 机器人](https://blog.cloudflare.com/introducing-precursor/) ⭐️ 8.0/10

Cloudflare 发布了 Precursor，这是一个客户端、基于会话的验证引擎，通过持续监控鼠标移动、键盘节奏和滚动等行为信号来区分人类与 AI 机器人。 Precursor 将机器人检测从单点挑战转变为持续验证，使得自动化代理更难逃避检测，同时提供无摩擦的用户体验。这可能成为易受 AI 驱动爬取和欺诈攻击的网站的新网络安全标准。 Precursor 使用动态注入的 JavaScript 在整个浏览会话中收集信号，并将其整合到基于会话的分析面板中。该功能面向企业版 Bot Management 客户提供免费测试，正式版计划今年晚些时候上线。

telegram · zaihuapd · Jul 14, 09:44

**背景**: 传统的验证码甚至 Cloudflare 的 Turnstile 仅在登录或结账等特定入口点对用户进行验证。Precursor 通过分析人类特有的微行为——例如自然的鼠标弧线轨迹和认知停顿——将验证扩展到整个会话，这些行为 AI 难以准确模仿。这种方法是对 Turnstile 的补充，覆盖了初始挑战之外的用户旅程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.cloudflare.com/introducing-precursor/">Introducing Precursor: detecting agentic behavior with continuous client-side signals</a></li>
<li><a href="https://developers.cloudflare.com/cloudflare-challenges/precursor/">Precursor · Cloudflare challenges docs</a></li>
<li><a href="https://tech.slashdot.org/story/26/07/13/1645252/cloudflare-precursor-watches-your-mouse-and-keyboard-to-decide-if-you-are-human">Cloudflare Precursor Watches Your Mouse and Keyboard To Decide If You Are Human - Slashdot</a></li>

</ul>
</details>

**标签**: `#Cloudflare`, `#反机器人`, `#行为验证`, `#网络安全`, `#AI检测`

---

<a id="item-10"></a>
## [DeepSeek 完成超 500 亿元首轮融资，采用特殊架构维持创始人控制](https://t.me/zaihuapd/42557) ⭐️ 8.0/10

DeepSeek 完成逾 500 亿元人民币（约 74 亿美元）的首轮融资，估值超过 500 亿美元。此次融资采用非常规的有限合伙架构，投资者需将资金注入创始人梁文锋管理的有限合伙企业，并接受五年锁定期且不享有表决权。 这笔巨额融资凸显了 DeepSeek 作为 AI 领军企业的迅速崛起，并展示了一种治理创新——即使获得大规模外部投资，创始人仍能保持控制权。这可能为其他寻求在资本注入与创始人自主权之间取得平衡的高增长科技初创公司树立先例。 创始人梁文锋在本轮融资中个人投资 200 亿元。腾讯和宁德时代分别考虑投资 100 亿元和 50 亿元，可能成为最大的外部投资者。该架构要求投资者接受五年锁定期且不享有表决权。

telegram · zaihuapd · Jul 14, 11:06

**背景**: 在有限合伙架构中，普通合伙人（GP）负责管理基金并做出决策，而有限合伙人（LP）提供资金但不参与管理。这使得创始人可以在不稀释投票权的情况下融资。通过将投资注入创始人控制的有限合伙企业，DeepSeek 确保梁文锋尽管筹集了巨额资金，仍能保留决策权。这种结构在风险投资中常见，但对于直接的初创企业融资轮次而言相对新颖。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.sohu.com/a/968465639_122554521">有限合伙架构：长期主义企业的控制权护航利器_股权_杰诚_公司</a></li>
<li><a href="https://k.sina.cn/article_7879922977_1d5ae152106801fx3y.html">DeepSeek创始人梁文锋具体采用了何种交易结构来保持控制权？|合伙企业...</a></li>

</ul>
</details>

**标签**: `#AI`, `#Funding`, `#DeepSeek`, `#Governance`, `#Startup`

---

<a id="item-11"></a>
## [Telegram 短域名 t.me 被注册局冻结](https://t.me/zaihuapd/42559) ⭐️ 8.0/10

Telegram 的短链接域名 t.me 自 2025 年 7 月 13 日起被注册局设置为 serverHold 状态，导致 DNS 解析暂停，可能影响短链接服务。该域名通过 GoDaddy 注册，有效期至 2035 年，现被附加 serverHold 及禁止删除、转移、续费、更新等多项 EPP 状态码。 此事影响全球数百万依赖 t.me 链接分享频道、群组和机器人访问的 Telegram 用户。Telegram 及注册局均未给出官方解释，增加了不确定性，也暴露了大型平台基于域名的基础设施的脆弱性。 ServerHold 状态是注册局级别的暂停，会将该域名从区域文件中移除，阻止 DNS 解析。同时还附加了 clientDeleteProhibited、clientTransferProhibited 等状态码，进一步限制域名管理。冻结的确切原因尚不清楚；可能包括法律行动、滥用举报或监管合规问题。

telegram · zaihuapd · Jul 14, 12:48

**背景**: 域名由注册局（管理顶级域数据库）和注册商（向最终用户销售域名）共同管理。ServerHold 状态由注册局设置，通常出于法律或滥用原因，比注册商设置的 clientHold 更严重。Telegram 的 t.me 域名作为其平台的 URL 缩短器，允许用户分享类似 t.me/username 的链接。此次冻结可能导致现有短链接失效，并阻止新的短链接解析。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.namecheap.com/support/knowledgebase/article.aspx/10717/46/why-was-my-domain-suspended-with-a-serverhold-or-clienthold-status/">Why was my domain suspended with a serverHold or clientHold ...</a></li>
<li><a href="https://www.godaddy.com/help/what-is-the-difference-between-a-registry-registrar-and-registrant-8039">What is the difference between a registry, registrar and ...</a></li>
<li><a href="https://www.icann.org/resources/pages/epp-status-codes-2014-06-16-en">EPP Status Codes | What Do They Mean, and Why Should I Know?</a></li>

</ul>
</details>

**标签**: `#telegram`, `#domain`, `#dns`, `#outage`, `#registry`

---

<a id="item-12"></a>
## [DeepMind CEO 呼吁美国主导全球 AI 监管机构](https://www.theverge.com/tech/965270/google-deepmind-demis-hassabis-global-ai-watchdog) ⭐️ 8.0/10

Google DeepMind 首席执行官 Demis Hassabis 呼吁由美国主导成立一个全球 AI 监管机构，在部署前评估前沿 AI 模型，力争在 2025 年底前开始运作。 这一来自 AI 领域领军人物提议可能深刻影响全球 AI 治理格局，有望为部署前的安全评估和风险过高时的行业协同暂停建立先例。 拟议的监管机构将由独立专家和开源社区代表组成，若模型风险过高可要求全行业协同暂停。Hassabis 已与特朗普政府、其他 AI 实验室及欧洲官员进行了讨论。

telegram · zaihuapd · Jul 14, 14:29

**背景**: 前沿 AI 模型是具备高度能力的基础模型，可能拥有足以对公共安全构成严重风险的危险能力。随着这些模型不断进步，人们对其潜在滥用或意外后果的担忧日益加剧，从而引发了在部署前进行主动监管的呼声。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/frontier-ai-regulation/">Frontier AI regulation: Managing emerging risks to public ...</a></li>
<li><a href="https://www.governance.ai/analysis/frontier-ai-regulation">Frontier AI Regulation | GovAI - Governance</a></li>

</ul>
</details>

**标签**: `#AI regulation`, `#DeepMind`, `#Demis Hassabis`, `#global governance`, `#AI safety`

---

<a id="item-13"></a>
## [DeepSeek 寻求 710 亿美元估值新一轮融资，自研 AI 芯片](https://t.me/zaihuapd/42564) ⭐️ 8.0/10

中国 AI 创业公司 DeepSeek 在完成首轮融资仅一个月后，已开始与投资者初步洽谈新一轮融资，投前估值约 710 亿美元，而 5 月底刚以约 520 亿美元估值完成约 70 亿美元融资。此外，据路透社本月早些时候报道，DeepSeek 正在开发自有 AI 芯片，以减少对英伟达和华为芯片的依赖。 估值在一个月内从 520 亿美元飙升至 710 亿美元，凸显了在地缘政治紧张局势下投资者对中国顶级 AI 初创公司的强烈需求。开发自研 AI 芯片表明 DeepSeek 在战略上致力于掌控供应链，以更独立地与美国 AI 巨头竞争。 新一轮融资的投前估值据称为 710 亿美元，而该公司在 2026 年 5 月底刚以 520 亿美元估值完成约 70 亿美元融资。自研芯片仍处于早期阶段，旨在减少对英伟达和华为硬件的依赖。

telegram · zaihuapd · Jul 14, 15:15

**背景**: DeepSeek 是一家中国 AI 初创公司，2025 年初其 AI 助手登顶应用下载榜并导致美国科技股下跌，从而引发全球关注，其模型可与 OpenAI 竞争。此后该公司发布了升级版模型并拓展至非洲市场。自研 AI 芯片是主要 AI 公司的常见战略，旨在优化性能并降低成本，但这需要大量投资和时间。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek - Wikipedia</a></li>
<li><a href="https://www.usnews.com/news/top-news/articles/2026-07-07/exclusive-chinas-deepseek-developing-its-own-ai-chip-sources-say">Exclusive-China's DeepSeek Developing Its Own AI Chip ...</a></li>

</ul>
</details>

**标签**: `#AI`, `#DeepSeek`, `#funding`, `#AI chips`, `#startup`

---

<a id="item-14"></a>
## [白宫将召集电力公司讨论 AI 用电成本](https://t.me/zaihuapd/42566) ⭐️ 8.0/10

白宫计划在未来几周召集电力公司和数据中心开发商，推动一项自愿承诺，确保人工智能带来的电力需求激增不会转嫁给居民和企业用户。 这一举措可能为 AI 基础设施成本的分摊开创先例，在支持 AI 数据中心快速扩张的同时保护消费者免受电价上涨影响。涉及大型科技公司和州长，表明协调政策的趋向。 今年早些时候，Google、Meta 和 OpenAI 等公司已在白宫签署类似承诺，同意自行承担 AI 项目所需的发电和电网升级成本。新一轮活动旨在将电力公司、数据中心运营商以及州长也纳入承诺范围。

telegram · zaihuapd · Jul 14, 16:00

**背景**: AI 数据中心消耗大量电力，给电网带来压力，并引发普通用户电费上涨的担忧。白宫的干预旨在防止成本转嫁，并鼓励可持续的基础设施投资。

**标签**: `#AI`, `#Energy`, `#Policy`, `#Data Centers`, `#US Government`

---

<a id="item-15"></a>
## [美国批准英伟达 H200 对约 10 家中国企业销售](https://t.me/zaihuapd/42567) ⭐️ 8.0/10

美国商务部已批准包括阿里巴巴、腾讯在内的约 10 家中国企业购买英伟达 H200 人工智能芯片，但由于中方指导趋于谨慎，目前尚未有交付完成。 这一决定标志着美国芯片出口管制可能有所放松，有望显著提升英伟达的收入，同时在中美科技竞争加剧背景下，让中国科技巨头获得尖端 AI 硬件。 买家包括阿里巴巴、腾讯、字节跳动和京东，联想、富士康等分销商也获得许可，单一客户最多可购买 7.5 万颗芯片。英伟达 CEO 黄仁勋访华被视为推动交易落地的举措。

telegram · zaihuapd · Jul 15, 00:14

**背景**: H200 Tensor Core GPU 是英伟达的高端 AI 加速器，基于 Hopper 架构，配备 141GB HBM3e 显存和 4.8 TB/s 带宽，大型语言模型推理性能比 H100 最高提升 45%。此前限制阻碍了中国获取先进 AI 芯片，刺激了国产替代品的发展。此次批准正值美中贸易紧张局势持续以及中国推动 AI 自主之际。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/data-center/h200/">H200 GPU | NVIDIA</a></li>
<li><a href="https://www.cnbc.com/2026/07/14/nvidia-h200-ai-chips-china.html">Commerce official says Nvidia H200 AI chips have been shipped ...</a></li>
<li><a href="https://introl.com/blog/h100-vs-h200-vs-b200-choosing-the-right-nvidia-gpus-for-your-ai-workload">H100 vs H200 vs B200: NVIDIA GPU Comparison | Introl Blog</a></li>

</ul>
</details>

**标签**: `#AI hardware`, `#US-China trade`, `#H200`, `#Nvidia`, `#semiconductor`

---