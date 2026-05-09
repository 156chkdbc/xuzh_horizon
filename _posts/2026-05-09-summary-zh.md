---
layout: default
title: "Horizon Summary: 2026-05-09 (ZH)"
date: 2026-05-09
lang: zh
---

> From 37 items, 13 important content pieces were selected

---

1. [Mozilla 使用 Claude Mythos 发现数百个 Firefox 漏洞](#item-1) ⭐️ 9.0/10
2. [Triton 3.7.0 发布：新增张量操作与 FP8 支持](#item-2) ⭐️ 8.0/10
3. [Google 新版 reCAPTCHA 实行远程证明，阻碍去 Google 化安卓用户](#item-3) ⭐️ 8.0/10
4. [人工智能打破两种漏洞披露文化](#item-4) ⭐️ 8.0/10
5. [Meta 停止 Instagram 私信端到端加密](#item-5) ⭐️ 8.0/10
6. [Mojo 1.0 Beta 发布：兼容 Python，引入 Rust 所有权与 Zig 编译时计算](#item-6) ⭐️ 8.0/10
7. [Luke Curley 批评 WebRTC 丢包影响 LLM 提示](#item-7) ⭐️ 8.0/10
8. [Canvas LMS 遭 ShinyHunters 黑客攻击，影响美国学校期末周](#item-8) ⭐️ 8.0/10
9. [Cloudflare 裁员超 1100 人，称 AI 使用量激增 600%是关键原因](#item-9) ⭐️ 8.0/10
10. [Anthropic 拟融资数百亿美元，估值逼近万亿美元](#item-10) ⭐️ 8.0/10
11. [美国怀疑英伟达芯片经泰国走私至中国，阿里巴巴被指为终端客户](#item-11) ⭐️ 8.0/10
12. [DeepSeek 寻求 450 亿美元估值，国资或领投](#item-12) ⭐️ 8.0/10
13. [苹果或结束台积电独家代工，考虑英特尔代工部分芯片](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Mozilla 使用 Claude Mythos 发现数百个 Firefox 漏洞](https://simonwillison.net/2026/May/7/firefox-claude-mythos/#atom-everything) ⭐️ 9.0/10

Mozilla 利用 Anthropic 的 Claude Mythos 预览版在 Firefox 中定位并修复了数百个安全漏洞，2026 年 4 月修复了 423 个安全漏洞，远高于通常的每月 20-30 个。 这标志着 AI 辅助安全的范式转变，LLM 从生成无用的漏洞报告转变为产生高质量、可操作的漏洞发现，可能大幅降低开源软件加固的成本和人力。 发现的漏洞包括一个存在 20 年的 XSLT 漏洞和一个存在 15 年的 <legend> HTML 元素漏洞；许多尝试被 Firefox 的纵深防御措施阻断，突显了该模型发现细微缺陷的能力。

rss · Simon Willison · May 7, 17:56

**背景**: Claude Mythos 是 Anthropic 开发的先进 AI 模型，专为复杂的多步网络安全任务设计。此前，AI 生成的安全报告常常不正确且给维护者带来负担。Mozilla 结合了改进的模型和更优的提示技术，过滤噪声并放大信号，在漏洞检测方面取得了突破。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_(language_model)">Claude (language model) - Wikipedia</a></li>
<li><a href="https://www.bbc.com/news/articles/crk1py1jgzko">What is Anthopic's Claude Mythos and what risks does it pose?</a></li>
<li><a href="https://www.pluralsight.com/resources/blog/ai-and-data/what-is-claude-mythos">What is Claude Mythos? | Pluralsight</a></li>

</ul>
</details>

**标签**: `#AI`, `#security`, `#Firefox`, `#vulnerability detection`, `#LLM`

---

<a id="item-2"></a>
## [Triton 3.7.0 发布：新增张量操作与 FP8 支持](https://github.com/triton-lang/triton/releases/tag/v3.7.0) ⭐️ 8.0/10

Triton 3.7.0 引入了 tl.squeeze 和 tl.unsqueeze 操作、缩放批量矩阵乘法以及直接创建 FP8 常量。该版本还包括对 AMD 和 NVIDIA GPU 的后端增强。 此版本增强了 Triton 在深度学习工作负载中的表达能力，特别是针对效率日益重要的低精度 FP8 计算。新操作简化了复杂 GPU 内核的编写。 缩放 BMM 操作支持高效的批量矩阵乘法，并可选择缩放。FP8 常量允许直接使用 8 位浮点值，无需转换。后端改进包括 NVIDIA 的 2CTA 模式和 TMA 多播，以及 AMD 的多种修复。

github · atalman · May 7, 22:19

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/parca-dev/proton">GitHub - parca-dev/ proton</a></li>
<li><a href="https://en.wikipedia.org/wiki/Minifloat">Minifloat - Wikipedia</a></li>

</ul>
</details>

**标签**: `#Triton`, `#GPU compiler`, `#deep learning`, `#release`, `#open source`

---

<a id="item-3"></a>
## [Google 新版 reCAPTCHA 实行远程证明，阻碍去 Google 化安卓用户](https://reclaimthenet.org/google-broke-recaptcha-for-de-googled-android-users) ⭐️ 8.0/10

Google 新版 reCAPTCHA 实际上执行了远程证明，破坏了去 Google 化安卓用户的功能，并引发了严重的隐私担忧。 这一变化影响了选择从安卓设备上移除 Google 服务的用户，限制了他们访问许多使用 reCAPTCHA 的网站。同时，远程证明可能将设备身份与用户活动关联，引发了严重的隐私问题。 新版 reCAPTCHA 使用远程证明，涉及从烧录的私钥 (EK) 到由 Google 服务器签名的临时身份密钥 (AIK) 的信任链，可能允许 Google 跨会话关联设备身份。

hackernews · anonymousiam · May 8, 18:45 · [社区讨论](https://news.ycombinator.com/item?id=48067119)

**背景**: 远程证明是一种可信计算技术，设备通过它向远程验证者证明其完整性。在此上下文中，Google 的 reCAPTCHA 利用它来确保设备未被篡改。去 Google 化安卓指移除了 Google 服务的设备，通常运行自定义 ROM。这些设备缺乏通过远程证明所需的专有组件，因此被屏蔽。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Remote_attestation">Remote attestation</a></li>
<li><a href="https://tech.yahoo.com/phones/articles/googling-android-simpler-think-no-193119747.html">De - Googling Android is simpler than you think—no special phone...</a></li>

</ul>
</details>

**社区讨论**: 评论表达了沮丧和担忧。用户讨论远程证明的技术细节，并寻求 reCAPTCHA 的替代方案。有人认为此举强制用户进行 KYC（了解你的客户），属于过度行为。

**标签**: `#reCAPTCHA`, `#Android`, `#privacy`, `#remote attestation`, `#Google`

---

<a id="item-4"></a>
## [人工智能打破两种漏洞披露文化](https://www.jefftk.com/p/ai-is-breaking-two-vulnerability-cultures) ⭐️ 8.0/10

一项新分析指出，人工智能通过加速漏洞利用生成并扩大协调披露与公开利用之间的鸿沟，正在瓦解传统的漏洞披露规范。 这一转变可能从根本上改变漏洞报告和修补的方式，增加零日漏洞被利用的风险，并削弱协调披露的效果。 该分析以 Log4Shell 事件为基础，指出 AI 工具让攻击者生成漏洞利用代码的速度快于防御者修补的速度，对代码公开的开源软件影响尤甚。

hackernews · speckx · May 8, 17:55 · [社区讨论](https://news.ycombinator.com/item?id=48066524)

**背景**: 漏洞披露传统上存在两种主要文化：协调披露（研究人员私下通知厂商并给予修补时间）和完全披露（立即公开细节）。人工智能的兴起以及软件透明度的提升——通过开源软件的采用和先进的逆向工程工具——模糊了这一区别，因为攻击者现在可以快速地从公开的补丁或提交中生成漏洞利用代码。

**社区讨论**: 评论者普遍认为 AI 加速了已有趋势而非创造新问题，tptacek 指出软件透明度的影响早有预言。freeqaz 强调 Log4Shell 是漏洞利用与披露赛跑的关键例子。但 rikafurude21 认为更廉价的漏洞利用生成反而使协调披露更加重要。

**标签**: `#AI`, `#cybersecurity`, `#vulnerability disclosure`, `#open source`, `#Log4Shell`

---

<a id="item-5"></a>
## [Meta 停止 Instagram 私信端到端加密](https://www.pcmag.com/news/meta-shuts-down-end-to-end-encryption-for-instagram-dms-messaging) ⭐️ 8.0/10

Meta 已停止为 Instagram 私信提供端到端加密，理由是用户选择启用的人数太少。公司将转而以未加密形式存储消息。 这一决定引发了用户隐私方面的担忧，并标志着从行业加强加密的趋势倒退。批评者认为 Meta 优先考虑获取用户数据用于广告和合规，而非隐私保护。 该加密功能是选择性加入的，需要用户手动启用。Meta 声称很少用户选择开启，使得该功能不可持续。

hackernews · tcp_handshaker · May 8, 21:47 · [社区讨论](https://news.ycombinator.com/item?id=48069192)

**背景**: 端到端加密确保只有发送方和接收方能读取消息，即使是服务提供商也无法访问内容。隐私倡导者通常推动默认加密，例如 WhatsApp（也属于 Meta）和 Signal 等应用。Meta 的决定与其早前承诺在其消息平台上推广加密的做法形成对比。

**社区讨论**: 评论批评 Meta 没有将加密设为默认，并将其与 Signal 和 WhatsApp 进行不利比较。一些人认为 Meta 的举动反映了企业普遍不愿将隐私置于商业利益之上，而另一些人则对保护用户数据方面缺乏进展表示沮丧。

**标签**: `#privacy`, `#encryption`, `#Instagram`, `#Meta`, `#tech-policy`

---

<a id="item-6"></a>
## [Mojo 1.0 Beta 发布：兼容 Python，引入 Rust 所有权与 Zig 编译时计算](https://mojolang.org/) ⭐️ 8.0/10

Modular 公司发布了 Mojo 1.0 Beta，这是一种结合了 Python 语法、类似 Rust 的所有权机制和类似 Zig 的编译时计算（comptime）的编程语言，旨在用于高性能机器学习和系统编程。 Mojo 旨在弥合高级语言易用性与底层性能之间的差距，可能使 Python 开发者无需切换语言即可编写高效的系统代码。其独特地使用 MLIR 作为编译器基础设施，使其能够从单一代码库支持 CPU、GPU 和 TPU 等目标。 Mojo 目前闭源，但标准库开源，Modular 承诺将于 2026 年秋季开源。它支持一等 SIMD、丰富的类型系统，并可通过外部函数接口与 Python 互操作。

hackernews · sbt567 · May 8, 02:49 · [社区讨论](https://news.ycombinator.com/item?id=48057901)

**背景**: Mojo 构建于 MLIR（多层中间表示）之上，这是一种编译器框架，相比单独的 LLVM 能够实现更高级别的优化。这使得 Mojo 能够高效地针对包括 GPU 和 TPU 在内的多种硬件。所有权模型借鉴了 Rust，确保内存安全而无需垃圾回收；而 Zig 中的编译时执行（comptime）则实现了强大的元编程能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mojo_(programming_language)">Mojo (programming language)</a></li>
<li><a href="https://zig.guide/language-basics/comptime/">Comptime | zig .guide</a></li>

</ul>
</details>

**社区讨论**: 评论者对 Mojo 的性能以及所有权和 comptime 等功能表示兴奋，但也指出由于语法差异和有限的 Python 兼容性，Python 开发者面临挑战。一些用户还对计划于 2026 年开源表示迫不及待。

**标签**: `#programming language`, `#performance`, `#ML`, `#systems programming`, `#Mojo`

---

<a id="item-7"></a>
## [Luke Curley 批评 WebRTC 丢包影响 LLM 提示](https://simonwillison.net/2026/May/9/luke-curley/#atom-everything) ⭐️ 8.0/10

Luke Curley 指出，WebRTC 为降低延迟而丢弃音频包的设计损害了 LLM 提示的准确性，并提到浏览器甚至无法重传丢失的数据包，以 Discord 的经验为例。 这突显了实时通信优化与 AI 模型准确性要求之间的根本冲突，可能影响基于语音的 AI 交互质量。 WebRTC 在网络条件不佳时主动丢弃音频包以保持低延迟，但这可能导致音频失真；Curley 指出，为获得准确的 LLM 提示，多等 200 毫秒是更可取的。

rss · Simon Willison · May 9, 01:03

**背景**: WebRTC 是浏览器中实时通信的标准，专为视频通话等低延迟场景设计。大语言模型（LLM）处理语音提示需要准确的输入，因此丢包会带来问题。

**标签**: `#WebRTC`, `#LLM`, `#real-time communication`, `#audio`, `#latency`

---

<a id="item-8"></a>
## [Canvas LMS 遭 ShinyHunters 黑客攻击，影响美国学校期末周](https://www.cnn.com/2026/05/07/us/canvas-hack-strands-college-students-finals-week) ⭐️ 8.0/10

Instructure 旗下的 Canvas 学习管理系统遭到 ShinyHunters 黑客组织的勒索软件攻击和数据泄露，在美国学校期末周造成大范围中断。此次攻击泄露了超过 300 TB 的数据，包括学生姓名、ID 和学校邮箱，迫使部分大学重新安排考试时间。 此事件突显了关键教育基础设施的脆弱性，在高风险的学术期末影响了数千所学校和数百万学生。它强调了教育技术领域迫切需要加强网络安全措施，尤其是勒索软件组织越来越多地将目标对准敏感的学生数据。 ShinyHunters 声称对 2026 年 5 月针对 Instructure 的两起事件负责：5 月 1 日的第一起事件泄露了用户名、邮箱和学生 ID；5 月 7 日的第二起事件涉及勒索软件，导致许多用户无法访问 Canvas，据称影响近 9000 所学校或组织，窃取数据超过 300 TB。

telegram · zaihuapd · May 8, 04:30

**背景**: Canvas 是由 Instructure 开发的基于云的学习管理系统 (LMS)，广泛应用于 K-12、高等教育和企业培训，用于课程管理、测验和学生互动。ShinyHunters 是一个成立于 2019 年左右的黑帽犯罪黑客组织，以在多个行业策划数据泄露而闻名。该组织通常窃取数据并勒索赎金，威胁若不支付则泄露敏感信息。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Canvas_LMS">Canvas LMS</a></li>
<li><a href="https://en.wikipedia.org/wiki/ShinyHunters">ShinyHunters - Wikipedia</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#data breach`, `#education`, `#ransomware`, `#canvas`

---

<a id="item-9"></a>
## [Cloudflare 裁员超 1100 人，称 AI 使用量激增 600%是关键原因](https://blog.cloudflare.com/building-for-the-future/) ⭐️ 8.0/10

Cloudflare 宣布在全球范围内裁减超过 1100 名员工，并将此次重组归因于过去三个月内各部门内部 AI 智能体使用量增长超过 600%。 这表明一家关键互联网基础设施公司正转向以 AI 为驱动的劳动力重组，可能影响更广泛的科技行业就业趋势，并凸显 AI 智能体对人类岗位的替代日益加剧。 此次裁员为一次性完成，遣散方案包括：至 2026 年底的全额基本工资补偿、美国员工医疗保险延至年底、股权归属延至 2026 年 8 月 15 日，以及对未满一年归属期的员工豁免“悬崖期”条款并按比例计算股权。

telegram · zaihuapd · May 8, 08:15

**背景**: AI 智能体是能够自主执行任务、做出决策并与环境交互的软件工具，它们利用内部系统和企业工具的数据。像 Cloudflare 这样的公司正越来越多地在工程、人力资源、财务和市场等部门部署 AI 智能体来自动化日常工作，从而减少对人类员工的需求。这一趋势反映了更广泛的行业变革，即 AI 的采用直接影响了劳动力规模和结构。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/resources/articles/what-are-ai-agents">What are AI agents ? · GitHub</a></li>
<li><a href="https://www.grammarly.com/agentic-ai">What is Agentic AI ? | Agentic AI 101</a></li>

</ul>
</details>

**标签**: `#Cloudflare`, `#layoffs`, `#AI`, `#restructuring`, `#tech industry`

---

<a id="item-10"></a>
## [Anthropic 拟融资数百亿美元，估值逼近万亿美元](https://www.ft.com/content/a40cafcc-0fa4-4e70-9e24-90d826aea56d) ⭐️ 8.0/10

据报道，Anthropic 正计划在今年夏天筹集数百亿美元资金，用于扩充其算力基础设施，此举可能将其估值推高至近 1 万亿美元，超越 OpenAI。 这轮融资将成为 AI 行业的一个重要里程碑，标志着投资者信心从 OpenAI 转向 Anthropic，并凸显前沿 AI 开发对资本的巨大需求。 在 Forge Global 的二级市场上，Anthropic 的隐含估值已达到 1 万亿至 1.2 万亿美元，高于 OpenAI 约 8800 亿美元的估值。而就在今年 2 月，Anthropic 刚完成一轮 300 亿美元融资，估值 3800 亿美元。

telegram · zaihuapd · May 8, 11:15

**背景**: Anthropic 由前 OpenAI 员工创立，是一家领先的 AI 安全初创公司，与 OpenAI 直接竞争。像 Forge Global 这样的私人二级市场允许投资者交易未上市公司的股份，为初创公司的感知价值提供实时指标。估值的快速飙升反映了 Anthropic 强劲的企业客户增长以及 AI 算力资源的巨大需求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/Forge_Global">Forge Global</a></li>

</ul>
</details>

**标签**: `#AI`, `#Anthropic`, `#funding`, `#valuation`, `#startup`

---

<a id="item-11"></a>
## [美国怀疑英伟达芯片经泰国走私至中国，阿里巴巴被指为终端客户](https://www.bloomberg.com/news/articles/2026-05-08/us-said-to-suspect-nvidia-chips-smuggled-to-alibaba-via-thailand) ⭐️ 8.0/10

美国检方怀疑泰国公司 OBON Corp. 将价值 25 亿美元的 Super Micro 服务器（内含先进英伟达芯片）走私至中国，阿里巴巴集团被指为多个终端客户之一。 此案凸显了持续的美中科技紧张局势，可能导致美国加强对泰国的出口管制，从而阻碍泰国的人工智能发展并影响全球供应链。 OBON 曾参与创建泰国主权 AI 云 Siam AI，后者获得了英伟达合作伙伴地位。阿里巴巴否认与 Super Micro 或 OBON 有任何业务关系。

telegram · zaihuapd · May 8, 13:23

**背景**: 美国已对向中国出口先进英伟达芯片实施管制，以防止其用于军事领域。通过泰国等第三国的走私路线成为关注焦点，促使调查展开。Super Micro 服务器是常用于人工智能和数据中心的高性能计算系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.supermicro.com/">Supermicro Data Center Server , Blade, Data Storage, AI System</a></li>
<li><a href="https://siam.ai/">Siam ai corporation co., ltd.</a></li>

</ul>
</details>

**标签**: `#export controls`, `#Nvidia`, `#smuggling`, `#Alibaba`, `#US-China relations`

---

<a id="item-12"></a>
## [DeepSeek 寻求 450 亿美元估值，国资或领投](https://t.me/zaihuapd/41289) ⭐️ 8.0/10

据报道，DeepSeek 正在其首次大规模外部融资中寻求约 450 亿美元的估值，中国国家集成电路产业投资基金可能领投。 此轮融资将标志着国有资本深度介入中国人工智能领域，加强了政府对核心 AI 公司的支持，并显示出国家对 DeepSeek 的强力背书。 这是 DeepSeek 首次进行大规模外部融资，此前该公司完全由其母公司对冲基金 High-Flyer 出资。450 亿美元的估值将使 DeepSeek 成为中国估值最高的 AI 初创公司之一。

telegram · zaihuapd · May 8, 14:59

**背景**: DeepSeek 由 High-Flyer 联合创始人梁文锋于 2023 年 7 月创立。该公司以开发开放权重的大型语言模型而闻名，其训练成本远低于 OpenAI 等竞争对手，尽管面临美国芯片出口限制，只能使用性能较低的硬件。该公司于 2025 年 1 月发布的 R1 模型以其极低的训练成本和高性能震惊了业界。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek_(Company)">DeepSeek (Company)</a></li>
<li><a href="https://www.deepseek.com/en/">DeepSeek</a></li>

</ul>
</details>

**标签**: `#AI`, `#funding`, `#DeepSeek`, `#China`, `#semiconductor`

---

<a id="item-13"></a>
## [苹果或结束台积电独家代工，考虑英特尔代工部分芯片](https://t.me/zaihuapd/41292) ⭐️ 8.0/10

据报道，苹果正考虑结束台积电自 2014 年以来的独家芯片代工协议，最早可能在 2027 年将部分中低端芯片交由英特尔的 18A 工艺生产。 此举将多元化苹果的供应链，减少对台积电的依赖，而台积电目前正优先处理英伟达等 AI 企业的代工需求。同时，这也将为英特尔的代工业务带来重大利好。 英特尔的参与仅限于代工制造，不涉及芯片设计。苹果此举是由于台积电因 AI 芯片订单激增而产能紧张。

telegram · zaihuapd · May 8, 17:18

**背景**: 自 2014 年以来，苹果一直依赖台积电独家代工其自研的 A 系列和 M 系列芯片。苹果自行设计芯片，但将制造外包。转向英特尔将是半导体供应链的重大变化，可能挑战台积电的主导地位。

**标签**: `#Apple`, `#TSMC`, `#Intel`, `#chip manufacturing`, `#supply chain`

---