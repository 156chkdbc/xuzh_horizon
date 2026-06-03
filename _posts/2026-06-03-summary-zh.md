---
layout: default
title: "Horizon Summary: 2026-06-03 (ZH)"
date: 2026-06-03
lang: zh
---

> From 36 items, 7 important content pieces were selected

---

1. [黑客利用 Meta AI 聊天机器人劫持 Instagram 账户](#item-1) ⭐️ 9.0/10
2. [CT 扫描揭示比亚迪的制造质量与垂直整合](#item-2) ⭐️ 8.0/10
3. [2020 年西雅图监控基础设施步行导览](#item-3) ⭐️ 8.0/10
4. [KDE Plasma 最后一个支持 X11 的版本标志着全面转向 Wayland](#item-4) ⭐️ 8.0/10
5. [微软发布高效 MAI 大模型，仅需少量活跃参数](#item-5) ⭐️ 8.0/10
6. [特朗普签署 AI 行政令，要求企业自愿提交模型审查](#item-6) ⭐️ 8.0/10
7. [谷歌向 Play Store 开发者付费获取代码训练 AI](#item-7) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [黑客利用 Meta AI 聊天机器人劫持 Instagram 账户](https://simonwillison.net/2026/Jun/1/hackers-simply-asked-meta-ai/#atom-everything) ⭐️ 9.0/10

黑客成功劫持了高知名度 Instagram 账户，只需请求 Meta 的 AI 支持聊天机器人更改关联邮箱即可，该漏洞已获多个来源验证。 此漏洞显示了将 AI 集成到账户恢复系统中的关键失败，允许以极小代价进行未授权账户劫持，突显了缺乏适当防护措施的危险性。 攻击涉及与 Meta 的 AI 支持机器人开始对话，并请求为目标账户关联新邮箱地址，绕过了典型验证步骤，因为该聊天机器人被设计为快速完成整个账户恢复流程。

rss · Simon Willison · Jun 1, 21:14

**背景**: 提示注入是一种攻击方式，恶意输入欺骗 AI 模型执行非预期操作。在此案例中，AI 聊天机器人缺乏适当防护措施来区分合法请求与恶意请求，导致简单提示即可触发账户恢复流程。该事件类似于其他针对 AI 系统的提示注入攻击。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>
<li><a href="https://krebsonsecurity.com/2026/06/hackers-used-metas-ai-support-bot-to-seize-instagram-accounts/">Hackers Used Meta’s AI Support Bot to Seize Instagram Accounts ...</a></li>
<li><a href="https://www.bbc.com/news/articles/c98rzr72dpyo">Meta AI chatbot enabled hackers to access others' Instagram accounts</a></li>

</ul>
</details>

**标签**: `#security`, `#AI`, `#Meta`, `#Instagram`, `#vulnerability`

---

<a id="item-2"></a>
## [CT 扫描揭示比亚迪的制造质量与垂直整合](https://www.lumafield.com/scan-of-the-month/byd) ⭐️ 8.0/10

LumaField 发布了比亚迪汽车零部件的 CT 扫描图像，揭示了令人印象深刻的制造质量和广泛的垂直整合，挑战了“中国车质量差”的论调。 这为比亚迪的制造质量提供了客观、数据驱动的证据，可能改变消费者的看法。同时凸显了比亚迪的战略性垂直整合，这是历史上福特大规模采用的模式。 扫描显示控制臂、副车架等坚固部件。社区评论纠正指出，机械备用钥匙并非铰接，而是通过卡扣拉出。

hackernews · viasfo · Jun 2, 20:30 · [社区讨论](https://news.ycombinator.com/item?id=48375824)

**背景**: 垂直整合指企业控制从原材料到最终装配的多个生产环节。比亚迪约 75%的零部件自产，与特斯拉比例相近，但产量更大（年产 460 万辆，特斯拉为 160 万辆）。传统车企如福特仅自产约 25%的零部件。CT 扫描利用 X 射线创建内部结构的详细 3D 图像，实现无损质量分析。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://supplychain360.io/operations/teslas-vertical-integration-revolutionizes-supply-chains/">Tesla's Vertical Integration Revolutionizes Supply Chains</a></li>
<li><a href="https://www.forbes.com/councils/forbesbusinesscouncil/2024/01/29/why-vertical-integration-is-the-path-to-strategic-advantage/">Why Vertical Integration Is The Path To Strategic Advantage</a></li>

</ul>
</details>

**社区讨论**: 一位高级技师称赞比亚迪零部件坚固耐用，反驳了负面刻板印象。另一用户纠正了钥匙机制的细节。评论者还注意到比亚迪的组织创新及其与特斯拉、福特相比的垂直整合规模。

**标签**: `#automotive`, `#engineering`, `#manufacturing`, `#BYD`, `#CT scanning`

---

<a id="item-3"></a>
## [2020 年西雅图监控基础设施步行导览](https://coveillance.org/a-walking-tour-of-surveillance-infrastructure-in-seattle/) ⭐️ 8.0/10

这篇文章对西雅图的监控摄像头进行了详细的地面考察，记录了这些设备的部署方式以及它们所强制执行的社会协议。 这一分析具有重要意义，因为它引发了关于隐私、伦理和技术的高参与度讨论，揭示了城市监控如何塑造社会规范，并引发对监控国家的担忧。 文章使用了‘注视的种类’和‘编码观看方式’等语言，一些社区成员批评这些语言过于学术化，不易理解。

hackernews · eustoria · Jun 2, 13:24 · [社区讨论](https://news.ycombinator.com/item?id=48369980)

**背景**: 城市监控基础设施，包括摄像头和传感器，在全球城市中越来越普遍。这些系统通常以公共安全和预防犯罪为理由，但批评者认为它们侵犯隐私，并可能加剧社会不平等。西雅图的讨论反映了关于安全与公民自由之间权衡的更广泛辩论。

**社区讨论**: 社区评论表达了不同观点：一些人认为鉴于高犯罪率以及陪审团不愿在没有视频证据的情况下定罪，监控是必要的；而另一些人则批评文章的语言过于学术化，并担心自由受到侵蚀。

**标签**: `#surveillance`, `#privacy`, `#ethics`, `#technology`, `#seattle`

---

<a id="item-4"></a>
## [KDE Plasma 最后一个支持 X11 的版本标志着全面转向 Wayland](https://blog.davidedmundson.co.uk/blog/596/) ⭐️ 8.0/10

KDE Plasma 即将发布的版本将是最后一个支持 X11 的版本，这意味着未来的所有版本将完全使用 Wayland 显示服务器协议。 这一转变影响了数百万 Linux 桌面用户，因为 Wayland 提供了更好的安全性和性能，但仍缺少 X11 的一些功能，例如完全的无障碍支持和窗口管理功能。 通过 Wayland 迁移到单一代码路径将加快开发速度并推动创新，但依赖 X11 特定功能的用户，如语音输入工具（例如 Talon）或按应用设置键盘布局，可能会遇到功能退化。

hackernews · jandeboevrie · Jun 2, 14:16 · [社区讨论](https://news.ycombinator.com/item?id=48370588)

**背景**: X11 是类 Unix 系统的传统显示服务器协议，而 Wayland 是其现代替代品，设计更简单、更安全。KDE Plasma 是一个流行的桌面环境，一直在逐步改进对 Wayland 的支持，现在计划完全放弃 X11。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Wayland_display_server">Wayland display server</a></li>
<li><a href="https://en.wikipedia.org/wiki/X_display_server">X display server</a></li>

</ul>
</details>

**社区讨论**: 社区评论表达了对 Wayland 中无障碍功能退化的担忧，一些用户指出缺少窗口位置持久化和按应用设置键盘布局等功能。其他人则赞扬 KDE 在推动 Wayland 发展方面取得的进展。

**标签**: `#KDE`, `#Wayland`, `#Linux desktop`, `#X11`, `#accessibility`

---

<a id="item-5"></a>
## [微软发布高效 MAI 大模型，仅需少量活跃参数](https://simonwillison.net/2026/Jun/2/microsofts-new-models/#atom-everything) ⭐️ 8.0/10

微软宣布了两款新的文本大模型：MAI-Thinking-1（一款 1 万亿参数、仅 350 亿活跃参数的推理模型）和 MAI-Code-1-Flash（一款 1370 亿参数、50 亿活跃参数的代码模型），二者均采用混合专家（MoE）架构。 这些模型表明，使用更少的活跃参数即可实现高性能，有望降低部署成本和能耗。同时也凸显了微软在高效 AI 方面的投入，但训练数据仍依赖于大规模网页爬取，许可问题仍在争论之中。 MAI-Thinking-1 是一款面向特定早期合作伙伴的推理模型；MAI-Code-1-Flash 则正逐步向 VS Code 中的 GitHub Copilot 用户推出。训练数据包括从 1.2 万亿页过滤至 7940 亿页的专有爬取数据，以及 Common Crawl，并过滤了 AI 生成内容和成人/盗版域名。

rss · Simon Willison · Jun 2, 22:21

**背景**: 混合专家（MoE）架构每次输入仅激活一部分参数，从而在保持模型容量的同时降低计算量。总参数计数包括所有参数，而活跃参数是单次前向传播中使用的参数；这一区别对于理解 MAI-Thinking-1（总参数 1T，活跃 35B）等模型至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.f22labs.com/blogs/active-vs-total-parameters-whats-the-difference/">Active vs Total Parameters: What's the Difference?</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained</a></li>

</ul>
</details>

**标签**: `#AI`, `#Microsoft`, `#LLMs`, `#model efficiency`

---

<a id="item-6"></a>
## [特朗普签署 AI 行政令，要求企业自愿提交模型审查](https://www.whitehouse.gov/presidential-actions/2026/06/promoting-advanced-artificial-intelligence-innovation-and-security/) ⭐️ 8.0/10

2026 年 6 月 2 日，美国总统特朗普签署了一项行政命令，建立自愿框架，要求 AI 开发者在公开发布先进 AI 模型前 30 天，将其提交给政府进行网络安全审查。 这项命令表明美国政府意图通过合作、非强制性的方式来平衡 AI 创新与国家安全，可能为未来 AI 监管树立先例。 审查期从最初提议的 90 天缩短至 30 天，原因是行业反对，同时命令明确禁止任何强制性的政府许可或预审机制。

telegram · zaihuapd · Jun 2, 16:44

**背景**: 该行政命令针对“受保护的尖端模型”，即最先进、潜在风险最高的 AI 系统。它还指示财政部、国防部和国土安全部组建 AI 网络安全清算所，协调漏洞扫描与修复。这一自愿审查机制基于此前关于 AI 是否应像药品或医疗器械一样被监管的讨论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.implicator.ai/trump-signs-ai-order-for-voluntary-pre-release-cyber-reviews/">Trump signs voluntary AI cyber review order</a></li>
<li><a href="https://thenextweb.com/news/trump-signs-downsized-ai-executive-order-voluntary-review">Trump signs narrowed AI order with voluntary 30-day model review</a></li>
<li><a href="https://federalnewsnetwork.com/cybersecurity/2026/06/ai-executive-order-sets-stage-for-new-cybersecurity-directives/">AI executive order sets stage for new cybersecurity directives | Federal News Network</a></li>

</ul>
</details>

**标签**: `#AI regulation`, `#executive order`, `#cybersecurity`, `#US policy`, `#AI safety`

---

<a id="item-7"></a>
## [谷歌向 Play Store 开发者付费获取代码训练 AI](https://www.neowin.net/reports/google-wants-to-pay-play-store-developers-for-code-to-train-its-ai/) ⭐️ 8.0/10

谷歌正私下联系 Android 开发者，提议付费获取其私有代码库的非独家使用权，用于训练 AI 模型和改进开发工具。 此举帮助谷歌缩小与 GitHub Copilot 和 Claude Code 等竞争对手在 AI 辅助编程方面的差距，同时为开发者提供新的收入来源，并可能带来更好的 Android 开发工具。 该安排是非排他性的，开发者保留 100%知识产权并可将代码授权给他人。谷歌计划利用这些代码训练其 Gemini 模型并改进 Antigravity 2.0 等工具。

telegram · zaihuapd · Jun 3, 02:47

**背景**: 用于代码生成的大型语言模型（如 GitHub Copilot 和 Claude Code）依赖海量代码库进行训练。谷歌的 Gemini 在该领域竞争但落后于对手。为了追赶，谷歌采取了新颖的数据获取策略，直接激励开发者贡献高质量的私有代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://antigravity.google/product/antigravity-2">Google Antigravity - Antigravity 2.0</a></li>

</ul>
</details>

**标签**: `#AI`, `#Google`, `#Android`, `#Code Generation`, `#Developer Tools`

---