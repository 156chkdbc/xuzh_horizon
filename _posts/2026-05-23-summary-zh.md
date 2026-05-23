---
layout: default
title: "Horizon Summary: 2026-05-23 (ZH)"
date: 2026-05-23
lang: zh
---

> From 38 items, 13 important content pieces were selected

---

1. [Anthropic 推出 Project Glasswing，用 Mythos AI 检测漏洞](#item-1) ⭐️ 9.0/10
2. [SpaceX 发射星舰 v3 火箭，结果喜忧参半](#item-2) ⭐️ 9.0/10
3. [中国审查 Meta 收购 Manus，限制创始人离境](#item-3) ⭐️ 9.0/10
4. [礼来 Retatrutide 三期试验平均减重 28.3%](#item-4) ⭐️ 9.0/10
5. [Antigravity 2.0 在 OpenSCAD 建筑 3D LLM 基准测试中夺冠](#item-5) ⭐️ 8.0/10
6. [yt-dlp 因安全与兼容性问题弃用 Bun 支持](#item-6) ⭐️ 8.0/10
7. [安娜的档案要求 AI 模型捐款，引发 AI 伦理争议](#item-7) ⭐️ 8.0/10
8. [美国研究人员面临与外国合作者发表论文的新限制](#item-8) ⭐️ 8.0/10
9. [AI 内存需求推动消费电子涨价](#item-9) ⭐️ 8.0/10
10. [FTC 对 Cox Media Group 罚款 100 万美元，因虚假'主动监听'AI 广告](#item-10) ⭐️ 8.0/10
11. [字节跳动开源 3B 多模态模型 Lance](#item-11) ⭐️ 8.0/10
12. [中国八部门整治非法跨境证券，拉勾网破产重整](#item-12) ⭐️ 8.0/10
13. [Cloudflare 因修复 Next.js 漏洞导致全球网络中断](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Anthropic 推出 Project Glasswing，用 Mythos AI 检测漏洞](https://www.anthropic.com/research/glasswing-initial-update) ⭐️ 9.0/10

Anthropic 宣布了 Project Glasswing 项目，利用其 Mythos AI 模型检测安全漏洞，实现了 90.6% 的真阳性率，并经独立安全公司验证发现了数千个可利用的缺陷。 这一突破可能大幅减少寻找零日漏洞的时间和成本，有望改变代码安全分析的面貌。然而，它也引发了人们对 AI 驱动的黑客工具被用于攻击目的的担忧。 在六家独立安全研究公司评估的 1,752 个高级或严重级别漏洞中，90.6%（1,587 个）为有效真阳性，62.4%（1,094 个）被确认为高或严重级别。该模型目前仅限邀请预览。

hackernews · louiereederson · May 22, 19:31 · [社区讨论](https://news.ycombinator.com/item?id=48240419)

**背景**: Project Glasswing 是 Anthropic 的一项计划，旨在将 AI 应用于防御性网络安全，使用 Claude Mythos 模型。Mythos 是由 Anthropic 开发的大型语言模型，专为代码分析而设计。该项目旨在帮助保护人工智能时代的关键软件，但也引发了关于双重用途风险的讨论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/glasswing">Project Glasswing: Securing critical software for the AI era \ Anthropic</a></li>
<li><a href="https://thehackernews.com/2026/04/anthropics-claude-mythos-finds.html">Anthropic's Claude Mythos Finds Thousands of Zero-Day Flaws Across ...</a></li>
<li><a href="https://www.forbes.com/sites/paulocarvao/2026/04/08/five-reasons-anthropic-kept-its-cybersecurity-breakthrough-invite-only/">Five Reasons Anthropic Kept Its Cybersecurity Breakthrough ... - Forbes</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：一些用户如 mdeeks 报告了高准确性和实用性，而怀疑者如 mukmuk 引用 curl 维护者 Daniel Steinberg 的观点，认为 Mythos 并不比现有工具明显更好。其他人如 nikcub 则为这些数字辩护，demorro 则认为在应用昂贵的 LLM 工具之前，应首先使用基本的静态分析。

**标签**: `#AI`, `#security`, `#vulnerability detection`, `#Anthropic`, `#code analysis`

---

<a id="item-2"></a>
## [SpaceX 发射星舰 v3 火箭，结果喜忧参半](https://www.nbcnews.com/now/video/spacex-successfully-launches-prototype-of-starship-rocket-263835205505) ⭐️ 9.0/10

SpaceX 首次试飞成功发射星舰 v3 火箭，尽管损失了一台发动机，但上面级成功再入并精确着陆，而超重型助推器未能返回发射场，偏离目标着陆。 这次测试标志着可重复使用火箭技术的重大进展，尤其是在隔热罩性能方面，使 SpaceX 更接近完全可重复使用的重型运载能力，这可以降低太空进入成本，并为登月和火星任务铺平道路。 星舰 v3 采用全新推进系统设计，增加了推进剂储箱容积，并改进了反应控制系统。再入期间隔热罩没有出现可见热点，这是相对于之前飞行的显著改进，但助推器的回推燃烧失败，最终硬着陆在海洋中。

hackernews · busymom0 · May 22, 23:41 · [社区讨论](https://news.ycombinator.com/item?id=48242959)

**背景**: SpaceX 的星舰是一种完全可重复使用的两级火箭，旨在将大型有效载荷和机组人员运送到地球轨道以外的目的地。v3 版本是最新的迭代，比前代更高、更强大。成功的再入和着陆对于重复使用至关重要，而早期飞行的隔热罩问题是一个关键挑战。这次飞行的改进表明向运营状态迈进了。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.spacex.com/updates/starship-v3">SpaceX - Updates</a></li>
<li><a href="https://www.scientificamerican.com/article/spacex-launches-starship-v3-the-worlds-most-powerful-and-tallest-rocket-ever/">SpaceX launches Starship V3—the world's most powerful and tallest ...</a></li>
<li><a href="https://www.space.com/space-exploration/launches-spacecraft/spacex-starship-v3-megarocket-first-test-flight">SpaceX just launched Starship V3 — its most powerful megarocket yet ...</a></li>

</ul>
</details>

**社区讨论**: 评论者注意到令人印象深刻的再入过程没有可见热点，将其归因于改进的隔热罩设计。对助推器未能返回感到失望，但整体情绪对上面级的性能表示积极。一些人强调了发动机舱的戏剧性画面和模拟卫星燃烧的壮观景象。

**标签**: `#space`, `#SpaceX`, `#rocketry`, `#engineering`, `#technology`

---

<a id="item-3"></a>
## [中国审查 Meta 收购 Manus，限制创始人离境](https://t.me/zaihuapd/41509) ⭐️ 9.0/10

中国监管部门正在审查 Meta 收购 AI 初创公司 Manus 是否违反投资规定，并已限制联合创始人兼 CEO 肖红和首席科学家季一超离境。 这标志着中国政府对涉及 AI 的外国技术收购审查显著升级，直接限制创始人离境，凸显了 AI 交易中的地缘政治紧张局势。 Meta 于 2025 年 12 月宣布收购通用型 AI 智能体开发商 Manus，交易金额未公开。两位联合创始人在北京与国家发展和改革委员会会面后被告知不得出境。

telegram · zaihuapd · May 21, 13:11

**背景**: AI 智能体是一种能够自主代表用户执行任务的系统。Manus 由北京初创公司蝴蝶效应开发，是一个通用型 AI 智能体，能够处理编程、研究和数据分析等任务。Meta 收购该公司的目的是将 AI 智能体推广到全球企业。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Manus_(AI_agent)">Manus (AI agent) - Wikipedia</a></li>
<li><a href="https://manus.im/">Manus: Hands On AI</a></li>

</ul>
</details>

**标签**: `#Meta`, `#Manus`, `#AI`, `#acquisition`, `#regulation`

---

<a id="item-4"></a>
## [礼来 Retatrutide 三期试验平均减重 28.3%](https://www.prnewswire.com/news-releases/lillys-triple-agonist-retatrutide-delivered-powerful-weight-loss-in-pivotal-phase-3-obesity-trial-302778859.html) ⭐️ 9.0/10

礼来公司宣布，其三重激动剂 retatrutide 在三期 TRIUMPH-1 试验中实现了平均 28.3% 的减重效果，其中 45.3% 的参与者减重至少 30%。 这一结果代表了肥胖治疗的重大进展，可能提供优于现有 GLP-1 类药物的减重效果，并可能重塑代谢疾病药物市场。 12 mg 剂量组平均减重 28.3%，4 mg 组平均减重 19.0%；因不良事件停药率为 4.1%（retatrutide）对比 4.9%（安慰剂），最常见副作用为胃肠道反应。

telegram · zaihuapd · May 22, 02:18

**背景**: Retatrutide 是一种在研的三重激动剂，同时激活 GIP、GLP-1 和胰高血糖素受体，协同增强减重和代谢益处。它每周注射一次，正在开发用于肥胖和 2 型糖尿病。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://investor.lilly.com/news-releases/news-release-details/lillys-triple-agonist-retatrutide-delivered-powerful-weight-loss">Lilly's triple agonist, retatrutide, delivered powerful weight loss in ...</a></li>
<li><a href="https://www.empr.com/news/retatrutide-weight-loss-obesity-triumph-1-trial/">TRIUMPH-1: Triple Agonist Retatrutide Yields Significant ...</a></li>

</ul>
</details>

**标签**: `#weight loss`, `#clinical trial`, `#obesity`, `#pharmaceutical`, `#retatrutide`

---

<a id="item-5"></a>
## [Antigravity 2.0 在 OpenSCAD 建筑 3D LLM 基准测试中夺冠](https://modelrift.com/blog/openscad-llm-benchmark/) ⭐️ 8.0/10

一项新的基准测试评估了大型语言模型生成建筑 3D 模型的 OpenSCAD 代码的能力，谷歌的 Antigravity 2.0 通过正确实现万神殿复杂的格子天花板内部结构而获得最高性能。该基准测试要求模型为万神殿等标志性建筑生成参数化代码。 该基准测试引入了一种对 LLM 生成的参数化 3D 建模代码的新颖评估方式，这一领域在设计和制造中具有实际应用价值。Antigravity 2.0 的强劲表现凸显了专业 AI 代理在 CAD 任务中的潜力，但社区反馈也提出了对现实世界可用性和模型一致性的担忧。 Antigravity 2.0 是唯一一个实现了万神殿通过穹顶可见的重复方形藻井内部天花板图案的自主代理。该基准测试涉及为多个建筑模型生成 OpenSCAD 代码，结果突显了模型性能可能参差不齐——在某些类型中表现出色，但在其他类型中则不然。

hackernews · jetter · May 22, 10:38 · [社区讨论](https://news.ycombinator.com/item?id=48234090)

**背景**: OpenSCAD 是一款免费的基于脚本的 3D CAD 建模器，使用自己的描述语言创建实体对象。与交互式建模工具不同，OpenSCAD 完全依赖代码，因此成为测试 LLM 生成精确参数化几何体能力的合适工具。该基准测试是首批系统评估 LLM 在此特定任务上表现的测试之一，提供了关于它们在生成式设计中优缺点的见解。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenSCAD">OpenSCAD - Wikipedia</a></li>
<li><a href="https://techcrunch.com/2026/05/19/google-launches-antigravity-2-0-with-an-updated-desktop-app-and-cli-tool/">Google launches Antigravity 2.0 with an updated desktop app and CLI tool at IO 2026 | TechCrunch</a></li>
<li><a href="https://medium.com/data-science-in-your-pocket/google-antigravity-2-0-bye-claude-code-f13fd82ffb0e">Google AntiGravity 2.0 : Bye Claude Code | by Mehul Gupta | Data Science in Your Pocket | May, 2026 | Medium</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：一些用户对 Antigravity 在基准测试中的表现印象深刻，并分享了 LLM 在实际 OpenSCAD 任务中的积极经验，而另一些用户则批评 Antigravity 的推出问题，并质疑基准测试的有效性，因为样本量小且模型不一致。大家一致认为此类基准测试有用，但需要更广泛的规模才能得出定论。

**标签**: `#LLM`, `#OpenSCAD`, `#3D modeling`, `#AI benchmark`, `#generative design`

---

<a id="item-6"></a>
## [yt-dlp 因安全与兼容性问题弃用 Bun 支持](https://github.com/yt-dlp/yt-dlp/issues/16766) ⭐️ 8.0/10

yt-dlp 项目已弃用对 Bun 的支持，理由是存在可预见的兼容性和安全问题，且维护者无法审查大部分并非由他们编写的代码库。该决定与 Bun 正在进行但尚未发布的 Rust 重写相关。 此次弃用凸显了生态系统中对 AI 辅助重写项目的代码质量和安全性的日益担忧，并可能降低 Bun 在需要稳定运行时环境工具中的采用率。这也反映了当项目进行重大语言重写时，围绕可维护性的更广泛矛盾。 Bun 的 Rust 重写涉及约一百万行代码，yt-dlp 维护者称对其进行全面审查不切实际。弃用同时适用于当前基于 Zig 的 Bun 和未来基于 Rust 的版本，因为重写尚未发布。

hackernews · tamnd · May 22, 17:24 · [社区讨论](https://news.ycombinator.com/item?id=48238789)

**背景**: Bun 是一个用 Zig 构建的快速全能 JavaScript 运行时，与 Node.js 和 Deno 竞争。Bun 的创建公司 Oven 被 Anthropic 收购，随后公司宣布将 Bun 用 Rust 重写以提高内存安全性。yt-dlp 是一个流行的开源命令行程序，用于下载 YouTube 视频。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bun.sh/">Bun — A fast all-in-one JavaScript runtime</a></li>
<li><a href="https://www.reddit.com/r/programming/comments/1tcuebe/rewrite_bun_in_rust_has_been_merged/">r/programming on Reddit: Rewrite Bun in Rust has been merged</a></li>
<li><a href="https://news.ycombinator.com/item?id=48073680">Bun's experimental Rust rewrite hits 99.8% test compatibility on Linux x64 glibc | Hacker News</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：有人支持这一决定，认为审查 AI 生成的代码确实困难；也有人认为这是政治性而非技术性的，因为 Rust 重写尚未引发实际问题。部分用户对 Bun 在被 Anthropic 收购后的发展方向表示遗憾。

**标签**: `#Bun`, `#yt-dlp`, `#deprecation`, `#Rust rewrite`, `#JavaScript runtime`

---

<a id="item-7"></a>
## [安娜的档案要求 AI 模型捐款，引发 AI 伦理争议](https://annas-archive.gl/blog/llms-txt.html) ⭐️ 8.0/10

安娜的档案发布了一篇幽默的博客文章，要求那些使用其盗版数据进行训练的大型语言模型（LLM）进行捐款，以此支持进一步保存人类作品。 这篇帖子凸显了 AI 训练数据、版权侵权与道德义务之间日益交织的关系，引发了关于 AI 公司是否应补偿影子图书馆等数据来源的社区辩论。 安娜的档案是一个影子图书馆元搜索引擎，聚合来自 Sci-Hub 和 Library Genesis 等来源的书籍和论文，并被指控以超过 10,000 美元的价格向 AI 公司出售盗版材料的快速访问权限。

hackernews · janandonly · May 22, 11:28 · [社区讨论](https://news.ycombinator.com/item?id=48234413)

**背景**: 安娜的档案是一个用于影子图书馆的开源元搜索引擎，于 2022 年在 Z-Library 遭到执法打击后推出。它声称要编录所有现存书籍，并提供第三方下载链接，但因版权侵权面临法律诉讼。该网站因助长大规模盗版受版权保护的学术和文学作品而饱受争议。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anna's_Archive">Anna's Archive</a></li>
<li><a href="https://grokipedia.com/page/Anna's_Archive">Anna's Archive</a></li>

</ul>
</details>

**社区讨论**: 评论者反应幽默且怀疑，有人指出 LLM 在没有人类监督的情况下产生幻觉并捐款的讽刺性，称其为提示注入安全漏洞。另一人称赞安娜的档案通过提供免费教科书帮助他们完成了大学学业，而第三人则强调了该网站向 AI 公司收取快速数据访问费用的历史。

**标签**: `#AI ethics`, `#copyright`, `#training data`, `#Anna's Archive`, `#LLM`

---

<a id="item-8"></a>
## [美国研究人员面临与外国合作者发表论文的新限制](https://www.science.org/content/article/u-s-researchers-face-new-restrictions-publishing-foreign-collaborators) ⭐️ 8.0/10

美国国立卫生研究院（NIH）和美国国家航空航天局（NASA）开始要求研究人员报告外国合作情况，并从进展报告中删除相关论文，由于尚未发布正式指导，这引发了困惑。 这一政策变化威胁到国际科学合作，并可能因不完整的生产力数据导致资金削减。 这些限制适用于自 2003 年起就已存在的'外国成分'活动，但如今被更广泛地执行，涵盖了研究人员自身的合作。

hackernews · ceejayoz · May 22, 16:23 · [社区讨论](https://news.ycombinator.com/item?id=48238025)

**背景**: 过去十年中，美国政府因担心知识产权被盗和不当外国影响，加强了对国外人才招聘计划的审查。NIH 和 NASA 等机构现在要求受资助者披露和证明其外国合作，但尚未公开发布正式指南。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.researchsecurity.pitt.edu/research-security/foreign-talent-recruitment-programs">Foreign Talent Recruitment Programs | Office of Research Security...</a></li>
<li><a href="https://www.vanderbilt.edu/researchintegrityandcompliance/research-security/malign-foreign-talent-recruitment-programs/">Malign Foreign Talent Recruitment Programs | Research Integrity...</a></li>
<li><a href="https://researchservices.upenn.edu/areas-of-service/research-security/foreign-talent-recruitment-programs/">Foreign Talent Recruitment Programs – Office of Research Services</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了对缺乏官方指导的沮丧和困惑，并担心从进展报告中删除论文会人为降低被认为的生产力，可能导致未来资金削减。

**标签**: `#Research Policy`, `#International Collaboration`, `#Academic Freedom`, `#NIH`, `#NASA`

---

<a id="item-9"></a>
## [AI 内存需求推动消费电子涨价](https://davidoks.blog/p/ai-is-killing-the-cheap-smartphone) ⭐️ 8.0/10

人工智能对高带宽存储器（HBM）的需求激增，正在挤占 DRAM 晶圆产能，导致 PC 和智能手机所用的 DDR 及 LPDDR 内存短缺，从而推高消费电子产品的价格。 这一涨价现象影响了笔记本电脑和手机等日常设备的可负担性，同时凸显了 AI 基础设施投资与消费硬件成本之间日益增长的矛盾，也彰显了内存制造产能的战略重要性。 文章指出，建造一座现代 DRAM 晶圆厂耗资 150 亿至 200 亿美元，且需数年时间才能达到盈利良率。HBM 采用 3D 堆叠 DRAM 芯片，每 GB 所需的晶圆面积大于传统 DRAM。

hackernews · d0ks · May 21, 21:55 · [社区讨论](https://news.ycombinator.com/item?id=48229319)

**背景**: DRAM 是一种用于电脑和手机的易失性存储器。HBM 是高带宽、3D 堆叠的变体，用于 AI 加速器。由于 HBM 与其他 DRAM 类型共享相同的晶圆制造工艺，HBM 产量增加会减少 DDR 和 LPDDR 的产能，从而推高价格。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://www.rambus.com/blogs/hbm3-everything-you-need-to-know/">High Bandwidth Memory (HBM): Everything You Need to Know - Rambus</a></li>
<li><a href="https://newsroom.lamresearch.com/high-bandwidth-memory-explained-semi-101?blog=true">High Bandwidth Memory (HBM) Explained</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，主要内存厂商专注于 HBM，可能助推中国竞争对手如长鑫存储（CXMT）和长江存储（YMTC）的发展，它们计划 IPO 并可能在 2027-2028 年增加产能，从而降低价格。另有评论者称赞文章对内存市场动态的深入解释。

**标签**: `#memory`, `#DRAM`, `#AI`, `#semiconductors`, `#hardware`

---

<a id="item-10"></a>
## [FTC 对 Cox Media Group 罚款 100 万美元，因虚假'主动监听'AI 广告](https://simonwillison.net/2026/May/22/ftc-active-listening/#atom-everything) ⭐️ 8.0/10

FTC 要求 Cox Media Group、MindSift 和 1010 Digital Works 支付近 100 万美元，以和解他们欺骗客户的指控。他们声称'主动监听'AI 服务能通过监听电话对话来定向投放广告，但实际上只是转售电子邮件列表。 这一执法行动为 AI 驱动的广告中的问责制树立了先例，警告公司如果对 AI 能力做出虚假宣称将受到处罚。它还强调，不能通过模糊的服务条款绕过消费者的隐私。 FTC 还指控这些公司错误地声称消费者通过应用服务条款选择了该服务，而这种做法不足以构成对这种侵入性数据收集的充分同意。

rss · Simon Willison · May 22, 04:48

**背景**: “主动监听”的谣言已经流传多年，许多人相信智能设备会监听对话以投放定向广告。尽管缺乏技术证据，公司利用这种恐惧销售营销服务。FTC 的行动证实，这类服务在技术上并不可行，通常只是基于转售的数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.business-standard.com/technology/tech-news/is-your-phone-listening-marketing-firm-confirms-tech-behind-targeted-ads-124090400592_1.html">Is your phone listening ? Marketing firm confirms... - Business Standard</a></li>
<li><a href="https://www.404media.co/mindsift-brags-about-using-smart-device-microphone-audio-to-target-ads-on-their-podcast/">Company Brags About Using Smart Device Microphone Audio to...</a></li>

</ul>
</details>

**标签**: `#FTC`, `#privacy`, `#AI marketing`, `#deceptive practices`, `#regulation`

---

<a id="item-11"></a>
## [字节跳动开源 3B 多模态模型 Lance](https://mp.weixin.qq.com/s/Xbfq72cr1796RZxJIs3L1A) ⭐️ 8.0/10

字节跳动发布了 Lance，一个 3B 参数的统一多模态模型，可同时处理图像/视频理解与生成，并以 Apache 2.0 许可证开源。 Lance 证明了相对较小的 3B 模型在理解与生成任务上都能取得有竞争力的表现，可能降低多模态 AI 研究和应用的门槛。 Lance 采用双流专家架构与共享上下文，分别使用 Qwen2.5-VL 处理理解和 Wan2.2 处理生成任务，并通过模态感知位置编码解决序列边界混淆。

telegram · zaihuapd · May 22, 06:40

**背景**: 大多数多模态模型专精于理解（如图像描述）或生成（如文生图），但很少两者兼得。Lance 通过分离的专家编码器和共享上下文来统一这些能力，这是一种平衡效率与性能的新颖设计。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/388960284">多模态之ViLBERT：双流网络，各自为王 - 知乎</a></li>
<li><a href="https://kexue.fm/archives/10352">“闭门造车”之多模态思路浅谈（三）：位置编码 - 科学空间|Scientific Spaces</a></li>

</ul>
</details>

**标签**: `#multimodal AI`, `#open source`, `#model release`, `#computer vision`, `#generative AI`

---

<a id="item-12"></a>
## [中国八部门整治非法跨境证券，拉勾网破产重整](https://mp.weixin.qq.com/s?__biz=MzA4NzAzMDgwMw==&amp;mid=2651090403&amp;idx=3&amp;sn=bca72a940ac72bef356f29b5b9576ac1&amp;chksm=8a1670281e2bc67d2df3608a313ba9fdaf0fcd2f43ce44475c6bf273b386af2e4f9d8e8e2e2b&amp;scene=0&amp;xtrack=1) ⭐️ 8.0/10

中国八部门联合印发整治方案，严厉打击非法跨境证券期货基金经营，仅允许存量投资者单向卖出并转出资金。证监会已对老虎证券、富途证券、长桥证券等机构非法跨境展业立案调查，同时互联网招聘平台拉勾网已进入破产重整程序。 此次监管行动对跨境投资平台及其用户产生重大影响，可能重塑中国境外投资准入的格局。拉勾网的破产反映了招聘行业向 AI 驱动的移动直聊模式快速转型，传统垂直平台面临严峻挑战。 整治方案设定两年集中整治期清理存量业务，期满后相关境内网站、交易软件和配套服务器须全面关停。证监会拟没收被调查机构全部违法所得并严厉处罚。拉勾网运营主体于 2026 年 5 月 15 日申请破产重整，其 APP 已从应用商店下架。

telegram · zaihuapd · May 22, 08:26

**背景**: 港股通、QDII（合格境内机构投资者）和跨境理财通等合规渠道允许中国投资者合法投资境外市场。拉勾网成立于 2013 年，曾是互联网招聘领域的独角兽公司，2017 年前程无忧以 1.2 亿美元收购其 60%股权。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.swhyhk.com/tc/cross-boundary/">申萬宏源（香港）有限公司 - 粵港澳大灣區 跨 境 理 財 通</a></li>
<li><a href="https://en.wikipedia.org/wiki/QDII">QDII</a></li>

</ul>
</details>

**标签**: `#金融监管`, `#跨境证券`, `#平台治理`, `#互联网招聘`, `#破产`

---

<a id="item-13"></a>
## [Cloudflare 因修复 Next.js 漏洞导致全球网络中断](https://t.me/zaihuapd/41527) ⭐️ 8.0/10

2025 年 12 月 5 日，Cloudflare 全球网络发生 25 分钟中断，影响 28%的 HTTP 流量，原因是部署了一个有缺陷的 WAF 规则，旨在修补 CVE-2025-55182——这是一个影响 React Server Components 和 Next.js 的严重远程代码执行漏洞。 此次事件凸显了安全补丁与复杂系统交互时互联网基础设施的脆弱性，并强调了 WAF 规则严格测试的关键重要性。它影响了数百万依赖 Cloudflare 提供 CDN 和安全保护的网站。 本次中断主要影响使用旧版 FL1 代理并部署了 Cloudflare 托管规则集的客户。有缺陷的修复试图阻止 CVE-2025-55182，但无意中导致控制平面过载，引发全球服务降级 25 分钟。

telegram · zaihuapd · May 22, 16:15

**背景**: CVE-2025-55182 是 React Server Components 中的一个严重预认证远程代码执行漏洞，影响 Next.js 等框架。该漏洞于 2025 年 12 月 3 日由 Meta 和 Vercel 披露。Cloudflare 试图在上游补丁广泛部署之前通过 WAF 规则缓解该漏洞，但该规则触发了一连串故障。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.microsoft.com/en-us/security/blog/2025/12/15/defending-against-the-cve-2025-55182-react2shell-vulnerability-in-react-server-components/">Defending against the CVE-2025-55182 (React2Shell) vulnerability in React Server Components | Microsoft Security Blog</a></li>
<li><a href="https://www.cve.org/CVERecord?id=CVE-2025-55182">CVE Record: CVE-2025-55182</a></li>
<li><a href="https://cloud.google.com/blog/products/identity-security/responding-to-cve-2025-55182">Responding to CVE-2025-55182 | Google Cloud Blog</a></li>

</ul>
</details>

**标签**: `#cloudflare`, `#outage`, `#security`, `#cve`, `#waf`

---