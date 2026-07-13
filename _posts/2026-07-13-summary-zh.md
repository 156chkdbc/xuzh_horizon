---
layout: default
title: "Horizon Summary: 2026-07-13 (ZH)"
date: 2026-07-13
lang: zh
---

> From 32 items, 10 important content pieces were selected

---

1. [vLLM v0.25.0 发布：Model Runner V2 成为默认，PagedAttention 被移除](#item-1) ⭐️ 9.0/10
2. [GPT-5.6 一小时攻克 50 年图论难题](#item-2) ⭐️ 9.0/10
3. [OpenAI 发布 GPT-5.6 系列：Sol、Terra、Luna 三款模型，性能和成本大幅优化](#item-3) ⭐️ 9.0/10
4. [全球首款侵入式脑机接口医疗器械在中国获批](#item-4) ⭐️ 9.0/10
5. [陶哲轩用 LLM 编程代理开发应用](#item-5) ⭐️ 8.0/10
6. [研究：Claude Code 在提示前消耗 33k tokens，OpenCode 仅 7k](#item-6) ⭐️ 8.0/10
7. [我爱 LLM，但我讨厌炒作](#item-7) ⭐️ 8.0/10
8. [苹果起诉 OpenAI 窃取商业机密用于硬件业务](#item-8) ⭐️ 8.0/10
9. [xAI Grok CLI 默认上传整个代码库及密钥文件](#item-9) ⭐️ 8.0/10
10. [Cursor 开发 'Sand' AI 代理挑战 Claude Cowork](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [vLLM v0.25.0 发布：Model Runner V2 成为默认，PagedAttention 被移除](https://github.com/vllm-project/vllm/releases/tag/v0.25.0) ⭐️ 9.0/10

vLLM v0.25.0 已发布，包含来自 232 位贡献者的 558 次提交。Model Runner V2 现在成为所有密集模型的默认执行路径，传统 PagedAttention 已被移除，Transformers 后端达到了与原生 vLLM 相同的速度。 此次发布通过移除 PagedAttention 并标准化为 MRv2，实现了重大的架构简化，带来更干净的代码和潜在的性能提升。Transformers 后端的性能持平使得用户能够采用熟悉的接口而不牺牲速度，从而扩大了 vLLM 的吸引力。 MRv2 现在支持 EVS、实时嵌入、Mamba 混合模型的前缀缓存、多模态前缀双向注意力以及完整的 CUDA 图支持的动态推测解码。新增模型包括 LLaVA-OneVision-2、Unlimited OCR、MOSS-Transcribe-Diarize、openai/privacy-filter 和 Hy3。

github · khluu · Jul 11, 20:06

**背景**: vLLM 是一个用于高性能 LLM 推理和服务的高效开源库。Model Runner V2（MRv2）是从头重新实现的执行核心，旨在提高模块化和效率。PagedAttention 是原始的注意力机制；它的移除表明全面采用了更新的 V1 和 MRv2 后端。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://vllm-website-5zwgmvte0-inferact-inc.vercel.app/blog/mrv2">Model Runner V 2 : A Modular and Faster Core for vLLM | vLLM Blog</a></li>
<li><a href="https://docs.vllm.ai/en/latest/design/model_runner_v2/">Model Runner V 2 Design Document - vLLM</a></li>
<li><a href="https://huggingface.co/blog/dynamic_speculation_lookahead">Faster Assisted Generation with Dynamic Speculation</a></li>

</ul>
</details>

**标签**: `#vllm`, `#LLM inference`, `#AI frameworks`, `#open source`, `#performance`

---

<a id="item-2"></a>
## [GPT-5.6 一小时攻克 50 年图论难题](https://www.qbitai.com/2026/07/447873.html) ⭐️ 9.0/10

OpenAI 的 GPT-5.6 Sol Ultra 在不到一小时内证明了循环双覆盖猜想，这是一个存在近 50 年的图论开放问题，模型通过协调 64 个并行子代理并使用精心设计的提示完成证明。 这一成就展示了 AI 在高级推理和多代理协调方面的能力，标志着数学研究方式的范式转变。它表明大型语言模型能够解决困扰人类数学家数十年的深奥理论问题。 证明在一小时内完成并生成了 3 页 PDF。模型将问题转化为有限域上的边标号和线性方程组问题，OpenAI 发布了完整的 700 字符提示，其中规定了验收标准、定义、边界条件和失败情形，但没有规定固定步骤。

telegram · zaihuapd · Jul 12, 03:49

**背景**: 循环双覆盖猜想询问每个无桥图是否都有一个圈的集合，使得每条边恰好被覆盖两次。图中的桥是指删除后增加连通分量数量的边。该猜想由 Szekeres (1973) 和 Seymour (1979) 独立提出，是图论中的一个核心开放问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cycle_double_cover_conjecture">Cycle double cover conjecture</a></li>
<li><a href="https://en.wikipedia.org/wiki/Bridge_(graph_theory)">Bridge (graph theory)</a></li>
<li><a href="https://mathworld.wolfram.com/CycleDoubleCoverConjecture.html">Cycle Double Cover Conjecture -- from Wolfram MathWorld</a></li>

</ul>
</details>

**标签**: `#AI`, `#graph theory`, `#GPT-5.6`, `#breakthrough`, `#mathematics`

---

<a id="item-3"></a>
## [OpenAI 发布 GPT-5.6 系列：Sol、Terra、Luna 三款模型，性能和成本大幅优化](https://t.me/zaihuapd/42512) ⭐️ 9.0/10

OpenAI 于 2026 年 6 月 26 日宣布推出 GPT-5.6 模型家族，包含三个变体：旗舰版 Sol（最强能力）、平衡版 Terra（性能与成本平衡）和低成本版 Luna（高并发场景）。该系列在代码生成、知识工作、设计、研究和网络安全方面有显著提升，并引入了 max/ultra 推理模式、多智能体协作和 Programmatic Tool Calling。 此次发布通过分层定价使先进 AI 更易获取且更具成本效益，让组织能够为自身需求选择合适的能力级别。推理模式和多智能体协作等代理功能的引入，突破了自主任务完成的边界，有望改变代码、研究和安全领域的工作流程。 GPT-5.6 默认使用 Sol 进行通用任务；Terra 为大多数工作负载提供平衡的定价，而 Luna 则针对高并发和低成本进行了优化。'max' 推理模式支持更深入的思考，'ultra' 模式利用子代理加速复杂任务；Programmatic Tool Calling 允许模型以编程方式与外部 API 和工具交互。

telegram · zaihuapd · Jul 12, 11:19

**背景**: OpenAI 的 GPT 系列发展迅速，GPT-5.5 在两个月前刚刚发布。这种分层方法反映了行业针对不同用例提供专门模型的趋势。Programmatic Tool Calling 扩展了函数调用能力，通过允许模型以结构化方式调用工具和 API，实现自主工作流。ChatGPT Work 是一个新代理，旨在通过连接工具和自动化任务，将目标转化为完成的输出。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.digitalapplied.com/blog/gpt-5-6-sol-terra-luna-preview-guide-2026">GPT - 5 . 6 Sol , Terra & Luna : OpenAI's New Model Family</a></li>
<li><a href="https://www.linkedin.com/posts/vaibhavs10_introducing-gpt-56-sol-terra-and-luna-activity-7476322117161058304-W_mZ">Introducing GPT - 5 . 6 : Sol , Terra and Luna . Sol is our strongest...</a></li>
<li><a href="https://openai.com/index/chatgpt-for-your-most-ambitious-work/">ChatGPT is now a partner for your most ambitious work - OpenAI</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#GPT-5.6`, `#Large Language Models`, `#AI`, `#Generative AI`

---

<a id="item-4"></a>
## [全球首款侵入式脑机接口医疗器械在中国获批](https://t.me/zaihuapd/42515) ⭐️ 9.0/10

国家药监局批准了全球首款侵入式脑机接口医疗器械，即博睿康医疗科技开发的植入式脑机接口手部运动功能代偿系统。这标志着该类医疗器械在全球首次获批上市。 该批准标志着脑机接口从研究走向临床应用，是神经技术领域的范式转变。它为四肢瘫患者恢复手部功能带来新希望，可能改善数百万患者的生活质量，并加速脑机接口技术的投资。 该设备采用硬脑膜外微创植入技术，结合无线供能与数据传输，并通过气动手套辅助手部抓握。适应症为 18 至 60 岁因颈段脊髓损伤导致四肢瘫的患者。

telegram · zaihuapd · Jul 12, 14:39

**背景**: 脑机接口（BCI）实现大脑与外部设备的直接通信。侵入式 BCI 需要手术植入，信号质量更高但风险也更大。此前获批的 BCI 仅限于非侵入式或半侵入式系统，这是首个获得临床使用监管批准的完全侵入式 BCI。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ecns.cn/m/news/sci-tech/2026-03-17/detail-ihfaunkv7709855.shtml">China approves world's first invasive BCI medical device</a></li>
<li><a href="https://trial.medpath.com/news/china-approves-world-s-first-commercial-brain-computer-interface-for-spinal-cord-injury-treatment">China Approves World's First Commercial Brain - Computer Interface ...</a></li>

</ul>
</details>

**标签**: `#brain-computer interface`, `#medical device`, `#regulatory approval`, `#neurotechnology`, `#spinal cord injury`

---

<a id="item-5"></a>
## [陶哲轩用 LLM 编程代理开发应用](https://terrytao.wordpress.com/2026/07/11/old-and-new-apps-via-modern-coding-agents/) ⭐️ 8.0/10

菲尔兹奖得主陶哲轩使用现代 LLM 编程代理，为他的研究论文构建可视化和简单的交互式应用，展示了 AI 辅助编程在非关键任务上的易用性。 这凸显了 AI 编程工具已经足够强大，以至于非软件工程领域的专家也能创建定制软件，可能为科学家、教育工作者和爱好者带来软件创作的民主化。 陶哲轩指出，由于这些可视化只是补充而非论文的关键内容，使用 LLM 代理的负面风险是可以接受的，这反映了一种务实的 AI 可信度观点。

hackernews · subset · Jul 12, 11:09 · [社区讨论](https://news.ycombinator.com/item?id=48880170)

**背景**: LLM 编程代理是使用大型语言模型根据自然语言指令编写和调试代码的 AI 系统。它们能根据用户提示生成完整的应用或可视化，降低了软件开发的门槛。这类工具在教育和原型设计中越来越受欢迎，让非程序员也能创建功能性软件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zencoder.ai/">Zencoder | The AI Coding Agent</a></li>

</ul>
</details>

**社区讨论**: 社区评论对 LLM 辅助编程表达了热情，一位用户指出这大大提升了他们的计算机科学课程，能实现之前没时间构建的可视化。另一个人幽默地将陶哲轩对编程代理的接纳比作米其林大厨发现微波炉晚餐。有评论强调传统领域之外存在无限的软件潜在需求，其他人则欣赏陶哲轩关于可信度的平衡观点。

**标签**: `#LLM`, `#coding agents`, `#software development`, `#education`, `#visualization`

---

<a id="item-6"></a>
## [研究：Claude Code 在提示前消耗 33k tokens，OpenCode 仅 7k](https://systima.ai/blog/claude-code-vs-opencode-token-overhead) ⭐️ 8.0/10

一项实证研究发现，Claude Code 在处理用户提示前，会在工具框架开销上消耗约 33,000 个 token，而 OpenCode 仅使用约 7,000 个 token，显示出显著的 token 消耗低效。 这种开销直接影响开发者的成本和 API 使用预算，使得 OpenCode 在智能体编码任务中成为更 token 高效的选择。同时也引发了对 Anthropic 的设计是否鼓励更高 token 消耗的疑问。 该研究记录了编码工具与 Anthropic 端点之间的所有请求，比较了缓存策略和工具框架的 token 使用情况。作者计划后续进行更深入的任务和定性对比，以回应社区反馈。

hackernews · systima · Jul 12, 18:25 · [社区讨论](https://news.ycombinator.com/item?id=48883275)

**背景**: Token 是语言模型处理的文本单位，每个 token 都会产生费用并占用上下文窗口容量。像 Claude Code 和 OpenCode 这样的智能体编码工具使用系统提示和工具框架来编排自主编码工作流，这增加了额外开销。不同工具间的开销差异很大，影响速度和成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.kdnuggets.com/the-beginners-guide-to-tracking-token-usage-in-llm-apps">The Beginner’s Guide to Tracking Token Usage in LLM ... - KDnuggets</a></li>
<li><a href="https://cloud.google.com/discover/what-is-agentic-coding">What is agentic coding? How it works and use cases | Google Cloud</a></li>
<li><a href="https://www.tembo.io/blog/agentic-ai-coding-tools">Best Agentic AI Coding Tools in 2026: Compared - Tembo.io</a></li>

</ul>
</details>

**社区讨论**: 评论者指出子智能体消耗大量 token，有用户报告 7 个子智能体在任何一个完成前就耗尽了预算。其他人怀疑 Anthropic 从 token 膨胀中获利，而 pi 等工具使用的 token 甚至更少。研究作者承认了关于衡量正确指标的合理批评，并承诺改进分析。

**标签**: `#AI coding tools`, `#token efficiency`, `#Claude Code`, `#OpenCode`, `#LLM overhead`

---

<a id="item-7"></a>
## [我爱 LLM，但我讨厌炒作](https://geohot.github.io//blog/jekyll/update/2026/07/12/i-love-llms.html) ⭐️ 8.0/10

George Hotz 发表了一篇博客文章，反思围绕大型语言模型的炒作，尽管 LLM 创造了巨大价值，但前沿实验室可能无法捕获这些价值。 这一批评挑战了 AI 公司的天价估值，并提出了关于谁从 AI 进步中受益的重要问题，影响投资者、开发者和开源社区。 文章的主要论点认为价值创造不等于价值捕获，这解释了为什么前沿实验室推动基于代币的定价模式，而开源替代方案蓬勃发展。

hackernews · therepanic · Jul 12, 18:31 · [社区讨论](https://news.ycombinator.com/item?id=48883343)

**社区讨论**: 评论者大多同意价值捕获的观点，一些人指出 LLM 提高了他们在特定软件上的个人生产力，但也对开源维护的未来表示担忧，因为分支变得过于容易。

**标签**: `#LLMs`, `#hype`, `#value capture`, `#open source`, `#productivity`

---

<a id="item-8"></a>
## [苹果起诉 OpenAI 窃取商业机密用于硬件业务](https://t.me/zaihuapd/42502) ⭐️ 8.0/10

7 月 10 日，苹果在美国加州北区联邦法院起诉 OpenAI、两名前员工及 io Products，指控其通过招聘苹果员工、接触供应商等方式，系统性窃取苹果的产品设计、制造工艺及供应链机密，以加速 OpenAI 的消费级硬件研发。 两大科技巨头之间的这场高 stakes 法律战可能重塑 AI 硬件竞争格局，并为行业商业机密保护树立先例。如果苹果胜诉，可能延缓 OpenAI 的硬件计划，并威慑其他公司通过挖角获取机密信息。 苹果特别指控前员工 Chang Liu 离职后仍访问内部网络并下载数十份硬件文件；OpenAI 硬件负责人 Tang Yew Tan 被指在离职前将供应商资料发送至个人邮箱，并要求求职者携带苹果零部件参加面试。苹果还声称，目前有超过 20 名前员工被 OpenAI 雇佣，引发对系统性信息泄露的担忧。

telegram · zaihuapd · Jul 11, 16:29

**背景**: 苹果长期投入巨资开发定制硬件，包括 A 系列和 M 系列芯片以及 Vision Pro 等产品，其设计和供应链细节高度机密。OpenAI 以 ChatGPT 等软件闻名，但近年来正扩展至硬件领域，据称正在开发 AI 专用设备。商业机密诉讼在硅谷并不罕见，但此案涉及两家资源雄厚的知名企业，因此格外引人注目。

**标签**: `#Apple`, `#OpenAI`, `#trade secrets`, `#legal`, `#hardware`

---

<a id="item-9"></a>
## [xAI Grok CLI 默认上传整个代码库及密钥文件](https://gist.github.com/cereblab/dc9a40bc26120f4540e4e09b75ffb547) ⭐️ 8.0/10

安全研究人员发现，xAI 的 Grok Build CLI（0.2.93 版本）默认将整个代码仓库及 .env 等敏感文件上传至 xAI 服务器，即使关闭隐私开关也无法阻止；xAI 随后于 7 月 13 日部署了服务器端修复，新增了 disable_codebase_upload 字段。 该漏洞对使用该工具的开发者构成严重的安全和隐私风险，可能导致专有代码、凭据和密钥在未经同意的情况下泄露至外部服务器，这可能会严重破坏对 xAI 工具及 AI 辅助开发平台的信任。 抓包分析显示，工具读取的文件内容会被嵌入模型请求并上传至 Google Cloud Storage 存储桶；即使提示词明确要求不要打开某个文件，整个仓库仍以 git bundle 形式上传；在 12 GB 仓库的测试中，超过 5 GiB 数据成功上传。

telegram · zaihuapd · Jul 12, 04:19

**背景**: Grok Build 是 xAI 官方推出的命令行编码代理，由 Grok 4.5 驱动，旨在协助完成复杂编码任务。git bundle 是一个包含 Git 仓库所有对象和引用的单一文件，常用于离线或网络传输仓库。该工具的“改进模型”隐私设置被发现无法有效阻止上传。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.ai/cli">Grok Build | SpaceXAI</a></li>
<li><a href="https://git-scm.com/docs/git-bundle">Git - git-bundle Documentation</a></li>

</ul>
</details>

**标签**: `#security`, `#privacy`, `#xAI`, `#CLI`, `#data leak`

---

<a id="item-10"></a>
## [Cursor 开发 'Sand' AI 代理挑战 Claude Cowork](https://www.theinformation.com/articles/cursor-developing-ai-agent-compete-claude-cowork) ⭐️ 8.0/10

Cursor 正在秘密开发代号为 'Sand' 的通用 AI 代理，可处理邮件回复和电子表格整理等多步骤任务，旨在于直接与 Anthropic 的 Claude Cowork 和 OpenAI 的 ChatGPT Work 竞争。 此举标志着 Cursor 有意突破代码编辑器领域，进入更广泛的企业 AI 助手市场，加剧 AI 代理之间的竞争，并可能重塑企业采用 AI 进行工作流自动化的方式。 'Sand' 代理尚未公开发布，其开发凸显了向多步骤、自主 AI 代理发展的趋势，这些代理可在各种应用程序和文件类型中操作。

telegram · zaihuapd · Jul 13, 01:34

**背景**: Cursor 是一个 AI 驱动的代码编辑器，利用 AI 代理辅助开发者完成编码任务。Anthropic 的 Claude Cowork 和 OpenAI 的 ChatGPT Work 是可以与文件、文件夹和应用程序交互以执行实际任务的 AI 助手。这些工具代表了从简单聊天机器人向能够执行复杂工作流的自主代理的转变。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cursor.com/">Cursor: AI coding agent</a></li>
<li><a href="https://claude.com/product/cowork">Claude Cowork | Claude by Anthropic</a></li>
<li><a href="https://chatgpt.com/work/">ChatGPT Work</a></li>

</ul>
</details>

**标签**: `#AI agent`, `#Cursor`, `#enterprise AI`, `#competition`, `#general AI`

---