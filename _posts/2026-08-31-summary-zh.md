---
layout: default
title: "Horizon Summary: 2026-08-31 (ZH)"
date: 2026-08-31
lang: zh
---

> From 29 items, 8 important content pieces were selected

---

1. [索尼音乐等起诉 Anthropic，用盗版内容训练 Claude](#item-1) ⭐️ 9.0/10
2. [Kernel.org 的 Anubis 反机器人系统引发社区尖锐批评](#item-2) ⭐️ 8.0/10
3. [QubesOS 严重漏洞：通过复制到 VM 的错误报告可执行任意代码](#item-3) ⭐️ 8.0/10
4. [Omarchy 漏洞允许任意用户进程提权至 root](#item-4) ⭐️ 8.0/10
5. [西蒙·威利森解析 ChatGPT Work 的双重产品形态](#item-5) ⭐️ 8.0/10
6. [腾讯发布 Hy4 预览：770B 参数开源权重大模型](#item-6) ⭐️ 8.0/10
7. [苹果发布 M6 与 M5 Ultra 芯片，采用 2 纳米制程与四芯片架构](#item-7) ⭐️ 8.0/10
8. [Claude 共享链接遭 Google 索引，用户敏感数据被公开](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [索尼音乐等起诉 Anthropic，用盗版内容训练 Claude](https://www.musicbusinessworldwide.com/files/2026/08/COMPLAINT-in-Sony_Music_Publishing_US_LLC_e.pdf) ⭐️ 9.0/10

索尼音乐出版、华纳查佩尔音乐等多家公司在美国加州联邦法院起诉 Anthropic 及其创始人，指控其使用从 LibGen、PiLiMi 等盗版库非法下载的逾 700 万本书籍以及抓取的歌词来训练 Claude 模型，并删除歌词的版权管理信息。原告要求每件作品最高 15 万美元的赔偿并获得永久禁令，还指出此前类似诉讼已促成 15 亿美元和解。 这起诉讼是对 Anthropic 乃至整个人工智能行业的重大法律挑战，或将为“AI 训练使用受版权保护作品”确立先例。若 Anthropic 败诉，其可能面临巨额赔偿，并迫使 AI 公司彻底改变训练数据的获取方式，对音乐出版、图书出版及生成式 AI 领域都将产生深远影响。 值得特别关注的是，诉状指控 Anthropic 在抓取歌词时删除了版权管理信息（CMI），这违反了美国《数字千年版权法》第 1202 条，构成独立的违法行为。被告包括 Anthropic 及其创始人，诉状明确提及使用了 LibGen 和 PiLiMi（Pirate Library Mirror）等影子图书馆；PiLiMi 此前曾公开承认“在大多数国家故意违反版权法”。

telegram · zaihuapd · Aug 30, 01:00

**背景**: LibGen（Library Genesis）是一个影子图书馆项目，免费提供被付费墙限制的学术文章和书籍，但通常未经授权，出版商曾指控其构成网络盗版。PiLiMi（Pirate Library Mirror）是匿名镜像影子图书馆的项目，并承认故意违反版权法。《数字千年版权法》第 1202 条保护“版权管理信息”（如标题、作者、版权声明），移除或篡改此类信息属于违法行为。这起诉讼是作家、艺术家和出版商针对 AI 公司未经授权使用受版权保护内容进行训练而提起的又一起案件，此类法律纠纷正日益增多。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LibGen">LibGen</a></li>
<li><a href="https://en.wikipedia.org/wiki/Anna's_Archive">Anna's Archive - Wikipedia</a></li>
<li><a href="https://www.law.cornell.edu/uscode/text/17/1202">17 U.S. Code § 1202 - Integrity of copyright management information</a></li>

</ul>
</details>

**标签**: `#AI`, `#copyright`, `#legal`, `#Anthropic`, `#music`

---

<a id="item-2"></a>
## [Kernel.org 的 Anubis 反机器人系统引发社区尖锐批评](https://people.kernel.org/monsieuricon/creepy-crawlies) ⭐️ 8.0/10

kernel.org 团队在博客文章《Creepy Crawlies》中为其使用 Anubis 工作量证明反机器人系统防御 AI 爬虫的行为进行了辩护，但社区回复却暴露出严重的可用性问题。有评论者称，Anubis 难度等级 6 几乎让移动设备无法访问，而专家则指出工作量证明机制本质上更有利于机器人运营者而非人类用户。 由于 kernel.org 托管着 Linux 内核的权威 git 仓库，若反机器人措施妨碍了合法用户，反而会伤害其本欲保护的开源社区。这场争论也映射出整个行业在阻止 AI 爬虫的同时，避免对移动端和低资源用户造成附带伤害的普遍困境。 Anubis 采用基于哈希的工作量证明挑战，目前已部署在 kernel.org、lists.ffmpeg.org 等自由软件站点上。据报道，kernel.org 需消耗 14 个 CPU 核心来应对 AI 爬虫请求，评论者还指出 cgit 的参数化 URL 会生成数十亿个爬虫可见的链接。

hackernews · zdw · Aug 29, 17:49 · [社区讨论](https://news.ycombinator.com/item?id=49491791)

**背景**: Anubis 是一种开源“Web AI 防火墙”，它要求访问者在浏览页面前先解决一道工作量证明挑战，以此阻止脚本化抓取。工作量证明系统迫使客户端消耗计算资源，意图使批量爬行对机器人而言成本高昂。然而，低算力的移动设备在解同一道题时可能疲于应付，而高明的机器人运营者则可以利用更快的硬件或住宅代理绕过这一成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anubis_(software)">Anubis (software) - Wikipedia</a></li>
<li><a href="https://elsolitario.org/en/2026/08/30/kernel-org-ai-bots-anubis-cpu/">Kernel.org Burns 14 CPU Cores Tracking AI Crawlers</a></li>
<li><a href="https://github.com/TecharoHQ/anubis">Anubis - GitHub</a></li>

</ul>
</details>

**社区讨论**: 评论者对加强反机器人措施与批评工作量证明形成了两派。Semiquaver 称 Anubis 在难度 6 下对移动端“不可用”，而 robotmay 更倾向于用基于 LLM 的蜜罐陷阱而非 PoW 来浪费爬虫资源。Mzajc 则认为这是必要的，因为机器人在疯狂访问 cgit 服务器；tptacek 则复述了 Tavis Ormandy 一年前的批评：对爬虫而言每次请求都是有产出的，因此 PoW 并非良策。

**标签**: `#anti-bot`, `#proof-of-work`, `#web scraping`, `#kernel.org`, `#infrastructure`

---

<a id="item-3"></a>
## [QubesOS 严重漏洞：通过复制到 VM 的错误报告可执行任意代码](https://www.qubes-os.org/news/2026/08/29/qsb-118/) ⭐️ 8.0/10

QubesOS 于 2026 年 8 月 29 日发布了 QSB-118 安全公告，描述了 Dom0 中“复制到 VM”错误报告回传通道的严重漏洞。当从 Dom0 使用 qvm-copy-to-vm 时，恶意 qube 可向 Dom0 注入任意命令。 该漏洞破坏了 QubesOS 的核心安全边界，使被攻陷或恶意的 VM 可能通过 Dom0 接管整个系统。它凸显了即使高度关注安全的系统仍存在攻击面，并成为安全操作系统设计的重要案例。 qvm-copy-to-vm 的 VM 变体不受影响，因为其错误报告函数不使用 system()。该攻击需要用户从 Dom0 向恶意 qube 复制文件，因此并非远程攻击，但一旦执行该操作，就无需进一步用户交互。

hackernews · vntok · Aug 30, 08:51 · [社区讨论](https://news.ycombinator.com/item?id=49496918)

**背景**: QubesOS 是一款以安全为核心的桌面操作系统，使用 Xen 虚拟机监视器将应用程序和任务隔离到不同的虚拟机（qube）中。Dom0 是特权管理域，控制所有其他 qube，而 qvm-copy-to-vm 是用于在 qube 间复制文件的命令行工具。Dom0 中的错误报告回传通道以不安全的方式调用了 system()，使恶意 qube 能够注入命令。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.qubes-os.org/news/2026/08/29/qsb-118/">QSB-118: Dom0 arbitrary code execution in qvm-copy-to-vm error reporting | Qubes OS</a></li>
<li><a href="https://news.ycombinator.com/item?id=49496918">Arbitrary code execution in QubesOS via copy-to-VM error reporting backchannel | Hacker News</a></li>
<li><a href="http://www.mail-archive.com/qubes-users@googlegroups.com/msg39111.html">[qubes-users] QSB-118: Dom0 arbitrary code execution in qvm-copy-to-vm error reporting</a></li>

</ul>
</details>

**社区讨论**: 社区成员普遍承认该漏洞严重，但也指出攻击面有限，因为 Dom0 不应被用于日常工作或不可信操作。有人评论了创始人 Joanna Rutkowska 离开后项目的演变，还有用户质疑 QubesOS 是否比 BSD jail 更安全；回应强调了不同的安全模型以及 QubesOS 在隔离方面的优势。

**标签**: `#security`, `#qubes`, `#vulnerability`, `#arbitrary code execution`, `#operating systems`

---

<a id="item-4"></a>
## [Omarchy 漏洞允许任意用户进程提权至 root](https://0xcc.io/posts/omarchy-root-creds/) ⭐️ 8.0/10

一名安全研究员公开了基于 Arch 的 Linux 发行版 Omarchy 存在默认 Docker 配置缺陷，任何用户进程无需密码或 sudo 提示即可提权至 root。该问题已在 Omarchy 4.0.1 中修复。 由于 Omarchy 被宣传为一款现代且理念鲜明的桌面操作系统，此缺陷削弱了人们对那些重便利轻加固的发行版的信任，尤其是与 AI 辅助开发相关的发行版。它还凸显了炒作驱动和“vibe 编码”软件的更广泛安全风险，促使用户反思是否应信任新的发行版。 该漏洞源于 Omarchy 的默认 Docker 配置，它实际上使用户桌面会话中的每个程序都无需密码、sudo 或权限提示即可获得 root 权限。用户被敦促更新到 4.0.1，该版本移除了危险的默认配置。

hackernews · trap0xcc · Aug 30, 15:59 · [社区讨论](https://news.ycombinator.com/item?id=49499854)

**背景**: Omarchy 是由 37signals 创始人 DHH（David Heinemeier Hansson）创建的、基于 Arch Linux 的、理念鲜明的发行版，旨在提供美观实用的桌面操作系统。它部分通过网红炒作获得关注，导致一些安全观察人士警告不要使用可能缺乏严格审查的“vibe 编码”发行版。此外，Linux 桌面环境通常缺乏与 macOS 相当的、可靠的按应用沙箱机制，这使得提权问题尤为严重。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://0xcc.io/posts/omarchy-root-creds/">Omarchy : Any User Process Can Escalate to Root</a></li>
<li><a href="https://cyberpanel.net/blog/omarchy-linux-guide">Omarchy Linux : What Is It and Is It Worth Trying? 5 Min Read</a></li>
<li><a href="https://github.com/basecamp/omarchy">GitHub - basecamp/ omarchy : Beautiful, Modern & Opinionated Linux</a></li>

</ul>
</details>

**社区讨论**: 社区评论大多持怀疑和警示态度。一些人认为不应信任“vibe 编码”的发行版，并指出此前 Omarchy 曾出现 USB 描述符直接流入 shell 的漏洞。另一些人建议坚持使用 Ubuntu 等主流发行版，或使用 archinstall 而不是被炒作的衍生版；还有不少人指出 Linux 桌面沙箱机制薄弱，因此即使没有 root 权限，恶意进程也已经能造成严重危害。

**标签**: `#security`, `#vulnerability`, `#linux`, `#privilege-escalation`, `#distro`

---

<a id="item-5"></a>
## [西蒙·威利森解析 ChatGPT Work 的双重产品形态](https://simonwillison.net/2026/Aug/30/understanding-chatgpt-work/) ⭐️ 8.0/10

西蒙·威利森指出，OpenAI 的 ChatGPT Work 实际上包含两个不同的产品：云端版本（Work Cloud）和本地桌面应用（Work Local，前身为 Codex），并详细介绍了云端版本独有的功能，如模型选择、持久化文件系统和无头浏览器。 这一澄清帮助用户和开发者理解该使用哪种 ChatGPT Work 产品，降低了对一个功能强大但描述不清的产品的困惑。它也凸显了 OpenAI 如何针对不同用户需求和订阅等级来细分其 AI 产品。 Work Cloud 提供 GPT-5.6 Sol、Luna 和 Terra 模型，推理级别从 Light 到 Ultra，以及 GPT-5.5；而 Chat 提供不同的选择，包括 5.6 Instant 和 Pro，其中更高的推理级别仅限每月 100 美元以上的订阅用户使用。Work 仅向每月 20 美元及以上的订阅用户提供，Work Cloud 还包括可访问互联网的代码执行环境、无头 Chrome 浏览器、持久化共享文件系统、ChatGPT Sites 发布、子代理和定时提示自动化。

rss · Simon Willison · Aug 30, 23:59

**背景**: ChatGPT Work 是 OpenAI 推出的产品，旨在帮助用户完成有明确结果的重大任务，如创建简报、演示文稿、分析和工作流。它基于 OpenAI 的 Codex——一个可以编写代码和修复 bug 的 AI 编程代理，Codex 于 2025 年 4 月以 Codex CLI 形式发布，可通过 ChatGPT 和桌面应用使用。名为 Sol、Luna 和 Terra 的 GPT-5.6 模型似乎与 OpenAI API 中提供的模型相同，每种模型都有不同的能力和推理级别。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_Codex_(AI_agent)">OpenAI Codex (AI agent) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#ChatGPT`, `#OpenAI`, `#AI tools`, `#product analysis`, `#Simon Willison`

---

<a id="item-6"></a>
## [腾讯发布 Hy4 预览：770B 参数开源权重大模型](https://simonwillison.net/2026/Aug/29/hy4/) ⭐️ 8.0/10

腾讯发布了 Hy4 Preview，这是一款新的开源权重纯文本大语言模型，总参数 770B（激活 49B），上下文窗口达 100 万 token。模型权重总量 1.56TB，已在 Hugging Face 上开放下载。 这是腾讯上一代 Hy3 模型的重大升级，总参数接近三倍，上下文窗口扩大至四倍。这表明开放权重前沿模型的竞争正在加剧，让开发者能使用一款百万级上下文窗口的超大规模 MoE 风格模型。 Hy4 的聊天模板显示其推理强度分为 'high'（默认）和 'no_think'（禁用推理）两档。该模型仅支持文本输入，不具备视觉能力。Simon Willison 的测试发现其推理轨迹使用截断的英文表达，可能是为了节省 token。

rss · Simon Willison · Aug 29, 23:53

**背景**: Hy4 很可能采用混合专家（MoE）架构，因为其总参数（770B）与激活参数（49B）差距很大。MoE 模型每次只激活一部分参数，从而提高效率。开放权重模型公开训练后的权重，但不一定公开训练数据或具备完整开源许可，这是 AI 社区中的一个重要区别。100 万 token 的上下文窗口使模型可以一次性处理整个代码库或长文档。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://www.mindstudio.ai/blog/claude-1m-token-context-window-ai-agents">Claude 1M Token Context Window: What It Means for AI Agents and Long-Running Tasks | MindStudio</a></li>
<li><a href="https://deasadiqbal.medium.com/understanding-open-weights-vs-open-source-models-988b50ce64d7">Understanding Open Weights vs. Open Source Models | by Asad Iqbal | Medium</a></li>

</ul>
</details>

**标签**: `#LLM`, `#Tencent`, `#open-source`, `#AI`, `#Hugging Face`

---

<a id="item-7"></a>
## [苹果发布 M6 与 M5 Ultra 芯片，采用 2 纳米制程与四芯片架构](https://t.me/zaihuapd/43505) ⭐️ 8.0/10

苹果发布了 M6 与 M5 Ultra 芯片。M6 是苹果首款 2 纳米制程芯片，配备 12 核 CPU、12 核 GPU 和双 16 核神经网络引擎，统一内存带宽最高 170GB/s；M5 Ultra 采用四芯片架构，最高 36 核 CPU、80 核 GPU，支持 512GB 内存，带宽达 1.2TB/s。 这标志着苹果首次采用 2 纳米制程，以及 M 系列首个四芯片架构设计，为 AI 和专业工作负载带来显著的性能与内存带宽提升。此举进一步巩固了 Apple Silicon 在 PC 芯片领域的竞争力。 M5 Ultra 通过新一代 UltraFusion 技术连接两个双芯片 M5 Max，使四个芯片作为一个统一处理器运行。此外，苹果在 M5 和 M6 家族的每个 GPU 核心中集成了专用神经加速器，以提升端侧 AI 性能。

telegram · zaihuapd · Aug 30, 16:41

**背景**: 2 纳米制程是半导体制造工艺的最新节点，可带来更高的晶体管密度与能效。在 Apple Silicon 中，统一内存是 CPU、GPU 和神经网络引擎共享的高速内存池，避免了传统 PC 中系统内存与显存分离的问题。M6 的 170GB/s 和 M5 Ultra 的 1.2TB/s 带宽可让大型 AI 模型在本地运行，无需在内存池之间复制数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/2_nm_process">2 nm process - Wikipedia</a></li>
<li><a href="https://au.pcmag.com/processors/119512/apple-m5-ultra-and-m6-silicon-explained">Apple M5 Ultra and M6 Silicon Explained: 2nm Tech, Quad - Die Chips...</a></li>
<li><a href="https://www.hoxtonmacs.co.uk/blogs/news/what-is-unified-memory">What is Unified Memory – Hoxton Macs</a></li>

</ul>
</details>

**标签**: `#Apple`, `#chip design`, `#M6`, `#M5 Ultra`, `#hardware`

---

<a id="item-8"></a>
## [Claude 共享链接遭 Google 索引，用户敏感数据被公开](https://t.me/zaihuapd/43511) ⭐️ 8.0/10

Claude 的共享对话功能存在隐私漏洞：生成的公开链接未设置 noindex 标签，导致 Google 等搜索引擎收录这些页面，使 API 密钥、加密货币钱包、简历、律师咨询记录、公司内部资料及社会安全号码等敏感信息被公开索引。Anthropic 目前尚未修复此问题，而约一年前 ChatGPT 也出现过同类问题并迅速解决。 这是一项严重的隐私漏洞：被索引的页面会让敏感数据通过搜索引擎被永久公开检索，影响所有使用过共享功能的 Claude 用户。该问题削弱了用户对 AI 助手的信任，也暴露出 AI 聊天机器人领域反复出现的安全隐患。 根本原因在于 Claude 共享对话页面缺少 noindex 元标签（或 X-Robots-Tag），导致搜索引擎爬虫可以收录这些页面。泄露的数据据称包括 API 密钥、加密货币钱包、个人简历、律师咨询记录、公司内部项目资料和社会安全号码；建议用户前往「设置 → 共享对话」页面手动删除涉及隐私的聊天记录。

telegram · zaihuapd · Aug 31, 03:22

**背景**: Claude 是 Anthropic 公司开发的一系列大语言模型，于 2023 年 3 月以 AI 聊天机器人形式首次发布。noindex 指令是一种 HTML meta 标签（或 HTTP 响应头），用来告诉搜索引擎不要把页面纳入搜索结果；若缺少该指令，共享链接就可能被索引。约一年前，ChatGPT 的共享链接也曾出现类似隐私问题，当时得到了快速修复。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_(AI)">Claude (AI)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Noindex">noindex - Wikipedia</a></li>
<li><a href="https://developers.google.com/search/docs/crawling-indexing/block-indexing">Block Search Indexing with noindex | Google Search Central ...</a></li>

</ul>
</details>

**标签**: `#privacy`, `#security`, `#claude`, `#vulnerability`, `#data-leak`

---