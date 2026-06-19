---
layout: default
title: "Horizon Summary: 2026-06-19 (ZH)"
date: 2026-06-19
lang: zh
---

> From 37 items, 13 important content pieces were selected

---

1. [发现 1 万个 GitHub 仓库传播木马恶意软件](#item-1) ⭐️ 9.0/10
2. [诺姆·沙泽尔加入 OpenAI](#item-2) ⭐️ 9.0/10
3. [Z.ai 发布强大开源权重 LLM GLM-5.2](#item-3) ⭐️ 9.0/10
4. [Ubiquiti 推出基于 ZFS 的企业级 NAS](#item-4) ⭐️ 8.0/10
5. [康奈尔大学高级编译器课程免费自学上线](#item-5) ⭐️ 8.0/10
6. [医院以 90%更低成本重新利用药物](#item-6) ⭐️ 8.0/10
7. [强制同意罚款：Elkjop 被罚 180 万欧元](#item-7) ⭐️ 8.0/10
8. [Modos 彩色电子纸显示器刷新率达 60Hz](#item-8) ⭐️ 8.0/10
9. [Datasette Apps：支持 SQL 的沙盒化自定义 HTML 应用](#item-9) ⭐️ 8.0/10
10. [Charity Majors：AI 颠覆代码经济学](#item-10) ⭐️ 8.0/10
11. [苹果与英特尔达成初步芯片代工协议](#item-11) ⭐️ 8.0/10
12. [小米开源 Miloco 2.0 智能家居方案](#item-12) ⭐️ 8.0/10
13. [中国拟规区块链数字身份互通互认](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [发现 1 万个 GitHub 仓库传播木马恶意软件](https://orchidfiles.com/github-repositories-distributing-malware/) ⭐️ 9.0/10

一名研究人员发现超过 1 万个 GitHub 仓库通过操纵提交（如每隔几小时删除并推送新提交）来传播木马恶意软件。 这种大规模攻击对开源供应链安全构成严重威胁，因为自动化代理可能会在不知情的情况下克隆受感染的仓库作为依赖项，可能导致广泛感染。 恶意仓库通常是合法项目的克隆并注入了木马，它们不以人类为目标，而是针对搜索依赖项的自动化代理。频繁的提交操纵帮助它们出现在搜索结果中。

hackernews · theorchid · Jun 18, 11:45 · [社区讨论](https://news.ycombinator.com/item?id=48583928)

**背景**: 供应链攻击利用软件组件之间的信任关系，攻击者通过破坏一个依赖项来感染下游用户。GitHub 是托管开源代码的热门平台，但其宽松的特性可能被滥用。提交操纵（包括 commit stomping 等技术）允许攻击者更改仓库历史记录以逃避检测。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cybersecuritynews.com/commit-stomping/">Commit Stomping - An Offensive Technique Let Hackers Manipulate ...</a></li>
<li><a href="https://cybersecuritynews.com/23000-github-repositories-targeted/">23,000 GitHub Repositories Targeted In Supply Chain Attack</a></li>

</ul>
</details>

**社区讨论**: 评论者讨论了攻击策略的原因：针对代理而不是人类，以及操纵提交时间以出现在“最近更新”搜索的顶部。一位用户报告了类似的受害经历，发现自己的名字被附加到未知的恶意软件传播项目上。

**标签**: `#security`, `#malware`, `#GitHub`, `#supply chain`, `#Trojan`

---

<a id="item-2"></a>
## [诺姆·沙泽尔加入 OpenAI](https://twitter.com/NoamShazeer/status/2067400851438932297) ⭐️ 9.0/10

诺姆·沙泽尔是开创性论文《Attention Is All You Need》的合著者及 Character.AI 的联合创始人，他已离开谷歌加入 OpenAI，这一消息通过他的推文和路透社的报道确认。此次变动发生在他于 2024 年重返谷歌并担任 Gemini 联合负责人后不久。 沙泽尔的举动意义重大，因为他是 Transformer 架构的关键设计者之一，该架构支撑了大多数现代大型语言模型。他加入 OpenAI 可能会加速其研发工作，加剧 AI 行业的竞争。 沙泽尔于 2024 年通过一项与 Character.AI 的许可和人才协议重返谷歌，该协议据报价值约 27 亿美元，他随后成为 Gemini 项目的联合负责人。他此次离职转投 OpenAI 出乎意料，标志着顶尖 AI 公司之间的人才重大变动。

hackernews · lukasgross · Jun 18, 00:26 · [社区讨论](https://news.ycombinator.com/item?id=48578913)

**背景**: 诺姆·沙泽尔是知名计算机科学家，于 2000 年加入谷歌，曾参与拼写检查和 AdSense 等早期项目。他是 2017 年论文《Attention Is All You Need》的八位合著者之一，该论文提出了 Transformer 架构，通过实现高效的并行处理彻底改变了人工智能。Transformer 是 GPT-4 和谷歌 Gemini 等大型语言模型的基础。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Noam_Shazeer">Noam Shazeer</a></li>
<li><a href="https://en.wikipedia.org/wiki/Transformer_architecture">Transformer architecture</a></li>

</ul>
</details>

**社区讨论**: 评论者对沙泽尔在回归后迅速离开谷歌表示惊讶，有人回忆起他在谷歌的传奇地位和深厚的技术贡献。讨论还强调了谷歌与 OpenAI 之间的人才争夺战，并推测这对下一代 AI 模型开发的潜在影响。

**标签**: `#OpenAI`, `#Noam Shazeer`, `#AI industry`, `#transformers`, `#personnel move`

---

<a id="item-3"></a>
## [Z.ai 发布强大开源权重 LLM GLM-5.2](https://simonwillison.net/2026/Jun/17/glm-52/#atom-everything) ⭐️ 9.0/10

Z.ai 发布了 GLM-5.2，这是一个 753B 参数的混合专家（MoE）纯文本 LLM，具有 100 万 token 的上下文窗口，采用 MIT 许可证。 GLM-5.2 在 Artificial Analysis 智能指数上取得最高分，超越了 MiniMax-M3 和 DeepSeek V4 Pro 等其他开源权重模型，并在 Code Arena WebDev 上排名第二，证明了其作为纯文本模型的卓越性能。 该模型每个任务平均使用 43k 输出 token，高于同类模型，表明 token 消耗较高。它通过 OpenRouter 提供，输入 token 价格为 1.40 美元/百万，输出价格为 4.40 美元/百万，远低于 GPT-5.5 和 Claude Opus。

rss · Simon Willison · Jun 17, 23:58

**背景**: 混合专家（MoE）是一种架构，每次只激活一部分参数，从而实现大模型容量和高效计算。上下文窗口是 LLM 一次能考虑的最大文本量；GLM-5.2 的 100 万 token 窗口相比前代的 20 万有显著提升。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/google-cloud/how-mixture-of-experts-llms-work-58b3ba8e0349">How Mixture-of-Experts LLMs Work - Medium</a></li>
<li><a href="https://en.wikipedia.org/wiki/Context_window">Context window - Wikipedia</a></li>

</ul>
</details>

**标签**: `#open-weights`, `#LLM`, `#AI`, `#natural language processing`, `#MIT license`

---

<a id="item-4"></a>
## [Ubiquiti 推出基于 ZFS 的企业级 NAS](https://blog.ui.com/article/introducing-enterprise-nas) ⭐️ 8.0/10

Ubiquiti 宣布推出一款基于 ZFS 文件系统的新企业级 NAS 产品，标志着其进入网络附加存储市场。该设备配备双 25 Gigabit SFP28 端口和冗余电源。 这很重要，因为作为主要网络设备供应商的 Ubiquiti 进入 NAS 领域，并采用以数据完整性和高级功能著称的 ZFS 文件系统。它可能挑战现有的 NAS 供应商如 QNAP 和群晖，尤其对于偏好无订阅模式的用户。 该 NAS 定价 3999 美元，面向企业用户。社区讨论中提到了对 Ubiquiti 过去安全和软件质量问题的担忧，以及尽管有高速网络接口，但使用机械硬盘时可能存在的性能瓶颈。

hackernews · ksec · Jun 18, 14:24 · [社区讨论](https://news.ycombinator.com/item?id=48585866)

**背景**: ZFS 是一种高级文件系统，结合了卷管理和数据保护功能，例如用于数据完整性的校验和、快照和复制。与传统文件系统不同，ZFS 可以跨多个驱动器组成存储池，并防止比特腐烂和数据损坏。Ubiquiti 以其网络硬件闻名，但也因软件可靠性和安全事件受到批评。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ZFS">ZFS - Wikipedia</a></li>
<li><a href="https://itsfoss.com/what-is-zfs/">What is ZFS? Why are People Crazy About it?</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：一些人赞扬 ZFS 和无订阅模式，而另一些人则对 Ubiquiti 过去的安全漏洞和软件质量表示担忧。此外，还有人对使用机械硬盘饱和 25 Gbps 链路的技术可行性表示怀疑。

**标签**: `#Ubiquiti`, `#NAS`, `#ZFS`, `#Enterprise Storage`, `#Hardware`

---

<a id="item-5"></a>
## [康奈尔大学高级编译器课程免费自学上线](https://www.cs.cornell.edu/courses/cs6120/2025fa/self-guided/) ⭐️ 8.0/10

康奈尔大学的 CS 6120：高级编译器课程（阿德里安·桑普森教授授课）现以免费自学在线资源形式开放，包含讲座视频和作业。 该课程为全球学习者提供了可获取的高质量高级编译器教育，填补了自学者在系统和编程语言实现方面的空白。 课程涵盖数据流、SSA 形式等经典主题，以及 JIT 编译、并行化和垃圾回收等研究性主题，并包含博客和 GitHub 仓库供动手实践。

hackernews · ibobev · Jun 18, 11:04 · [社区讨论](https://news.ycombinator.com/item?id=48583606)

**背景**: 高级编译器课程传统上需要计算机科学背景，且通常只在大学授课。这个自学版本消除了障碍，提供了与线下授课类似的讲座视频和作业。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cs.cornell.edu/courses/cs6120/2020fa/self-guided/">CS 6120: Advanced Compilers: The Self-Guided Online Course</a></li>
<li><a href="https://github.com/sampsyo/cs6120">GitHub - sampsyo/cs6120: advanced compilers</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的评论指出，动态编译器部分侧重于追踪编译，有人认为这是死胡同，但整体课程质量受到赞扬。对于内容是否真正‘高级’或适合编译器入门课程存在争议。

**标签**: `#compilers`, `#online-course`, `#advanced-compilers`, `#education`, `#systems`

---

<a id="item-6"></a>
## [医院以 90%更低成本重新利用药物](https://www.kcl.ac.uk/news/hospitals-and-universities-repurposing-drugs-at-90-lower-cost) ⭐️ 8.0/10

医院和大学正在将现有药物重新用于新的治疗用途，与专利替代品相比，成本降低高达 90%。例如，癌症药物贝伐珠单抗（Avastin）被超说明书用于黄斑变性，每剂 50 美元，而批准药物 Lucentis 每剂 1500 美元。 这种做法挑战了制药定价模式，扩大了可负担治疗的可及性，特别是针对罕见或被忽视的疾病。它揭示了药品定价的系统性问题，并可能将激励转向基于证据的重新利用，而不是开发昂贵的新药。 药物重新利用得益于减少的临床试验步骤和已知的安全特性，但缺乏明确的监管途径以在没有制造商同意的情况下用于新适应症。社区评论指出，艾司氯胺酮（Spravato）是已过专利的氯胺酮的专利修饰版本，但证据表明其效果不如原药。

hackernews · giuliomagnifico · Jun 18, 10:33 · [社区讨论](https://news.ycombinator.com/item?id=48583386)

**背景**: 药物重新利用（也称为药物重定位）为现有 FDA 批准药物寻找新用途，有可能缩短上市时间和降低成本。它依赖于已知的安全性和药代动力学数据，通常用于罕见病研究，因为新药开发在经济上不可行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Drug_repurposing">Drug repurposing</a></li>
<li><a href="https://www.fda.gov/drugs/resources-drugs/drug-repurposing">Drug Repurposing | FDA</a></li>

</ul>
</details>

**社区讨论**: 评论者提供了具体例子和个人经历：一位指出 Avastin/Lucentis 的成本差异和分子相似性；另一位强调了非营利组织 Cures Within Reach 对亨廷顿病的研究。第三位批评 Spravato 是氯胺酮效果较差的专利版本，说明了美国医疗保健激励机制的缺陷。

**标签**: `#drug repurposing`, `#healthcare costs`, `#pharmaceuticals`, `#public health`

---

<a id="item-7"></a>
## [强制同意罚款：Elkjop 被罚 180 万欧元](https://www.thatprivacyguy.com/blog/elkjop-forced-consent-fine/) ⭐️ 8.0/10

挪威数据保护机构 Datatilsynet 对电子产品零售商 Elkjop 处以 2000 万挪威克朗（约 180 万欧元）罚款，因其要求顾客将同意接收营销信息作为加入忠诚俱乐部的条件，违反了 GDPR 关于自由给予同意的规定。 此次执法明确了 GDPR 禁止将服务会员资格与同意营销挂钩，为欧洲经济区的忠诚度计划树立了先例。同时也表明个人投诉能够推动重大的监管行动，从而增强隐私倡导者的力量。 罚款是在隐私倡导者警告 Elkjop 其做法违法五年后下达的。Elkjop 书面明确表示接收营销是会员资格的条件，这构成了强制同意。官方决定可在 Datatilsynet 网站上获取英文版本。

hackernews · speckx · Jun 18, 18:31 · [社区讨论](https://news.ycombinator.com/item?id=48589501)

**背景**: 根据 GDPR 第 4 条第 11 款，同意必须是自由给予的、具体的、知情的且不含糊的。第 7 条第 4 款禁止将服务访问与对非必要处理的同意捆绑。EDPB 指南强调，将同意与服务条款捆绑会使同意无效，因为个人无法真正做出选择。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.thatprivacyguy.com/blog/elkjop-forced-consent-fine/">I told them forced consent was unlawful. Five years later it ...</a></li>
<li><a href="https://www.edpb.europa.eu/sites/default/files/files/file1/edpb_guidelines_202005_consent_en.pdf">PDF Guidelines 05/2020 on consent under Regulation 2016/679 Version 1 - Europa</a></li>

</ul>
</details>

**社区讨论**: 评论者们普遍赞扬这一结果，有些人指出了投诉人起诉了为他赢得案件的实体这一讽刺之处。一位评论者提供了挪威语官方决定和英文机器翻译的链接。另一位评论者表示希望更多人能够行使自己的隐私权。

**标签**: `#GDPR`, `#privacy`, `#data protection`, `#forced consent`, `#fine`

---

<a id="item-8"></a>
## [Modos 彩色电子纸显示器刷新率达 60Hz](https://spectrum.ieee.org/modos-e-paper-monitor) ⭐️ 8.0/10

初创公司 Modos（仅两人）正在开发一款 13.3 英寸彩色电子纸显示器，原生分辨率 3200x2400，刷新率 60Hz，这对传统刷新率较低的电子纸显示器来说是一个重大飞跃。 这一进展将使电子纸显示器凭借高刷新率和分辨率，有望适用于通用计算（包括视频播放和交互任务），相比 LCD 可能降低眼疲劳和功耗。 该显示器名为 Modos Flow，支持触控输入，正在通过众筹募集资金。60Hz 刷新率引发了关于电泳显示面板寿命的问题，因为更高的刷新率可能会加速老化。

hackernews · Vinnl · Jun 18, 11:41 · [社区讨论](https://news.ycombinator.com/item?id=48583897)

**背景**: 电子纸显示器（如基于 E Ink 技术的产品）利用电泳粒子反射环境光，具有低功耗和在强光下可读的优点，但通常刷新率较低（常低于 20Hz）且色彩表现有限，限制了其在电子阅读器和数字标牌等领域的应用。Modos 的显示器旨在通过实现 60Hz 刷新率和高分辨率来克服这些限制，从而开辟新的使用场景。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.samsung.com/us/story-behind-samsung-color-e-paper-digital-signage-solution-displays-2-5-million-colors-without-continuous-power/">The Story Behind Samsung Color E-Paper: The Digital Signage Solution ...</a></li>
<li><a href="https://news.samsung.com/global/interview-i-thought-it-was-real-paper-the-story-behind-samsung-color-e-paper-the-digital-signage-solution-that-displays-2-5-million-colors-without-continuous-power">[Interview] 'I Thought It Was Real Paper' — The Story Behind Samsung ...</a></li>

</ul>
</details>

**社区讨论**: 社区成员对这个进展表示兴奋，有人提到创作者发布的有用 YouTube 视频。一位评论者担忧 60Hz 刷新率对面板寿命的影响，另一位则强调了户外可用、低功耗设备的潜力。总体情绪积极，人们称赞其规格并希望得到更广泛的应用。

**标签**: `#e-paper`, `#displays`, `#startups`, `#hardware`, `#innovation`

---

<a id="item-9"></a>
## [Datasette Apps：支持 SQL 的沙盒化自定义 HTML 应用](https://simonwillison.net/2026/Jun/18/datasette-apps/#atom-everything) ⭐️ 8.0/10

Simon Willison 发布了 Datasette 的 datasette-apps 插件，允许用户在沙盒化的 iframe 中托管自定义的 HTML+JavaScript 应用，并可对底层数据库进行读写 SQL 访问。 该插件将 Datasette 从数据探索工具大幅扩展为构建交互式 SQL 驱动 Web 应用的平台，使数据记者、研究人员和开发者无需离开 Datasette 生态系统即可创建自定义界面。 应用运行在受限的 iframe 中，设置 sandbox="allow-scripts allow-forms" 并注入 CSP 头，阻止对外 HTTP 请求，防止数据泄露。只有通过存储查询配置后才能执行写入操作。

rss · Simon Willison · Jun 18, 23:58

**背景**: Datasette 是一个开源工具，可将 SQLite 数据库转换为带有 JSON API 的交互式网页，广泛用于数据发布和探索。datasette-apps 插件最初是 Datasette Agent 的一个功能，但由于其沙盒模式具有广泛实用性而独立成为一个插件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jun/18/datasette-apps/">Datasette Apps: Host custom HTML applications inside Datasette</a></li>
<li><a href="https://datasette.io/plugins">Datasette Plugins</a></li>
<li><a href="https://docs.datasette.io/en/stable/plugins.html">Plugins - Datasette documentation</a></li>

</ul>
</details>

**标签**: `#Datasette`, `#plugin`, `#data visualization`, `#SQL`, `#JavaScript`

---

<a id="item-10"></a>
## [Charity Majors：AI 颠覆代码经济学](https://simonwillison.net/2026/Jun/17/charity-majors/#atom-everything) ⭐️ 8.0/10

Charity Majors 指出，到 2025 年，代码生产的经济学发生了剧变：生成代码变得几乎免费和即时，而不再困难、耗时且昂贵。 这一范式转变意味着代码变得可丢弃和可重新生成，迫使人们重新思考软件工程实践以及代码工艺的价值。 该引文来自她的 Substack 文章《AI 需要更多工程纪律，而非更少》，强调尽管代码生成变得廉价，工程纪律反而更加重要。

rss · Simon Willison · Jun 17, 17:12

**背景**: 传统上，编写和维护代码成本高昂，因此工程师将其视为需要复用和精心管理的宝贵资产。AI 驱动的代码生成工具颠覆了这一点，使得重新生成代码比维护旧代码更便宜。

**标签**: `#ai-assisted-programming`, `#software-engineering`, `#generative-ai`, `#economics-of-code`

---

<a id="item-11"></a>
## [苹果与英特尔达成初步芯片代工协议](https://t.me/zaihuapd/42031) ⭐️ 8.0/10

苹果与英特尔已达成初步协议，由英特尔代工生产部分苹果设备所需的芯片。该协议经过一年多的谈判，并在美国政府的深度推动下最终敲定。 该协议使苹果的芯片供应不再单一依赖台积电，并加强了英特尔的代工业务，对半导体供应链的地缘政治和美国制造业目标具有重要影响。 目前尚不清楚哪些苹果产品（iPhone、iPad 或 Mac）将使用英特尔制造的芯片。英特尔目前已有苹果、英伟达和 SpaceX 三家代工客户。

telegram · zaihuapd · Jun 18, 09:19

**背景**: 在半导体行业中，芯片代工厂是制造集成电路的工厂。传统上，英特尔是一家整合器件制造商（IDM），自行设计和制造芯片，而苹果则依赖台积电等代工厂。英特尔推出了英特尔代工服务，为外部客户制造芯片，旨在与台积电和三星竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chip_foundry">Chip foundry</a></li>
<li><a href="https://en.wikipedia.org/wiki/Intel_Foundry_Services">Intel Foundry Services</a></li>

</ul>
</details>

**标签**: `#Apple`, `#Intel`, `#chip manufacturing`, `#semiconductor`, `#foundry`

---

<a id="item-12"></a>
## [小米开源 Miloco 2.0 智能家居方案](https://github.com/XiaoMi/xiaomi-miloco) ⭐️ 8.0/10

小米正式开源自研智能家居方案 Miloco 2.0，它通过米家摄像头的音视频感知环境，内置 MiMo 大模型作为 OpenClaw 插件运行，实现主动式设备控制。 此举将强大的 AI 驱动家居自动化能力开放给开发者和爱好者，通过引入大模型实现主动推理与控制，有望推动开源智能家居生态的发展。 Miloco 2.0 需在 macOS 或 Linux（Windows 通过 WSL）上运行，建议 4 GB 内存和 256 GB 存储，并绑定小米账号与 MiMo API 密钥。感知与 Agent 依赖云端大模型，会产生持续的 API 费用，且该项目仅限非商业用途。

telegram · zaihuapd · Jun 18, 12:23

**背景**: Miloco 是小米开源智能家居平台，利用 AI 实现家庭自动化。MiMo 大模型是小米自研的大语言模型，提供多种定价方案。OpenClaw 是一个开源 AI Agent 框架，支持安装 Miloco 等插件。通过整合这些技术，Miloco 2.0 可以解读摄像头画面并主动调整智能设备。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/XiaoMi/xiaomi-miloco">Xiaomi Miloco - GitHub</a></li>
<li><a href="https://xiaomiforall.com/xiaomi-miloco-2-0-smart-home-ai/">Xiaomi Miloco 2.0: The AI Revolution for Your Smart Home</a></li>
<li><a href="https://open-claw.bot/docs/tools/plugins/">OpenClaw Plugins : Extend Your AI Agent | OpenClaw</a></li>

</ul>
</details>

**标签**: `#open source`, `#smart home`, `#AI`, `#Xiaomi`, `#large language model`

---

<a id="item-13"></a>
## [中国拟规区块链数字身份互通互认](https://www.cac.gov.cn/2026-06/18/c_1783525605384124.htm) ⭐️ 8.0/10

2026 年 6 月 18 日，国家网信办发布《促进分布式数字身份互通互认应用规定（征求意见稿）》，公开征求意见，旨在基于区块链技术推动分布式数字身份的互通互认。 该规定可能建立国家级的分布式身份管理框架，增强数据安全和用户控制权，同时实现金融、交通、海关、税务和数字人民币等跨领域的身份互认。 征求意见稿明确分布式数字身份由标识符、密钥、可验证凭证和可验证声明构成，并规定不满 14 周岁的用户需征得父母或其他监护人同意方可申领。

telegram · zaihuapd · Jun 19, 01:39

**背景**: 分布式数字身份（DID）是一种去中心化身份模型，允许用户自主控制身份数据，无需依赖中心化机构。借助区块链技术，DID 能生成可在不同平台间使用的安全可验证凭证。传统的中心化身份系统常面临隐私泄露风险与跨域互信难题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.news.cn/politics/20260618/780f2dbba382444385e6b59d0cd53dd4/c.html">国家互联网信息办公室关于《促进分布式数字身份互通互认应用规定（征求意见稿）》公开征求意见的通知-新华网</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/506783361">Dpki的崛起之路——分布式数字身份 (Did) - 知乎</a></li>
<li><a href="https://www.secrss.com/articles/84215">分布式数字身份技术概述 - 安全内参 | 决策者的网络安全知识库</a></li>

</ul>
</details>

**标签**: `#distributed digital identity`, `#blockchain`, `#regulation`, `#China`, `#data security`

---