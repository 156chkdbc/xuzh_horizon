---
layout: default
title: "Horizon Summary: 2026-05-08 (ZH)"
date: 2026-05-08
lang: zh
---

> From 41 items, 13 important content pieces were selected

---

1. [Dirty Frag: 影响所有主流 Linux 发行版的严重内核提权漏洞](#item-1) ⭐️ 10.0/10
2. [Canvas LMS 因勒索软件攻击在期末考试期间瘫痪](#item-2) ⭐️ 9.0/10
3. [DeepMind AlphaEvolve：Gemini 驱动的编码智能体跨领域扩展](#item-3) ⭐️ 9.0/10
4. [Mozilla 用 Claude Mythos 预览版强化 Firefox 安全](#item-4) ⭐️ 9.0/10
5. [Anthropic 与 SpaceX 达成算力合作，提升 Claude 容量](#item-5) ⭐️ 9.0/10
6. [小米开源 OmniVoice：支持 646 语种的语音克隆 TTS 模型](#item-6) ⭐️ 9.0/10
7. [Triton v3.7.0 发布：新增 scaled BMM、FP8 常量等操作](#item-7) ⭐️ 8.0/10
8. [智能体需要控制流，而非更多提示](#item-8) ⭐️ 8.0/10
9. [Cloudflare 裁员 20%，美其名曰‘建设未来’](#item-9) ⭐️ 8.0/10
10. [Anthropic 开源自然语言自编码器，推动 AI 可解释性](#item-10) ⭐️ 8.0/10
11. [AI 垃圾内容威胁在线社区真实性](#item-11) ⭐️ 8.0/10
12. [Chrome 删除设备端 AI 隐私承诺](#item-12) ⭐️ 8.0/10
13. [Anthropic Code w/ Claude 2026 主题演讲直播](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Dirty Frag: 影响所有主流 Linux 发行版的严重内核提权漏洞](https://github.com/V4bel/dirtyfrag) ⭐️ 10.0/10

2026 年 5 月 7 日，韩国安全研究员 Hyunwoo Kim 公开披露了名为 Dirty Frag 的 Linux 内核本地提权漏洞。该漏洞利用 IPsec ESP 和 RxRPC 两个模块的漏洞链式组合，可在所有主流发行版上获得 root 权限，目前尚无补丁。 该漏洞影响 Ubuntu、RHEL 和 Fedora 等所有主流 Linux 发行版，允许任何本地非特权用户无需认证即可获取 root 权限。由于披露流程被破坏且尚无补丁，数百万系统面临风险，直至各发行版完成补丁回溯移植。 Dirty Frag 属于与 Dirty Pipe 和 Copy Fail 相同的漏洞类别，利用零拷贝 splice()路径写入只读页缓存。该漏洞提供两种变体：一种利用存在约 9 年的 IPsec ESP 模块（需用户命名空间权限），另一种利用 2023 年引入的 RxRPC 模块（无需特殊权限），从而使攻击可在几乎所有发行版上通用。

telegram · zaihuapd · May 7, 23:07

**背景**: Linux 内核的页缓存对于只读文件描述符通常是只读的。splice()系统调用允许在不拷贝的情况下在文件描述符间移动数据，但在某些代码路径中，它可能将只读页面钉入套接字缓冲区，随后被就地修改，导致只读内存被写入。此类漏洞包括 Dirty Pipe（CVE-2022-0847）和 Copy Fail。IPsec ESP 和 RxRPC 模块是内核子系统，默认情况下大多数发行版会加载这些模块，即使系统并未使用对应协议。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/V4bel/dirtyfrag">GitHub - V4bel/dirtyfrag · GitHub</a></li>
<li><a href="https://blog.cloudlinux.com/dirty-frag-mitigation-and-kernel-update">Dirty Frag [CVE Pending]: Mitigation and Kernel Update on CloudLinux</a></li>
<li><a href="https://www.cyberkendra.com/2026/05/dirty-frag-no-patch-no-warning-root.html">Dirty Frag — No Patch, No Warning — Root Access on Every Major Linux Distro - Cyber Kendra</a></li>

</ul>
</details>

**社区讨论**: 社区评论对披露流程表示不满，并批评发行版默认启用罕用模块。有评论指出该漏洞与 Copy Fail 相似，认为根本原因早已明确但未得到正确修复。整体舆论对内核维护者和发行版的安全实践持批评态度。

**标签**: `#Linux kernel`, `#security`, `#privilege escalation`, `#vulnerability`, `#CVE`

---

<a id="item-2"></a>
## [Canvas LMS 因勒索软件攻击在期末考试期间瘫痪](https://www.theverge.com/tech/926458/canvas-shinyhunters-breach) ⭐️ 9.0/10

由 Instructure 公司开发的 Canvas 学习管理系统因持续勒索软件攻击而瘫痪，在期末考试周对大学造成重大干扰。 此次攻击突显了关键教育基础设施的脆弱性以及安全失效时的严重后果，尤其是在学术高峰期。它强调了制定稳健应急预案和离线备份的必要性。 此次攻击归因于 ShinyHunters 组织，扰乱了许多学生的期末考试。Canvas 并未正式确认勒索软件攻击，而是将其标记为'计划维护'。

hackernews · stefanpie · May 7, 22:22 · [社区讨论](https://news.ycombinator.com/item?id=48055913)

**背景**: 类似 Canvas 的学习管理系统(LMS)被大学用于托管课程资料、作业和考试。勒索软件是一种加密文件并要求支付赎金的恶意软件。Canvas 缺乏离线备份和沟通不畅使情况恶化。

**社区讨论**: 评论者表达了对 Canvas 缺乏沟通和透明度的沮丧，有人称此次攻击为'一团糟'。有人担心数据泄露会暴露学生成绩和个人信息。一位评论者指出，利用链本身并不新颖，但武器化速度令人担忧。

**标签**: `#security`, `#ransomware`, `#canvas`, `#education`, `#incident`

---

<a id="item-3"></a>
## [DeepMind AlphaEvolve：Gemini 驱动的编码智能体跨领域扩展](https://deepmind.google/blog/alphaevolve-impact/) ⭐️ 9.0/10

Google DeepMind 发布了 AlphaEvolve，这是一个由 Gemini 驱动的进化编码智能体，能够设计高级算法并解决数学和计算领域的问题。它甚至可以优化自身的训练和硬件，标志着向自我改进 AI 迈进了一步。 AlphaEvolve 代表着 AI 自我改进领域的重大突破，可能加速科学发现和算法设计。它也凸显了 DeepMind 对基础研究的关注，与优先发展商业编码助手的其他 AI 公司形成对比。 AlphaEvolve 将进化算法与大型语言模型相结合，自主生成和优化算法。它已成功解决了具有挑战性的数学问题，包括一些 Paul Erdős 未解决的问题。

hackernews · berlianta · May 7, 15:02 · [社区讨论](https://news.ycombinator.com/item?id=48050278)

**背景**: 像 Gemini 这样的大型语言模型可以生成代码，但通常需要人类指导。进化算法模拟自然选择来搜索最优解。AlphaEvolve 融合了这些技术，创建了一个自我改进的编码智能体，可以在无需人工干预的情况下进化算法，可能彻底改变复杂问题的解决方式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AlphaEvolve">AlphaEvolve - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者强调了 AI 自我改进的潜力，其中一位指出用户中存在两种极端：一些人认为它极其有用，另一些人则不屑一顾。另一位指出 DeepMind 专注于研究问题（如治疗癌症），与 OpenAI/Anthropic 的企业专注形成对比。还有人质疑谷歌员工本身是否更喜欢其他编码智能体，如 Claude Code 或 Codex。

**标签**: `#AI`, `#coding agent`, `#DeepMind`, `#Gemini`, `#research`

---

<a id="item-4"></a>
## [Mozilla 用 Claude Mythos 预览版强化 Firefox 安全](https://simonwillison.net/2026/May/7/firefox-claude-mythos/#atom-everything) ⭐️ 9.0/10

Mozilla 利用 Anthropic 的 Claude Mythos 预览版自动发现并修复了 Firefox 中数百个漏洞，月度安全漏洞修复数从约 20-30 个飙升至 2026 年 4 月的 423 个。 这标志着 AI 驱动的安全审计发生了范式转变，从低质量的自动报告转向大规模高精度漏洞发现，可能根本改变开源项目处理安全的方式。 该方法使用了自定义框架，将代理式 Claude Code 运行与过滤相结合以减少误报。许多尝试被 Firefox 现有的纵深防御所阻断，发现的漏洞包括一个存在 20 年的 XSLT 漏洞和一个存在 15 年的 <legend> 元素漏洞。

rss · Simon Willison · May 7, 17:56

**背景**: Claude Mythos 是 Anthropic 于 2026 年向特定合作伙伴发布的先进大语言模型。基于 LLM 的安全审计利用 AI 分析源代码以发现漏洞，但早期的尝试往往产生低质量报告。Mozilla 改进的技术和模型能力使这一突破成为可能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Mythos_Preview">Claude Mythos Preview</a></li>
<li><a href="https://red.anthropic.com/2026/mythos-preview/">Claude Mythos Preview \ red.anthropic.com</a></li>

</ul>
</details>

**标签**: `#security`, `#AI`, `#Firefox`, `#LLM`, `#vulnerability research`

---

<a id="item-5"></a>
## [Anthropic 与 SpaceX 达成算力合作，提升 Claude 容量](https://t.me/zaihuapd/41259) ⭐️ 9.0/10

Anthropic 已与 SpaceX 签署协议，使用其 Colossus 1 数据中心全部算力，一个月内获得超过 22 万块 NVIDIA GPU 和 300 兆瓦新增容量。同时，Claude Code 和 Claude API 的速率限制已大幅提升。 这一重大算力合作为 Anthropic 提供了大规模扩展 Claude 模型所需的基础设施，满足了对 Claude Code 等 AI 智能体日益增长的需求。这也是领先 AI 实验室与 SpaceX 之间的罕见合作，凸显了大规模 GPU 集群在推进前沿 AI 中的关键作用。 该协议授予 Anthropic 独家使用整个 Colossus 1 设施的权利，该设施此前为 xAI 建造。Claude Code 的 5 小时速率限制在全部付费方案中翻倍，Pro/Max 用户不再受高峰期限制；Claude Opus API 的速率限制也已提高。

telegram · zaihuapd · May 7, 08:19

**背景**: Anthropic 是一家领先的人工智能公司，开发了 Claude 系列大语言模型。Claude Code 是一款在终端中运行的智能编码工具，可帮助开发者自动化任务。Colossus 1 数据中心由 SpaceX 拥有，拥有世界上最大的 GPU 集群之一，最初用于训练 xAI 的 Grok 模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.datacenterdynamics.com/en/news/anthropic-to-use-all-of-spacex-xais-colossus-1-data-center-compute/">Anthropic to use all of SpaceX -xAI's Colossus 1 data center compute</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://www.aol.com/articles/anthropic-rent-ai-capacity-spacexs-180327894.html">Anthropic to rent all AI capacity at SpaceX 's Colossus data center</a></li>

</ul>
</details>

**标签**: `#Anthropic`, `#SpaceX`, `#算力合作`, `#Claude`, `#NVIDIA GPU`

---

<a id="item-6"></a>
## [小米开源 OmniVoice：支持 646 语种的语音克隆 TTS 模型](https://mp.weixin.qq.com/s/TCS_Sd10g_rvf1cszw673A) ⭐️ 9.0/10

小米下一代 Kaldi 团队开源了 OmniVoice，这是一个大规模多语言零样本文本转语音（TTS）模型，采用极简双向 Transformer 架构，支持 646 种语言的语音克隆。 此次发布标志着开源 TTS 的重要里程碑，OmniVoice 在覆盖前所未有的语种数量的同时，达到了与商用系统相媲美的质量，使得跨语言语音克隆和自定义音色成为可能，惠及全球用户。 OmniVoice 基于 50 个开源数据集构建了 58 万小时的多语言训练数据，训练速度达到每天 10 万小时；模型采用全码本随机掩蔽和大语言模型（LLM）初始化来提升收敛速度和可懂度。

telegram · zaihuapd · May 7, 10:06

**背景**: 传统 TTS 系统通常需要为每种语言单独建模，并依赖大量特定说话人的数据。零样本文本转语音允许在不提供说话人样本的情况下生成新的声音。OmniVoice 采用单阶段的文本到声学映射架构，简化了传统声学模型加声码器的两阶段流程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.aibase.com/news/26962">Xiaomi Open Sources Major Project! OmniVoice Covers 600+...</a></li>
<li><a href="https://www.emergentmind.com/papers/2604.00688">OmniVoice: Omnilingual Zero-Shot TTS</a></li>
<li><a href="https://github.com/wildminder/awesome-ai-voice">GitHub - wildminder/awesome-ai-voice: List of open-source TTS, voice cloning, and music generation models · GitHub</a></li>

</ul>
</details>

**标签**: `#TTS`, `#voice cloning`, `#multilingual`, `#open-source`, `#AI`

---

<a id="item-7"></a>
## [Triton v3.7.0 发布：新增 scaled BMM、FP8 常量等操作](https://github.com/triton-lang/triton/releases/tag/v3.7.0) ⭐️ 8.0/10

Triton v3.7.0 已发布，新增了缩放批量矩阵乘法 (scaled BMM)、直接创建 FP8 常量的支持，以及 tl.squeeze 和 tl.unsqueeze 等新操作，并改进了 LLVM 后端和 AMD/NVIDIA 后端。 Triton 是深度学习中自定义 GPU 内核的关键编译器，这些新功能增强了表达能力和性能，直接影响依赖优化矩阵运算和低精度计算的机器学习工作流的效率。 Scaled BMM 允许在批量矩阵乘法中应用缩放因子，FP8 常量创建减少了内存开销，tl.squeeze/unsqueeze 增加了张量操作的灵活性；该版本还包括前端和后端的众多错误修复和性能优化。

github · atalman · May 7, 22:19

**背景**: Triton 是一种用于编写高效 GPU 内核的领域特定语言和编译器，常用于深度学习框架中实现自定义算子。它将 Python 代码编译成高性能的 CUDA/HIP 内核。Scaled BMM（带缩放的批量矩阵乘法）常用于 Transformer 的注意力机制中。FP8 是一种 8 位浮点格式，可减少内存占用并加速计算，得到 NVIDIA Hopper 等现代 GPU 的支持。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Minifloat">Minifloat - Wikipedia</a></li>
<li><a href="https://docs.nvidia.com/deeplearning/transformer-engine/user-guide/examples/fp8_primer.html">Using FP8 and FP4 with Transformer Engine — Transformer Engine 2.14.0 documentation</a></li>
<li><a href="https://www.exxactcorp.com/blog/hpc/what-is-fp8-fp6-fp4">What is FP8, FP6, FP4? | Exxact Blog</a></li>

</ul>
</details>

**标签**: `#triton`, `#gpu-compiler`, `#machine-learning`, `#deep-learning`, `#release`

---

<a id="item-8"></a>
## [智能体需要控制流，而非更多提示](https://bsuh.bearblog.dev/agents-need-control-flow/) ⭐️ 8.0/10

这篇文章认为，基于大语言模型的智能体应优先采用显式控制流机制，而非依赖日益复杂的提示来处理任务。 这挑战了当前提示工程的流行趋势，并提出了 AI 智能体设计方式的根本转变，可能带来更可靠、更高效的系统。 作者指出，许多智能体任务（如遍历文件或执行确定性步骤）更适合由传统控制流而非大语言模型驱动的提示来处理。

hackernews · bsuh · May 7, 16:43 · [社区讨论](https://news.ycombinator.com/item?id=48051562)

**背景**: 大语言模型智能体利用大语言模型来理解用户请求并执行任务。当前方法通常依赖复杂提示来逐步引导大语言模型。然而，这可能导致低效和脆弱性。文章主张将控制逻辑（如循环、条件判断）与大语言模型的作用分离，仅在需要其推理能力时才使用大语言模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ema.ai/additional-blogs/addition-blogs/understanding-the-architecture-of-llm-agents">Understanding the Architecture of LLM Agents</a></li>

</ul>
</details>

**社区讨论**: 评论者一致同意，许多人分享了遇到提示限制的经验。一些人建议使用大语言模型来编写代码，而非在运行时处理确定性任务。其他人则指出需要超越纯大语言模型的下一代 AI 架构。

**标签**: `#LLM agents`, `#control flow`, `#prompt engineering`, `#AI systems`, `#software engineering`

---

<a id="item-9"></a>
## [Cloudflare 裁员 20%，美其名曰‘建设未来’](https://blog.cloudflare.com/building-for-the-future/) ⭐️ 8.0/10

Cloudflare 在 2026 年 5 月以‘建设未来’为标题发表博文，宣布裁员约 20%，涉及约 1100 名员工。 这家大型科技公司的大规模裁员突显了持续的降本趋势以及 AI 相关开支的影响，引发了关于企业委婉语和员工待遇的争论。 离职员工将获得截止 2026 年底的全额基本工资、美国地区到年底的医保以及加速股权归属；此前该公司曾招聘 1111 名实习生。

hackernews · PriorityLeft · May 7, 20:23 · [社区讨论](https://news.ycombinator.com/item?id=48054423)

**背景**: Cloudflare 提供内容分发网络和网络安全服务。科技行业自 2023 年以来普遍裁员，同时 AI 投资增加了许多公司的运营成本，但尚未立即带来收入增长。

**社区讨论**: 社区评论批评了这个委婉的标题，指出数月前刚招聘实习生却现在裁员的讽刺，并猜测裁员可能源于 AI 成本上升而非生产力提升。一名受影响的员工发布了求职请求，其他人则详细说明了遣散方案。

**标签**: `#layoffs`, `#cloudflare`, `#tech-industry`, `#management`, `#ai-impact`

---

<a id="item-10"></a>
## [Anthropic 开源自然语言自编码器，推动 AI 可解释性](https://www.anthropic.com/research/natural-language-autoencoders) ⭐️ 8.0/10

Anthropic 发布了开权重的自然语言自编码器（NLA）模型，能够将大语言模型（包括 Qwen 2.5 7B、Gemma 3 12B/27B 和 Llama 3.3 70B）的内部激活转换为可读的自然语言文本。 这代表了机械可解释性方面的重要进展，为理解大语言模型内部“思考”提供了新工具。通过开源这些模型，Anthropic 使更广泛的研究社区能够探索并基于此方法进行进一步研究。 NLA 包含一个将激活映射到 token 的 verbalizer 和一个将 token 还原为激活的 reconstructor。作者指出，目标函数中没有任何约束要求解释必须可读或与激活语义相关。

hackernews · instagraham · May 7, 17:54 · [社区讨论](https://news.ycombinator.com/item?id=48052537)

**背景**: 机械可解释性旨在通过分析神经网络内部计算来逆向工程其机制。Transformer circuits 是一个关键研究领域，专注于基于 transformer 的模型如何处理信息。NLAs 在此基础上通过生成激活模式的自然语言描述来推进研究。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/research/natural-language-autoencoders">Natural Language Autoencoders \ Anthropic</a></li>
<li><a href="https://transformer-circuits.pub/2026/nla/">Natural Language Autoencoders Produce Unsupervised...</a></li>
<li><a href="https://github.com/kitft/natural_language_autoencoders">GitHub - kitft/ natural _ language _ autoencoders · GitHub</a></li>

</ul>
</details>

**社区讨论**: 社区评论对 Anthropic 与开源社区（如 Hugging Face、GitHub）的互动表示兴奋，但也对文本是否真正反映模型的真实推理提出了质疑——生成的文本可能只是听起来合理而已。一些用户指出论文承认目标函数并未强制要求可读性。

**标签**: `#AI interpretability`, `#natural language autoencoders`, `#open-source AI`, `#mechanistic interpretability`, `#transformer circuits`

---

<a id="item-11"></a>
## [AI 垃圾内容威胁在线社区真实性](https://rmoff.net/2026/05/06/ai-slop-is-killing-online-communities/) ⭐️ 8.0/10

一篇博客文章指出，被称为“AI 垃圾内容”的低质量 AI 生成内容正在淹没在线社区，导致审核负担加重和信任侵蚀。 这个问题影响在线论坛和社交平台的生存能力，不受控制的 AI 垃圾内容可能会驱赶真实用户，并增加社区管理者的运营成本。 一位社区版主报告每月封禁约 600 个 AI 生成内容的账号，凸显了维持质量所需的不可持续的人工努力。

hackernews · thm · May 7, 18:46 · [社区讨论](https://news.ycombinator.com/item?id=48053203)

**背景**: AI 垃圾内容指用生成式 AI 创建的、被视为低投入、低质量且缺乏意义的数字内容。随着 LLM 等工具让生成大量文本和图像变得容易，它已成为日益增长的担忧。该术语在 Hacker News 等平台上获得关注，用户们讨论其对社区动态的影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_slop">AI slop - Wikipedia</a></li>
<li><a href="https://medium.com/@deejay.me/ai-slop-isnt-about-quality-it-s-about-control-why-people-attack-structure-they-don-t-understand-3f0f1c5eee1b">" AI Slop " Isn't About Quality—It's About Control: Why People...</a></li>

</ul>
</details>

**社区讨论**: 评论显示了分歧：有人认为低质量内容一直存在，真实性会演变；而其他人分享了审核斗争的第一手经验，害怕在与 AI 生成内容的斗争中失败。

**标签**: `#AI`, `#online communities`, `#content moderation`, `#AI slop`, `#Hacker News`

---

<a id="item-12"></a>
## [Chrome 删除设备端 AI 隐私承诺](https://old.reddit.com/r/chrome/comments/1t5qayz/chrome_removes_claim_of_ondevice_al_not_sending/) ⭐️ 8.0/10

Google Chrome 的最新更新中删除了此前声称设备端 AI 功能不会向 Google 服务器发送数据的声明，这引发了隐私担忧。 这一变化削弱了用户对 Chrome 隐私保护的信任，尤其是随着 Google 推动更多设备端 AI 功能（如 Gemini Nano），可能引发监管机构和用户更严格的审视。 被删除的声明是设备端 AI 披露的一部分，其中包括 Gemini Nano——一个悄然安装在设备上的 4GB AI 模型。如果用户保留聊天历史记录，他们也无法选择不让自己的数据用于训练。

hackernews · newsoftheday · May 7, 15:56 · [社区讨论](https://news.ycombinator.com/item?id=48050964)

**背景**: 设备端 AI 是指在用户本地设备上运行而非云端的人工智能模型，可以通过将数据保留在本地来增强隐私。Google 此前曾承诺 Chrome 的设备端 AI 不会向服务器发送任何数据。然而，最近的报道显示，这一承诺被悄然删除，引发了对 Google 数据做法的质疑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://decrypt.co/367193/chrome-removes-privacy-claim-gemini-nano-google">Chrome Deletes Its Own Privacy Promise for Sneaky On - Device AI</a></li>
<li><a href="https://www.notebookcheck.net/Google-Chrome-introduces-on-device-AI-scam-detection-for-enhanced-privacy.935632.0.html">Google Chrome introduces on - device AI ... - NotebookCheck.net News</a></li>

</ul>
</details>

**社区讨论**: 社区情绪高度怀疑，用户指出 Gemini 是唯一不允许选择不使用数据训练的主要供应商。一些人认为 AI 业务本质上就是数据收集，这一变化是策略的一部分。另一些人认为可能只是措辞变化，但担忧依然存在。

**标签**: `#chrome`, `#privacy`, `#AI`, `#on-device`, `#data-collection`

---

<a id="item-13"></a>
## [Anthropic Code w/ Claude 2026 主题演讲直播](https://simonwillison.net/2026/May/6/code-w-claude-2026/#atom-everything) ⭐️ 8.0/10

Anthropic 举办了 Code w/ Claude 2026 活动，主题演讲介绍了 Claude Code 的更新，包括多智能体编排和 Claude Code 例程。 该活动表明 Anthropic 持续投资于 AI 辅助编码工具，可能影响开发者使用大语言模型进行软件开发的方式。 Simon Willison 的直播博客提供了上午主题演讲的实时更新，涵盖了 Claude Code 的托管代理和例程等主题。

rss · Simon Willison · May 6, 15:58

**背景**: Claude 是 Anthropic 开发的一系列大型语言模型，于 2023 年首次发布。Claude Code 是将 Claude 集成到开发工作流中的工具，提供代码审查和自动化任务等功能。Code w/ Claude 活动是 Anthropic 举办的年度开发者大会。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://simonwillison.net/2026/May/6/code-w-claude-2026/">Live blog: Code w / Claude 2026 | Simon Willison’s Weblog</a></li>

</ul>
</details>

**标签**: `#ai`, `#anthropic`, `#claude`, `#generative-ai`, `#live-blog`

---