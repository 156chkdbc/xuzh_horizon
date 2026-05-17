---
layout: default
title: "Horizon Summary: 2026-05-17 (ZH)"
date: 2026-05-17
lang: zh
---

> From 35 items, 11 important content pieces were selected

---

1. [SGLang v0.5.12 全面支持 DeepSeek V4 推理](#item-1) ⭐️ 9.0/10
2. [vllm v0.21.0 发布：重大变更、KV 卸载与 Blackwell 支持](#item-2) ⭐️ 8.0/10
3. [2005 年科幻小说《加速》与当今 AI 热潮共鸣](#item-3) ⭐️ 8.0/10
4. [前沿 AI 攻破 CTF 比赛形式](#item-4) ⭐️ 8.0/10
5. [δ-mem：通过 delta 规则学习为 LLM 提供固定大小记忆](#item-5) ⭐️ 8.0/10
6. [Hashimoto 警告公司出现“AI 精神病”](#item-6) ⭐️ 8.0/10
7. [苹果与 OpenAI 联盟出现裂痕，OpenAI 考虑法律行动](#item-7) ⭐️ 8.0/10
8. [谷歌将操纵 AI 搜索结果列为垃圾行为](#item-8) ⭐️ 8.0/10
9. [盖洛普：71%美国人反对本地建 AI 数据中心](#item-9) ⭐️ 8.0/10
10. [马耳他政府与 OpenAI 合作，向所有公民免费提供 ChatGPT Plus](#item-10) ⭐️ 8.0/10
11. [GitHub Copilot 桌面应用技术预览开放](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [SGLang v0.5.12 全面支持 DeepSeek V4 推理](https://github.com/sgl-project/sglang/releases/tag/v0.5.12) ⭐️ 9.0/10

SGLang v0.5.12 为 DeepSeek V4 提供了完整的推理支持，包括张量并行、专家并行、上下文并行、数据并行注意力，以及 HiSparse KV 缓存卸载、DeepGemm 和 FlashMLA 内核等优化。 此版本意义重大，因为它能够高效部署 DeepSeek V4 这种先进的 MoE 模型，降低推理成本并提高吞吐量，从而惠及更广泛的人工智能基础设施生态系统。 该版本还包含 W4A4 MegaMoE 内核、预填充-解码分离、基于统一 Radix Tree 的 HiCache、针对 Blackwell GPU 的 TokenSpeed MLA 注意力后端，以及适用于所有 Nvidia GPU 的统一 Docker 镜像。

github · Fridge003 · May 16, 18:23

**背景**: SGLang 是一个开源的大语言模型推理引擎，专注于高性能和易用性。DeepSeek V4 是 DeepSeek 公司发布的大规模混合专家（MoE）模型，通过多个专家子网络提高容量，但推理计算复杂。SGLang 通过多种并行策略和优化内核来加速这一过程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.lmsys.org/blog/2026-04-10-sglang-hisparse/">HiSparse : Turbocharging Sparse Attention with... | LMSYS Org</a></li>
<li><a href="https://docs.ray.io/en/latest/serve/llm/architecture/serving-patterns/prefill-decode.html">Prefill-decode disaggregation — Ray 2.55.1</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#SGLang`, `#inference`, `#GPU optimization`, `#MoE`

---

<a id="item-2"></a>
## [vllm v0.21.0 发布：重大变更、KV 卸载与 Blackwell 支持](https://github.com/vllm-project/vllm/releases/tag/v0.21.0) ⭐️ 8.0/10

vllm 项目于 2025 年 3 月 26 日发布了 v0.21.0 版本，包含来自 202 位贡献者的 367 次提交。该版本引入了重大变更，包括弃用 transformers v4 和 C++20 构建要求，同时新增了基于混合内存分配器 (HMA) 的 KV 缓存卸载、支持思考预算的推测解码，以及面向 Blackwell GPU 的 TOKENSPEED_MLA 注意力后端。 该版本对 LLM 推理生态系统具有重要意义，它为未来与 transformers v5 和现代 C++ 标准的兼容性奠定了基础，同时通过 KV 卸载和推测解码增强提高了内存效率和推理速度。Blackwell GPU 支持使得在下一代硬件上为 DeepSeek-R1 和 Kimi-K2.5 等模型实现高性能推理。 值得注意的技术细节包括弃用 transformers v4 并转向 v5、强制要求 C++20 编译器，以及集成 HMA 用于 KV 卸载，通过在不同层类型间池化内存来减少内存浪费。推测解码的思考预算特性确保推理 token 生成遵守配置的限制，而 TOKENSPEED_MLA 后端则使用针对 Blackwell GPU 优化的 MLA（多头潜在注意力）内核。

github · khluu · May 15, 08:44

**背景**: vLLM 是一个开源的大语言模型推理引擎，旨在优化服务吞吐量和内存使用。混合内存分配器 (HMA) 是一种新的内存管理方案，按类型（如注意力、SSM）对层进行分组，并在它们之间池化内存，减少内部碎片。TOKENSPEED_MLA 是一个自定义注意力后端，用于 DeepSeek-R1 等模型中的多头潜在注意力 (MLA)，专为在 NVIDIA 的 Blackwell 架构上实现高性能而设计。推测解码通过使用较小的草稿模型预测 token，然后让目标模型并行验证，从而加速生成；而“思考预算”扩展确保推理模型不会生成过多的思考 token。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/design/hybrid_kv_cache_manager/">Hybrid KV Cache Manager - vLLM</a></li>
<li><a href="https://docs.vllm.ai/en/latest/design/attention_backends/">Attention Backend Feature Support - vLLM</a></li>
<li><a href="https://x.com/lightseekorg/status/2055483456503914952">Excited to see TOKENSPEED_MLA integrated into vLLM on ...</a></li>

</ul>
</details>

**标签**: `#LLM inference`, `#vllm`, `#breaking change`, `#KV cache`, `#speculative decoding`

---

<a id="item-3"></a>
## [2005 年科幻小说《加速》与当今 AI 热潮共鸣](https://www.antipope.org/charlie/blog-static/fiction/accelerando/accelerando.html) ⭐️ 8.0/10

查尔斯·斯特罗斯 2005 年的小说《加速》作为免费电子书在线发布，如今读者将其中的未来 AI 代理与当今的生成式 AI 和增强现实工具相类比，重新引发了公众讨论。 这部小说对 AI 驱动社会加速的先见性描绘为审视当前技术趋势提供了独特视角，引发了对 AI 发展轨迹及其社会影响的深刻反思。 《加速》获得了 2006 年轨迹奖，并获得了雨果奖、坎贝尔奖、克拉克奖和英国科幻协会奖提名；它采用知识共享许可发布，因此广泛可访问。

hackernews · eamag · May 16, 11:36 · [社区讨论](https://news.ycombinator.com/item?id=48159241)

**背景**: 《加速》是一部由相互关联的短篇小说组成的断续小说，讲述一个家庭在技术奇点（AI 超越人类智能）中数十年的历程。故事探讨了后人类主义、虚拟现实和经济破坏等主题，角色们极度依赖名为 Aineko 的 AI 代理和增强现实眼镜来完成日常任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Accelerando_(novel)">Accelerando (novel)</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的评论者强调，小说中关于 AI 代理和对增强现实依赖的预言正在成为现实，一位用户指出主角失去眼镜后变得无助——这一场景在现代 AI 助手下变得可信。其他人称赞这部小说的“合理的怪异”，并推荐它与《量子窃贼》一起阅读，以体验对未来怪异的现实描绘。

**标签**: `#science fiction`, `#AI`, `#agent systems`, `#futurism`, `#speculation`

---

<a id="item-4"></a>
## [前沿 AI 攻破 CTF 比赛形式](https://kabir.au/blog/the-ctf-scene-is-dead) ⭐️ 8.0/10

前沿 AI 模型现在能够瞬间解决传统 CTF 挑战，削弱了这些网络安全赛事的学习和竞争价值。 CTF 是培养网络安全人才的关键途径；如果 AI 使其变得无关紧要，可能会减少实践学习和技能发展，引发关于 AI 对教育影响的更广泛问题。 文章指出，AI 现在“破坏了”参与和构建 CTF 挑战的体验，参与者依赖大语言模型在几分钟内解决挑战；有人建议提高 CTF 难度，但又担心进入“过于困难”的领域。

hackernews · frays · May 16, 07:01 · [社区讨论](https://news.ycombinator.com/item?id=48157559)

**背景**: CTF（夺旗赛）是一种网络安全竞赛，参与者通过解决安全相关的挑战来寻找隐藏的“旗帜”。它们一直是学习与测试黑客、密码学、逆向工程和取证技术的流行方式。前沿 AI 指的是最先进的大语言模型，如 GPT-4，它们能够推理并解决复杂问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/ai-new-cybersecurity-frontier-why-trust-starts-identity-6mowc">AI and the New Cybersecurity Frontier : Why Trust Starts with Identity</a></li>
<li><a href="https://techitupme.com/sentinelone-unveils-wayfinder-frontier-ai-to-break-exploitation-chains/">SentinelOne Wayfinder Frontier AI Exposes Exploitation Chains</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了沮丧，认为 AI 消除了团队协作的学习体验——队友们原本会花费数小时一起解决挑战。有人提供了使用 AI 去混淆代码的例子，并指出“替我完成”的心态难以抗拒，导致失去了真正的学习。

**标签**: `#AI`, `#CTF`, `#cybersecurity`, `#education`, `#LLM`

---

<a id="item-5"></a>
## [δ-mem：通过 delta 规则学习为 LLM 提供固定大小记忆](https://arxiv.org/abs/2605.12357) ⭐️ 8.0/10

研究人员提出了δ-mem，该方法通过 delta 规则学习将过去信息压缩为固定大小的状态矩阵，使 LLM 能够在不扩展上下文窗口的情况下高效保留和更新记忆。 这可能显著降低 LLM 在长期交互中的内存占用，使得具有几乎无限上下文的实际智能体和助手成为可能，同时保持 GPU 效率。 δ-mem 使用通过 delta 规则学习更新的固定大小状态矩阵，delta 规则是一种基于预测误差调整权重的梯度下降方法。论文没有明确提到计算成本，但强调了可以高效存储和检索的固定大小记忆。

hackernews · 44za12 · May 16, 09:30 · [社区讨论](https://news.ycombinator.com/item?id=48158506)

**背景**: 大型语言模型（LLM）如 GPT-4 在大量文本数据上训练并生成回复。它们面临长期记忆困难，因为上下文窗口有限且扩展成本高。Delta 规则学习是一种神经网络中的权重更新方法，通过梯度下降最小化误差，常用于监督学习。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2605.12357">$δ$-mem: Efficient Online Memory for Large Language Models</a></li>
<li><a href="https://en.wikipedia.org/wiki/Delta_rule">Delta rule - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论对固定大小记忆实现无限上下文表示兴趣，但有人质疑它是否真正解决了容量问题，并注意到输入微小变化会导致激活巨大差异。其他人认为这种方法可以实现具有几乎无限记忆的智能体，但成本未被讨论。

**标签**: `#LLM`, `#memory`, `#efficiency`, `#online learning`, `#deep learning`

---

<a id="item-6"></a>
## [Hashimoto 警告公司出现“AI 精神病”](https://twitter.com/mitchellh/status/2055380239711457578) ⭐️ 8.0/10

Vagrant 和 Consul 的创始人 Mitchell Hashimoto 在 Twitter 上警告说，整个公司正陷入“AI 精神病”——盲目采用 AI 工具，而不考虑长期软件基础设施风险。 这一批评突显了软件工程中日益严重的对 AI 过度依赖的趋势，这可能会引入隐藏的漏洞、安全缺陷和不可持续的技术债务，尤其是在管理层施压要求团队对所有任务使用 AI 的情况下。 Hashimoto 的帖子引发了 1906 分和 1103 条评论的讨论，工程师们分享了真实案例，例如 FAANG 管理层强制要求日常 token 配额，以及财务经理为了赢得炫耀比赛而推动 AI 采用。

hackernews · reasonableklout · May 15, 20:26 · [社区讨论](https://news.ycombinator.com/item?id=48153379)

**背景**: “AI 精神病”一词最初指的是个体因与聊天机器人互动而出现精神病现象。在这里，Hashimoto 用其比喻性地描述那些非理性采用 AI 工具、忽视软件基础设施基础风险的组织。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_psychosis">AI psychosis</a></li>
<li><a href="https://www.forbes.com/sites/truebridge/2026/04/27/the-ai-buildout-boom-is-real--but-so-are-the-risks/">The AI Buildout Boom Is Real – But So Are The Risks - Forbes</a></li>

</ul>
</details>

**社区讨论**: 社区评论反映了复杂的情绪：一些工程师感到即使 AI 妨碍生产力也被迫使用，而另一些人则担心“腐朽的基础”和“氛围编程”会导致灾难性故障。一位财务经理承认，他们的 CFO 只是想跟上同行才加速 AI 使用。

**标签**: `#AI`, `#software engineering`, `#overreliance`, `#industry criticism`, `#risk`

---

<a id="item-7"></a>
## [苹果与 OpenAI 联盟出现裂痕，OpenAI 考虑法律行动](https://www.bloomberg.com/news/articles/2026-05-14/openai-apple-partnership-frays-setting-up-possible-legal-fight) ⭐️ 8.0/10

据彭博社报道，苹果与 OpenAI 的合作关系正在恶化，OpenAI 正就苹果未充分推广 ChatGPT 集成一事探讨法律选项，该集成带来的订阅收入远低于预期。苹果计划在 6 月的 WWDC 上向 Claude、Gemini 等第三方模型开放 Siri，进一步削弱 OpenAI 的独家地位。 两大行业巨头之间的裂痕可能重塑 AI 助手格局，推动移动设备上的 AI 生态系统更加开放和竞争。其结局可能影响其他科技公司如何构建 AI 合作伙伴关系和收入分成协议。 OpenAI 声称 ChatGPT 在苹果系统中的入口隐蔽且功能受限，导致多数用户仍直接使用独立 App。另一方面，苹果对 OpenAI 的隐私标准、硬件业务和挖角工程师感到不满，并计划在 iOS 27 的 Siri 中集成多个 AI 模型。

telegram · zaihuapd · May 15, 12:59

**背景**: 苹果与 OpenAI 于 2024 年宣布合作，将 ChatGPT 集成到 Siri 中，旨在创造数十亿美元的订阅收入。然而，双方在营销、收入分配和战略分歧上矛盾加剧。Anthropic 的 Claude 和 Google 的 Gemini 是竞争性的大语言模型（LLM），苹果目前正考虑集成它们。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_(language_model)">Claude (language model) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gemini_(AI_model)">Gemini (AI model)</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#Apple`, `#AI partnership`, `#legal dispute`, `#WWDC`

---

<a id="item-8"></a>
## [谷歌将操纵 AI 搜索结果列为垃圾行为](https://www.theverge.com/tech/931416/google-ai-search-spam-policy) ⭐️ 8.0/10

谷歌更新了搜索垃圾内容政策，明确禁止操纵生成式 AI 搜索结果（包括 AI Overview 和 AI Mode），并将此类行为视为垃圾内容处理。 该政策直接针对新兴的生成引擎优化（GEO）实践，影响 SEO 专业人士、内容创作者和依赖 AI 可见度的企业，可能重塑 AI 搜索的优化策略。 违规行为包括批量生成带有偏见的‘最佳推荐’内容或在网页中埋藏隐藏提示以影响 AI 模型；处罚可能包括排名降级甚至从搜索结果中完全移除。

telegram · zaihuapd · May 16, 06:31

**背景**: 生成引擎优化（GEO）是一种结构化内容以增加在 AI 生成回答中可见性的实践，类似于传统 SEO 但针对 AI 助手（如谷歌 AI Overview）。谷歌此前面临 AI Overview 中的垃圾问题，出现过偏见或不准确的结果案例。更新后的政策将现有垃圾规则应用于 AI 生成的搜索功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theverge.com/tech/931416/google-ai-search-spam-policy">Google updates its spam rules to include attempts to ‘manipulate’ AI</a></li>
<li><a href="https://searchengineland.com/google-updates-search-spam-policies-to-clarify-it-applies-to-generative-ai-responses-477657">Google confirms spam policies apply to AI Overviews and AI Mode</a></li>
<li><a href="https://en.wikipedia.org/wiki/Generative_engine_optimization">Generative engine optimization - Wikipedia</a></li>

</ul>
</details>

**标签**: `#Google`, `#AI search`, `#spam policy`, `#GEO`, `#SEO`

---

<a id="item-9"></a>
## [盖洛普：71%美国人反对本地建 AI 数据中心](https://news.gallup.com/poll/709772/americans-oppose-data-centers-area.aspx) ⭐️ 8.0/10

盖洛普 3 月的一项民调显示，71%的美国人反对在家附近建设 AI 数据中心，其中 48%表示强烈反对。这是盖洛普首次就这一问题进行调查。 这种强烈的公众反对情绪可能影响 AI 基础设施政策和选址决策，因为数据中心的能源和水资源消耗正成为有争议的环境问题。 在反对者中，约一半提到电力消耗过高和用水过多，其他人则担心污染、噪音、交通和生活成本上升；支持者主要提及就业和税收。对 AI 数据中心的抵触甚至超过对当地核电站的反对。

telegram · zaihuapd · May 16, 07:59

**背景**: AI 数据中心需要大量电力和水用于计算和冷却。2024 年，美国数据中心用电量为 183 太瓦时，超大规模设施的用水量预计到 2028 年将每年达到 330 亿加仑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.eesi.org/articles/view/data-centers-and-water-consumption">Data Centers and Water Consumption | Article | EESI</a></li>
<li><a href="https://www.iea.org/news/data-centre-electricity-use-surged-in-2025-even-with-tightening-bottlenecks-driving-a-scramble-for-solutions">Data centre electricity use surged in 2025, even with tightening bottlenecks driving a scramble for solutions - News - IEA</a></li>

</ul>
</details>

**标签**: `#AI`, `#data centers`, `#public opinion`, `#energy`, `#environment`

---

<a id="item-10"></a>
## [马耳他政府与 OpenAI 合作，向所有公民免费提供 ChatGPT Plus](https://openai.com/index/malta-chatgpt-plus-partnership/) ⭐️ 8.0/10

OpenAI 与马耳他政府推出'AI for All'计划，马耳他公民在完成由马耳他大学开发的 AI 素养课程后，可获得一年免费的 ChatGPT Plus。 这是首个国家级此类合作，可能为其他国家将 AI 素养教育与便捷的 AI 工具相结合提供范例，从而加速全球的 AI 普及和教育。 该计划于 5 月启动，由马耳他数字创新局管理，并将逐步扩展到海外马耳他公民。AI 素养课程涵盖 AI 的能力与责任。

telegram · zaihuapd · May 16, 10:40

**背景**: ChatGPT Plus 是付费订阅服务，提供更快的响应速度、优先使用新功能以及 GPT-4 等高级模型的访问权限。AI 素养教育日益被视为负责任地采用 AI 的关键，而此次合作直接将学习与实际使用联系起来。

**标签**: `#OpenAI`, `#ChatGPT`, `#AI education`, `#government partnership`, `#Malta`

---

<a id="item-11"></a>
## [GitHub Copilot 桌面应用技术预览开放](https://github.blog/changelog/2026-05-14-github-copilot-app-is-now-available-in-technical-preview/) ⭐️ 8.0/10

GitHub 发布了 Copilot 桌面应用的技术预览版，用户可从 issue、PR、提示词或历史会话中启动隔离的开发会话，并在应用内查看变更、运行测试及创建 PR。同时引入了 Agent Merge 功能，可自动处理审核评论和合并操作。 该桌面应用标志着 Copilot 从 IDE 插件向独立工作流中心的重大转变，有望简化开发者从构思到合并的整个贡献周期。它能减少上下文切换，尤其对使用 GitHub 中心化工作流的团队可提升生产力。 Copilot Pro 和 Pro+ 订阅者可立即申请抢先体验；Business 和 Enterprise 用户将在本周内陆续获得访问权限，但需要组织管理员在策略中开启预览和 CLI 权限。该应用通过 Copilot Cloud Agent 支持代理驱动的合并冲突解决，该功能最早于 2026 年 4 月预告。

telegram · zaihuapd · May 16, 15:07

**背景**: GitHub Copilot 是一款 AI 编程助手，传统上以插件形式运行于 VS Code 或 JetBrains 等 IDE 中。新的桌面应用旨在提供更集成的代码审查和 PR 管理环境。Agent Merge 由 Copilot Cloud Agent 驱动，可自动解决合并冲突和审核评论，减少手动工作。此前的版本允许在 GitHub.com 上通过一次点击修复合并冲突，而桌面应用将这些能力带入本地隔离会话中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.blog/changelog/2026-04-13-fix-merge-conflicts-in-three-clicks-with-copilot-cloud-agent/">Fix merge conflicts in three clicks with Copilot cloud agent</a></li>

</ul>
</details>

**标签**: `#GitHub`, `#Copilot`, `#AI`, `#developer-tools`, `#desktop-app`

---