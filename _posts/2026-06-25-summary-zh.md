---
layout: default
title: "Horizon Summary: 2026-06-25 (ZH)"
date: 2026-06-25
lang: zh
---

> From 34 items, 10 important content pieces were selected

---

1. [OpenAI 与博通联合发布首款自研芯片 Jalapeno](#item-1) ⭐️ 9.0/10
2. [高通以 40 亿美元收购 AI 初创公司 Modular](#item-2) ⭐️ 9.0/10
3. [Krea 2：开源权重 12B 图像模型发布](#item-3) ⭐️ 9.0/10
4. [美光创纪录 Q3：营收暴增 346%，日赚 31 亿美元](#item-4) ⭐️ 9.0/10
5. [Anthropic 指控阿里巴巴发动大规模 Claude 蒸馏攻击](#item-5) ⭐️ 9.0/10
6. [NVIDIA 45°C 液冷设计将数据中心用水降至接近零](#item-6) ⭐️ 8.0/10
7. [Nub：类 Bun 的 Node.js 一站式工具包](#item-7) ⭐️ 8.0/10
8. [生成式 AI 做作业或降低考试分数](#item-8) ⭐️ 8.0/10
9. [Cloudflare 等联合提议 PACT 协议替代验证码](#item-9) ⭐️ 8.0/10
10. [谷歌 Play 向美英欧开放外部计费](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI 与博通联合发布首款自研芯片 Jalapeno](https://techcrunch.com/2026/06/24/openai-unveils-its-first-custom-chip-built-by-broadcom/) ⭐️ 9.0/10

OpenAI 与博通联合推出 Jalapeño——一款专为大语言模型设计的自定义 AI 推理芯片，由台积电制造，研发周期仅九个月。 这标志着 OpenAI 进入定制 AI 硬件领域，有望减少对英伟达 GPU 的依赖，并在大规模推理中提高能效。 早期测试显示 Jalapeño 的每瓦性能显著优于现有方案，且芯片设计过程中使用了 OpenAI 自身的 AI 模型进行加速。

hackernews · jamdesk · Jun 24, 17:47 · [社区讨论](https://news.ycombinator.com/item?id=48663324)

**背景**: AI 推理芯片是专为高效运行已训练机器学习模型而设计的专用硬件。像谷歌这样的公司已经开发了自己的张量处理单元（TPU）用于类似目的。自定义芯片可以针对特定工作负载进行优化，在成本和性能上可能优于通用 GPU。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/openai-broadcom-jalapeno-inference-chip/">OpenAI and Broadcom unveil LLM-optimized inference chip</a></li>
<li><a href="https://www.techpowerup.com/forums/threads/openai-unveils-jalapeno-llm-inferencing-accelerator-built-in-collaboration-with-broadcom.350253/">OpenAI Unveils Jalapeno LLM Inferencing Accelerator Built in ...</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：部分用户对所谓的 AI 加速设计流程表示怀疑，认为这不过是营销话术；而另一些人则称赞潜在的效率提升，并将此举与谷歌的 TPU 战略相提并论。还有评论者讨论了将模型权重直接烧录进硅片等替代方案。

**标签**: `#OpenAI`, `#custom chip`, `#AI hardware`, `#Broadcom`, `#inference`

---

<a id="item-2"></a>
## [高通以 40 亿美元收购 AI 初创公司 Modular](https://www.reuters.com/business/qualcomm-buy-ai-startup-modular-2026-06-24/) ⭐️ 9.0/10

高通于 2026 年 6 月 24 日宣布以约 40 亿美元收购 Modular，该公司是 Mojo 编程语言和 MAX AI 推理栈的开发者。 此次收购增强了高通的 AI 推理能力，提供了 NVIDIA CUDA 栈的替代方案，并可能加速基于 ARM 的规模化 AI 推理的普及。 交易包括 Modular 的 Mojo 语言（通过 MLIR 编译器框架将类似 Python 的语法与高性能相结合）以及用于异构硬件推理的 MAX 框架。Mojo 预计将在 2026 年秋季开源。

hackernews · timmyd · Jun 24, 13:49 · [社区讨论](https://news.ycombinator.com/item?id=48659798)

**背景**: Mojo 是一种为 AI 基础设施设计的编程语言，利用 MLIR 编译器框架支持 CPU、GPU 和加速器，同时保持与 Python 的兼容性。Modular 还开发了 MAX，一个硬件无关的推理服务框架，用于高效部署 AI 模型。高通作为领先的 ARM 芯片设计商，一直扩展其 AI 产品组合，以在数据中心和边缘 AI 市场与 NVIDIA 等公司竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mojo_(programming_language)">Mojo (programming language)</a></li>
<li><a href="https://www.modular.com/">Modular: Inference from Kernel to Cloud</a></li>
<li><a href="https://github.com/modular/modular">GitHub - modular/modular: The Modular Platform (includes MAX & Mojo) · GitHub</a></li>

</ul>
</details>

**社区讨论**: 社区评论对收购之早感到意外，并对 Mojo 的发展方向看法不一，有人认为这浪费了 Chris Lattner 的才华。另一些人则看到了对 ARM vs NVIDIA 和 RISC-V 的战略影响，并指出高通近期在构建 AI 相关技术方面的举措。

**标签**: `#acquisition`, `#AI`, `#compilers`, `#Qualcomm`, `#Modular`

---

<a id="item-3"></a>
## [Krea 2：开源权重 12B 图像模型发布](https://www.krea.ai/blog/krea-2-technical-report) ⭐️ 9.0/10

Krea AI 发布了 Krea 2，这是一个最先进的开源权重 12B 参数文本到图像模型，并附带详细的技术报告，涵盖数据整理、架构和训练基础设施。此次发布包括两个版本：Krea 2 和 Krea 2 Turbo（蒸馏版本，推理速度更快）。 此次发布显著推动了开源 AI 图像生成的发展，因为 Krea 2 在与领先的闭源模型竞争的同时，提供了开源权重并可在本地部署。这使得开发者和研究人员能够定制和部署高质量图像生成，而无需依赖专有 API。 Krea 2 Turbo 模型结合了引导蒸馏和时间步蒸馏，可在低至 8 步内实现快速生成，性能优于许多其他本地可部署模型。技术报告提供了前所未有的细节，涵盖数据整理、字幕生成、模型架构、后期训练、强化学习流水线、提示扩展和风格参考。

hackernews · mattnewton · Jun 23, 15:31 · [社区讨论](https://news.ycombinator.com/item?id=48646659)

**背景**: 开源权重模型提供了训练好的神经网络权重，但可能不包含完整的训练数据或流程，用户可在足够硬件的支持下本地运行。12B 参数的图像生成模型规模较大，需要大量计算资源但能提供高质量。这体现了开源模型追赶专有模型的趋势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Large_language_model">Large language model - Wikipedia</a></li>
<li><a href="https://huggingface.co/blog/daya-shankar/open-source-llms">Best Open -Source LLM Models in 2026: Coding, Local, Agentic AI ...</a></li>
<li><a href="https://www.ibm.com/think/topics/mistral-ai">What is Mistral AI? | IBM</a></li>

</ul>
</details>

**社区讨论**: 作者积极回应评论，强调技术报告的详细程度和两个版本的发布。一位评论者称赞 Turbo 模型的速度和竞争力，指出它超越了大多数本地可部署模型（仅次于 Ideogram 4），同时提到了常见的失败案例。另一位评论者欣赏开源权重，但质疑该方法在新型组合模型出现后的相关性。

**标签**: `#AI`, `#image generation`, `#open-weights`, `#machine learning`, `#text-to-image`

---

<a id="item-4"></a>
## [美光创纪录 Q3：营收暴增 346%，日赚 31 亿美元](https://www.globenewswire.com/news-release/2026/06/24/3317151/14450/en/micron-technology-inc-reports-record-results-for-the-third-quarter-of-fiscal-2026.html) ⭐️ 9.0/10

美光公布 2026 财年第三季度财报，营收达 4146 亿美元，同比增长 346%，净利润 2824 亿美元，相当于每天净赚 31 亿美元。 这一惊人业绩突显了 AI 对高带宽内存的爆发式需求，使美光成为 AI 基础设施建设的最大受益者之一，并预示内存短缺将持续，可能迫使竞争对手加速 HBM 生产。 数据中心营收暴增 653%至 1152 亿美元，非 GAAP 毛利率升至 84.9%。美光已开始大规模量产 HBM4，预计 2027 年投产 HBM4E，并签署了 16 份长期战略协议。

telegram · zaihuapd · Jun 24, 22:22

**背景**: 高带宽内存（HBM）是一种 3D 堆叠 DRAM 技术，与传统 DDR 内存相比可提供显著更高的带宽，对 AI 加速器和高性能 GPU 至关重要。HBM4 是最新一代，而 HBM4E 是增强版，预计将提供更快的速度和更高的效率。内存行业正竞相大规模量产这些下一代芯片以满足 AI 基础设施需求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://nerds.xyz/2026/06/samsung-hbm4e-memory/">Samsung ships industry-first HBM 4 E memory as AI infrastructure race...</a></li>

</ul>
</details>

**标签**: `#Micron`, `#semiconductors`, `#AI infrastructure`, `#memory`, `#earnings`

---

<a id="item-5"></a>
## [Anthropic 指控阿里巴巴发动大规模 Claude 蒸馏攻击](https://www.cnbc.com/2026/06/24/anthropic-alibaba-distillation-campaign.html) ⭐️ 9.0/10

2026 年 6 月 10 日，Anthropic 致信美国参议院银行委员会，指控阿里巴巴及其 Qwen 实验室发动了针对 Claude 的迄今最大规模蒸馏攻击，使用约 2.5 万个欺诈账户在 2026 年 4 月 22 日至 6 月 5 日期间进行了超过 2880 万次交互。 这一指控凸显了中美之间日益加剧的人工智能知识产权紧张局势，可能影响国际技术竞争和 AI 安全实践。同时，它强调了前沿 AI 模型面对蒸馏攻击的脆弱性，可能削弱竞争优势和安全控制。 该信函是在国会 AI 听证会前夕发送的，并提及了美国早前的行动，包括白宫 4 月指责中国窃取 AI 知识产权，以及 6 月 12 日商务部对 Anthropic 的 Mythos 和 Fable 模型实施出口限制。阿里巴巴尚未回应这些指控。

telegram · zaihuapd · Jun 25, 01:36

**背景**: 蒸馏攻击是指用较弱的模型通过学习较强模型的输出来复制其能力。2026 年，此类攻击已成为主要的 AI 安全问题；Anthropic 此前曾在 2026 年 2 月指控三家中国 AI 公司（DeepSeek、Kimi、MiniMax）实施类似攻击。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://jangwook.net/zh/blog/zh/ai-distillation-attacks-enterprise-defense/">AI 模型 蒸 馏 攻 击 实态——CTO必知的IP保护策略</a></li>
<li><a href="https://zmyx.net/knowledge-distillation-or-distillation-theft/">中美 AI 博弈的最新焦点：“知识 蒸 馏 ”和“ 蒸 馏 攻 击 ” - 中美印象</a></li>

</ul>
</details>

**标签**: `#AI security`, `#distillation attack`, `#Anthropic`, `#Alibaba`, `#geopolitics`

---

<a id="item-6"></a>
## [NVIDIA 45°C 液冷设计将数据中心用水降至接近零](https://blogs.nvidia.com/blog/liquid-cooling-ai-factories/) ⭐️ 8.0/10

NVIDIA 推出了一种用于 AI 数据中心的新型液冷架构，使用高达 45°C 的冷却液，通过在许多气候条件下实现干冷却或自由冷却，大幅降低用水量。 随着 AI 工作负载带来前所未有的热密度，这一设计解决了水短缺问题，并为区域供暖协同打开大门，有可能将数据中心转变为当地热源。 该冷却方案采用直接芯片级液冷，冷却液温度高达 45°C (113°F)，高于传统液冷回路，并且在有利气候条件下效果尤佳，可利用环境空气冷却冷却液。

hackernews · nitin_flanker · Jun 24, 14:10 · [社区讨论](https://news.ycombinator.com/item?id=48660178)

**背景**: 传统数据中心依赖高能耗的空调或冷冻水系统，通过蒸发冷却消耗大量水资源。液冷可直接带走芯片热量，而提高冷却液温度后可使用干冷却或非蒸发排热。区域供暖网络可利用约 45°C 的低品位热量为建筑供暖，从而形成潜在的协同效应。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.guru3d.com/story/nvidia-unveils-liquid-cooling-design-for-ai-data-centers/">NVIDIA Unveils 45 ° C Liquid Cooling Design for AI Data Centers</a></li>
<li><a href="https://www.techbuzz.ai/articles/nvidia-s-45-c-liquid-cooling-redefines-ai-data-center-energy">NVIDIA's 45 ° C Liquid Cooling Redefines AI Data Center Energy</a></li>
<li><a href="https://www.araner.com/blog/data-center-and-district-heating-an-outstanding-combination">Data center and district heating : an outstanding combination</a></li>

</ul>
</details>

**社区讨论**: 社区成员注意到区域供暖协同的潜力，有评论者建议数据中心可免费向社区供热。也有人质疑创新性，指出更高冷却液温度并非新事，并要求更多关于气候依赖性的细节。还有评论提到了 NASA 类似的高温水冷却方案。

**标签**: `#data center`, `#cooling`, `#water conservation`, `#sustainability`, `#AI infrastructure`

---

<a id="item-7"></a>
## [Nub：类 Bun 的 Node.js 一站式工具包](https://github.com/nubjs/nub) ⭐️ 8.0/10

Nub 是一个新的工具包，通过预加载钩子和基于 oxc 的转译，为 Node.js 提供类 Bun 的开发体验。 它显著改善了 Node.js 开发体验，带来了快速的 TypeScript 转译和 polyfill，同时无需离开 Node.js 生态系统。 Nub 使用--require 预加载钩子集成基于 oxc 的转译器作为 Node-API 插件，并注册模块解析钩子，纯粹以附加方式注入如 Worker 和 Temporal 等 API 的 polyfill。

hackernews · colinmcd · Jun 24, 14:14 · [社区讨论](https://news.ycombinator.com/item?id=48660267)

**背景**: Bun 是一个一体化 JavaScript 运行时，内置转译和包管理。Node.js 传统上需要单独工具支持 TypeScript。Nub 利用 Node 的--require 钩子和高性能 oxc 转译器（Rust 编写），在原生 Node.js 之上模拟 Bun 的流畅开发体验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://git-stars.org/repositories/topic/transpiler">Top transpiler Repositories - GitHub Projects for transpiler ... | Git Stars</a></li>
<li><a href="https://stackoverflow.com/questions/67256729/difference-between-nodejs-preload-option-r-and-explicit-require-in-in-repl">javascript - Difference between NodeJs preload ... - Stack Overflow</a></li>

</ul>
</details>

**社区讨论**: 社区评论普遍积极，称赞该概念及作者的可信度。技术讨论围绕选择--require 而非--import 对 ESM 支持的影响，以及在 Node 原生支持 TypeScript 下是否需要转译器。一些用户报告无缝迁移到 Nub。

**标签**: `#Node.js`, `#TypeScript`, `#Bun`, `#developer-tools`, `#toolkit`

---

<a id="item-8"></a>
## [生成式 AI 做作业或降低考试分数](https://cepr.org/publications/dp21577) ⭐️ 8.0/10

一项对 26811 名中国 7 至 12 年级学生、持续 30 个月的追踪研究发现，生成式 AI 虽能让作业成绩平均提高 18%、完成时间减少 30%，却导致中考、高考等高风险考试成绩降低 18%至 24%，且全部影响在约两年后充分显现。 这项大规模实证研究提供了有力证据，表明依赖生成式 AI 完成作业可能损害深度学习与考试成绩，引发对 AI 工具融入教育的担忧，并凸显制定平衡使用政策的必要性。 研究发现，社科科目分数下降最多，其次是理工科和语言类；低年级、高成就学生和男生受影响更明显。约 80%的 AI 用户表现出‘作业外包’特征——作业时间极短但分数高，这些学生承担了主要损失。

telegram · zaihuapd · Jun 24, 05:15

**背景**: 生成式 AI（如大型语言模型 GPT、Claude 等）能够生成连贯文本并解决问题，容易诱使学生用于完成作业。但这可能绕过了闭卷考试所需的知识内化过程。本研究追踪了 26811 名中国学生长达 30 个月，以评估长期影响。

**标签**: `#generative AI`, `#education`, `#exam performance`, `#empirical study`, `#impact analysis`

---

<a id="item-9"></a>
## [Cloudflare 等联合提议 PACT 协议替代验证码](https://www.techtimes.com/articles/318891/20260623/cloudflare-chrome-firefox-plan-replace-captchas-cryptographic-tokens.htm) ⭐️ 8.0/10

Cloudflare 联合 Chrome、Firefox、Edge 和 Shopify 提出 PACT 协议，拟用基于 Privacy Pass 盲签名的匿名加密令牌替代 CAPTCHA。 该协议有望消除烦人的验证码挑战，同时保护用户隐私——令牌不会泄露身份或浏览记录，还能区分合法 AI 代理与恶意爬虫。 PACT 协议目前仍是提案，尚未确定标准组织或时间表，苹果未加入，令牌发行方的治理问题也未解决。

telegram · zaihuapd · Jun 24, 06:30

**背景**: 验证码广泛用于区分人类和机器人，但常常不便且无障碍性差。Privacy Pass 是 IETF 标准，利用盲签名实现匿名令牌验证——令牌在签名者不看到内容的情况下被签名，确保不可链接性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://privacypass.github.io/">Privacy Pass</a></li>
<li><a href="https://en.wikipedia.org/wiki/Blind_signature">Blind signature</a></li>

</ul>
</details>

**标签**: `#web security`, `#CAPTCHA replacement`, `#cryptographic tokens`, `#privacy`

---

<a id="item-10"></a>
## [谷歌 Play 向美英欧开放外部计费](https://android-developers.googleblog.com/2026/06/play-expanded-billing.html) ⭐️ 8.0/10

谷歌宣布自 6 月 30 日起，在美国、英国和欧洲经济区，开发者可以向用户提供外部计费选项，并采用重新调整的服务费结构，将 Play 服务费与计费费分离。 此次扩展是 Google Play 最大规模的外部计费部署，很可能是对监管压力的回应，可能通过给予开发者更多灵活性和潜在更低费用，从根本上改变应用分发的经济模式。 首 100 万美元年收入和自动续订订阅的服务费为 10%；其他交易分为“新安装”和“现有安装”。在这些地区，仅当使用 Google Play Billing 时才需额外支付 5%的计费费。

telegram · zaihuapd · Jun 25, 02:33

**背景**: 传统上，Google Play 要求开发者使用其自有计费系统，并收取 15-30%的佣金。外部计费允许开发者使用第三方支付处理商，从而减少谷歌的分成。新结构将服务费（用于 Play 平台服务）与计费费（用于支付处理）分离。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.android.com/google/play/billing/external">External offers APIs | Play Billing | Android Developers</a></li>
<li><a href="https://play.google.com/console/about/">Google Play for business | Launch & monetize your apps</a></li>

</ul>
</details>

**标签**: `#Google Play`, `#external billing`, `#antitrust`, `#developer policy`, `#mobile ecosystem`

---