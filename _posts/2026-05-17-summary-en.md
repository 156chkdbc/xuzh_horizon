---
layout: default
title: "Horizon Summary: 2026-05-17 (EN)"
date: 2026-05-17
lang: en
---

> From 35 items, 11 important content pieces were selected

---

1. [SGLang v0.5.12 Adds Full DeepSeek V4 Inference Support](#item-1) ⭐️ 9.0/10
2. [vllm v0.21.0: Breaking Changes, KV Offload, Blackwell Support](#item-2) ⭐️ 8.0/10
3. [2005 Sci-Fi Novel Accelerando Resonates with Today's AI Boom](#item-3) ⭐️ 8.0/10
4. [Frontier AI Breaks Open CTF Format](#item-4) ⭐️ 8.0/10
5. [δ-mem: Fixed-Size Memory for LLMs via Delta-Rule Learning](#item-5) ⭐️ 8.0/10
6. [Hashimoto warns of 'AI psychosis' in companies](#item-6) ⭐️ 8.0/10
7. [Apple-OpenAI alliance frays, OpenAI considers legal action](#item-7) ⭐️ 8.0/10
8. [Google Bans Manipulation of AI Search Results in Spam Policy](#item-8) ⭐️ 8.0/10
9. [71% of Americans Oppose Local AI Data Centers: Gallup](#item-9) ⭐️ 8.0/10
10. [Malta and OpenAI offer free ChatGPT Plus to all citizens](#item-10) ⭐️ 8.0/10
11. [GitHub Copilot Desktop App Enters Technical Preview](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [SGLang v0.5.12 Adds Full DeepSeek V4 Inference Support](https://github.com/sgl-project/sglang/releases/tag/v0.5.12) ⭐️ 9.0/10

SGLang v0.5.12 delivers comprehensive inference support for DeepSeek V4, including tensor parallelism, expert parallelism, context parallelism, data parallel attention, and optimizations like HiSparse KV cache offloading, DeepGemm, and FlashMLA kernels. This release is significant because it enables efficient deployment of DeepSeek V4, a state-of-the-art MoE model, reducing inference costs and improving throughput, which benefits the broader AI infrastructure ecosystem. The release also includes W4A4 MegaMoE kernels, prefill-decode disaggregation, HiCache with unified Radix Tree, and TokenSpeed MLA attention backend for Blackwell GPUs, plus a unified Docker image for all Nvidia GPUs.

github · Fridge003 · May 16, 18:23

**Background**: SGLang is an open-source LLM inference engine focused on high performance and ease of use. DeepSeek V4 is a large-scale Mixture-of-Experts (MoE) model from DeepSeek, which uses multiple expert sub-networks to increase capacity but requires complex inference. SGLang accelerates this process through various parallelism strategies and optimized kernels.

<details><summary>References</summary>
<ul>
<li><a href="https://www.lmsys.org/blog/2026-04-10-sglang-hisparse/">HiSparse : Turbocharging Sparse Attention with... | LMSYS Org</a></li>
<li><a href="https://docs.ray.io/en/latest/serve/llm/architecture/serving-patterns/prefill-decode.html">Prefill-decode disaggregation — Ray 2.55.1</a></li>

</ul>
</details>

**Tags**: `#DeepSeek`, `#SGLang`, `#inference`, `#GPU optimization`, `#MoE`

---

<a id="item-2"></a>
## [vllm v0.21.0: Breaking Changes, KV Offload, Blackwell Support](https://github.com/vllm-project/vllm/releases/tag/v0.21.0) ⭐️ 8.0/10

The vllm project released version 0.21.0 on March 26, 2025, with 367 commits from 202 contributors. It introduces breaking changes including deprecation of transformers v4 and a C++20 build requirement, alongside new features such as KV cache offloading with Hybrid Memory Allocator (HMA), speculative decoding with thinking budget support, and a TOKENSPEED_MLA attention backend for Blackwell GPUs. This release is significant for the LLM inference ecosystem as it lays the groundwork for future compatibility with transformers v5 and modern C++ standards, while also improving memory efficiency and inference speed through KV offloading and speculative decoding enhancements. The Blackwell GPU support enables high-performance inference for models like DeepSeek-R1 and Kimi-K2.5 on next-generation hardware. Notable technical details include the deprecation of transformers v4 in favor of v5, a mandatory C++20 compiler, and the integration of HMA for KV offloading which reduces memory waste by pooling memory across different layer types. The speculative decoding thinking budget feature ensures that reasoning token generation respects configured limits, and the TOKENSPEED_MLA backend uses optimized kernels for MLA (Multi-head Latent Attention) on Blackwell GPUs.

github · khluu · May 15, 08:44

**Background**: vLLM is an open-source inference engine for large language models that optimizes serving throughput and memory usage. The Hybrid Memory Allocator (HMA) is a new memory management scheme that groups layers by type (e.g., attention, SSM) and pools memory across them, reducing internal fragmentation. TOKENSPEED_MLA is a custom attention backend for Multi-head Latent Attention used in models like DeepSeek-R1, designed for high performance on NVIDIA's Blackwell architecture. Speculative decoding accelerates generation by using a smaller draft model to predict tokens that the target model then verifies in parallel; the 'thinking budget' extension ensures that reasoning models do not generate excessive thinking tokens.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/design/hybrid_kv_cache_manager/">Hybrid KV Cache Manager - vLLM</a></li>
<li><a href="https://docs.vllm.ai/en/latest/design/attention_backends/">Attention Backend Feature Support - vLLM</a></li>
<li><a href="https://x.com/lightseekorg/status/2055483456503914952">Excited to see TOKENSPEED_MLA integrated into vLLM on ...</a></li>

</ul>
</details>

**Tags**: `#LLM inference`, `#vllm`, `#breaking change`, `#KV cache`, `#speculative decoding`

---

<a id="item-3"></a>
## [2005 Sci-Fi Novel Accelerando Resonates with Today's AI Boom](https://www.antipope.org/charlie/blog-static/fiction/accelerando/accelerando.html) ⭐️ 8.0/10

Charles Stross's 2005 novel Accelerando, freely available online, has re-entered public discourse as readers draw parallels between its futuristic AI agents and today's generative AI and augmented reality tools. The novel's prescient depiction of AI-driven acceleration of society offers a unique lens to examine current technological trends, sparking deep reflection on the trajectory of AI development and its societal impact. Accelerando won the 2006 Locus Award and was nominated for Hugo, Campbell, Clarke, and BSFA awards; it is released under a Creative Commons license, making it widely accessible.

hackernews · eamag · May 16, 11:36 · [Discussion](https://news.ycombinator.com/item?id=48159241)

**Background**: Accelerando is a fix-up novel of interconnected short stories that follows a family over decades as they navigate a technological singularity where AI surpasses human intelligence. The story explores themes of posthumanism, virtual reality, and economic disruption, featuring characters who rely heavily on AI agents known as 'Aineko' and augmented reality glasses for daily tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Accelerando_(novel)">Accelerando (novel)</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters highlight how the novel's predictions about AI agents and dependency on augmented reality are becoming reality, with one user noting that the protagonist's loss of his glasses renders him helpless—a scenario now plausible with modern AI assistants. Others praise the novel's 'plausible weirdness' and recommend it alongside The Quantum Thief for its realistic portrayal of future weirdness.

**Tags**: `#science fiction`, `#AI`, `#agent systems`, `#futurism`, `#speculation`

---

<a id="item-4"></a>
## [Frontier AI Breaks Open CTF Format](https://kabir.au/blog/the-ctf-scene-is-dead) ⭐️ 8.0/10

Frontier AI models can now solve traditional CTF challenges instantly, undermining the learning and competition value of these cybersecurity events. CTFs are a key training ground for cybersecurity talent; if AI trivializes them, it could reduce hands-on learning and skill development, raising broader questions about AI's impact on education. The post notes that both playing and building CTF challenges are now 'ruined' by AI, with participants relying on LLMs to solve challenges in minutes; some suggest making CTFs harder but worry about crossing into 'too hard' territory.

hackernews · frays · May 16, 07:01 · [Discussion](https://news.ycombinator.com/item?id=48157559)

**Background**: CTF (Capture The Flag) competitions are cybersecurity contests where participants solve security-related challenges to find hidden 'flags'. They have been a popular method for learning and testing skills in hacking, cryptography, reverse engineering, and forensics. Frontier AI refers to the most advanced large language models like GPT-4, which can reason about and solve complex problems.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/ai-new-cybersecurity-frontier-why-trust-starts-identity-6mowc">AI and the New Cybersecurity Frontier : Why Trust Starts with Identity</a></li>
<li><a href="https://techitupme.com/sentinelone-unveils-wayfinder-frontier-ai-to-break-exploitation-chains/">SentinelOne Wayfinder Frontier AI Exposes Exploitation Chains</a></li>

</ul>
</details>

**Discussion**: Commenters expressed frustration that AI eliminates the collaborative learning experience, where teammates would spend hours together solving challenges. Some provided examples of using AI to deobfuscate code, and noted that the 'do it for me' mentality is hard to resist, leading to loss of genuine learning.

**Tags**: `#AI`, `#CTF`, `#cybersecurity`, `#education`, `#LLM`

---

<a id="item-5"></a>
## [δ-mem: Fixed-Size Memory for LLMs via Delta-Rule Learning](https://arxiv.org/abs/2605.12357) ⭐️ 8.0/10

Researchers have proposed δ-mem, a method that compresses past information into a fixed-size state matrix using delta-rule learning, enabling LLMs to retain and update memory efficiently without expanding the context window. This could significantly reduce the memory footprint of LLMs for long-term interactions, enabling more practical agents and assistants with effectively unlimited context while maintaining GPU efficiency. δ-mem uses a fixed-size state matrix updated via delta-rule learning, which is a gradient descent method for adjusting weights based on prediction errors. The paper does not explicitly mention computational cost but emphasizes fixed-size memory that can be stored and retrieved efficiently.

hackernews · 44za12 · May 16, 09:30 · [Discussion](https://news.ycombinator.com/item?id=48158506)

**Background**: Large language models (LLMs) like GPT-4 are trained on massive text data and generate responses. They struggle with long-term memory because the context window is limited and expanding it is expensive. Delta-rule learning is a weight update method from neural networks that minimizes error via gradient descent, commonly used in supervised learning.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2605.12357">$δ$-mem: Efficient Online Memory for Large Language Models</a></li>
<li><a href="https://en.wikipedia.org/wiki/Delta_rule">Delta rule - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Comments express interest in fixed-size memory for unlimited context, but some question whether it truly solves the capacity problem and note that slight input variations can create huge activation differences. Others suggest this approach could enable agents with essentially unlimited memory, but the cost is not discussed.

**Tags**: `#LLM`, `#memory`, `#efficiency`, `#online learning`, `#deep learning`

---

<a id="item-6"></a>
## [Hashimoto warns of 'AI psychosis' in companies](https://twitter.com/mitchellh/status/2055380239711457578) ⭐️ 8.0/10

Mitchell Hashimoto, creator of Vagrant and Consul, warned on Twitter that entire companies are suffering from 'AI psychosis'—blindly adopting AI tools without regard for long-term software infrastructure risks. This critique highlights a growing trend of overreliance on AI in software engineering, which can introduce hidden bugs, security vulnerabilities, and unsustainable technical debt, especially when management pressures teams to use AI for every task. Hashimoto's post sparked a discussion with 1906 points and 1103 comments, where engineers shared real-world examples such as FAANG management mandating daily token quotas and finance managers pushing AI adoption to win bragging contests.

hackernews · reasonableklout · May 15, 20:26 · [Discussion](https://news.ycombinator.com/item?id=48153379)

**Background**: The term 'AI psychosis' originally refers to a phenomenon where individuals develop psychosis from interacting with chatbots. In this context, Hashimoto uses it metaphorically to describe organizations that adopt AI tools irrationally, ignoring foundational risks to software infrastructure.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_psychosis">AI psychosis</a></li>
<li><a href="https://www.forbes.com/sites/truebridge/2026/04/27/the-ai-buildout-boom-is-real--but-so-are-the-risks/">The AI Buildout Boom Is Real – But So Are The Risks - Forbes</a></li>

</ul>
</details>

**Discussion**: Community comments reflected mixed sentiment: some engineers felt pressured to use AI even when it hinders productivity, while others expressed concerns about 'rotten foundations' and 'vibe coding' leading to catastrophic failures. A finance manager admitted their CFO wanted to accelerate AI usage just to keep up with peers.

**Tags**: `#AI`, `#software engineering`, `#overreliance`, `#industry criticism`, `#risk`

---

<a id="item-7"></a>
## [Apple-OpenAI alliance frays, OpenAI considers legal action](https://www.bloomberg.com/news/articles/2026-05-14/openai-apple-partnership-frays-setting-up-possible-legal-fight) ⭐️ 8.0/10

According to Bloomberg, Apple and OpenAI's partnership is deteriorating, with OpenAI exploring legal options over Apple's under-promotion of ChatGPT integration, which has led to subscription revenue far below expectations. Apple plans to open Siri to third-party models like Claude and Gemini at WWDC in June, further diluting OpenAI's exclusivity. This fracture between two industry giants could reshape the AI assistant landscape, potentially leading to a more open and competitive ecosystem for AI on mobile devices. The outcome may influence how other tech companies structure AI partnerships and revenue-sharing agreements. OpenAI claims that ChatGPT's entry point in Apple's system is hidden and functionally limited, causing most users to continue using the standalone app. Apple, meanwhile, is dissatisfied with OpenAI's privacy standards, hardware business, and poaching of engineers, and plans to integrate multiple AI models into iOS 27 Siri.

telegram · zaihuapd · May 15, 12:59

**Background**: Apple and OpenAI announced a partnership in 2024 to integrate ChatGPT into Siri, aiming to generate billions in subscription revenue. However, tensions have risen over marketing, revenue sharing, and strategic differences. Anthropic's Claude and Google's Gemini are competing large language models (LLMs) that Apple is now considering to integrate.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_(language_model)">Claude (language model) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gemini_(AI_model)">Gemini (AI model)</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#Apple`, `#AI partnership`, `#legal dispute`, `#WWDC`

---

<a id="item-8"></a>
## [Google Bans Manipulation of AI Search Results in Spam Policy](https://www.theverge.com/tech/931416/google-ai-search-spam-policy) ⭐️ 8.0/10

Google updated its Search spam policies to explicitly prohibit manipulating generative AI search responses, including AI Overviews and AI Mode, and to treat such tactics as spam. This policy directly targets the emerging practice of Generative Engine Optimization (GEO), affecting SEO professionals, content creators, and businesses that rely on AI-driven visibility, potentially reshaping optimization strategies for AI search. Violations include generating biased 'best-of' content at scale or embedding hidden prompts in web pages to influence AI models; penalties can range from ranking demotion to complete removal from search results.

telegram · zaihuapd · May 16, 06:31

**Background**: Generative Engine Optimization (GEO) is a practice of structuring content to increase visibility in AI-generated answers, similar to traditional SEO but for AI assistants like Google AI Overviews. Google has been facing a spam problem in AI Overviews, with examples of biased or inaccurate results. The updated policy applies existing spam rules to AI-generated search features.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theverge.com/tech/931416/google-ai-search-spam-policy">Google updates its spam rules to include attempts to ‘manipulate’ AI</a></li>
<li><a href="https://searchengineland.com/google-updates-search-spam-policies-to-clarify-it-applies-to-generative-ai-responses-477657">Google confirms spam policies apply to AI Overviews and AI Mode</a></li>
<li><a href="https://en.wikipedia.org/wiki/Generative_engine_optimization">Generative engine optimization - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Google`, `#AI search`, `#spam policy`, `#GEO`, `#SEO`

---

<a id="item-9"></a>
## [71% of Americans Oppose Local AI Data Centers: Gallup](https://news.gallup.com/poll/709772/americans-oppose-data-centers-area.aspx) ⭐️ 8.0/10

A March Gallup poll reveals that 71% of Americans oppose building AI data centers near their homes, with 48% strongly opposed, marking the first time Gallup has asked this question. This strong public opposition could influence AI infrastructure policy and siting decisions, as data center energy and water consumption become contentious environmental issues. Among opponents, roughly half cited high electricity and water usage, while others worried about pollution, noise, traffic, and rising living costs; supporters primarily mentioned jobs and tax revenue. The resistance to AI data centers was even stronger than to local nuclear power plants.

telegram · zaihuapd · May 16, 07:59

**Background**: AI data centers consume enormous amounts of electricity and water for computing and cooling. In 2024, U.S. data centers used 183 TWh of electricity, and water consumption from hyperscale facilities is projected to reach 33 billion gallons annually by 2028.

<details><summary>References</summary>
<ul>
<li><a href="https://www.eesi.org/articles/view/data-centers-and-water-consumption">Data Centers and Water Consumption | Article | EESI</a></li>
<li><a href="https://www.iea.org/news/data-centre-electricity-use-surged-in-2025-even-with-tightening-bottlenecks-driving-a-scramble-for-solutions">Data centre electricity use surged in 2025, even with tightening bottlenecks driving a scramble for solutions - News - IEA</a></li>

</ul>
</details>

**Tags**: `#AI`, `#data centers`, `#public opinion`, `#energy`, `#environment`

---

<a id="item-10"></a>
## [Malta and OpenAI offer free ChatGPT Plus to all citizens](https://openai.com/index/malta-chatgpt-plus-partnership/) ⭐️ 8.0/10

OpenAI and the Maltese government launched the 'AI for All' initiative, providing every Maltese citizen with one year of free ChatGPT Plus after completing an AI literacy course developed by the University of Malta. This is the first national-level partnership of its kind, potentially serving as a model for other countries to integrate AI literacy with accessible AI tools, accelerating AI adoption and education worldwide. The program begins in May, managed by the Malta Digital Innovation Authority, and will gradually extend to Maltese citizens living abroad. The AI literacy course covers both capabilities and responsibilities of AI.

telegram · zaihuapd · May 16, 10:40

**Background**: ChatGPT Plus is a premium subscription tier that offers faster response times, priority access to new features, and access to advanced models like GPT-4. AI literacy education is increasingly seen as crucial for responsible AI adoption, and this partnership directly ties learning to practical use.

**Tags**: `#OpenAI`, `#ChatGPT`, `#AI education`, `#government partnership`, `#Malta`

---

<a id="item-11"></a>
## [GitHub Copilot Desktop App Enters Technical Preview](https://github.blog/changelog/2026-05-14-github-copilot-app-is-now-available-in-technical-preview/) ⭐️ 8.0/10

GitHub has released a technical preview of its Copilot desktop app, allowing users to launch isolated development sessions from issues, PRs, prompts, or history, and to review changes, run tests, and create PRs within the app. It also introduces Agent Merge, which automatically handles review comments and merges. This desktop app marks a significant shift from Copilot being an IDE plugin to a standalone workflow hub, potentially streamlining developers' entire contribution cycle from ideation to merge. It could reduce context switching and improve productivity especially for teams using GitHub-centric workflows. Copilot Pro and Pro+ subscribers can immediately request early access, while Business and Enterprise users will get access within the week pending admin enabling the preview and CLI permissions in policies. The app supports agent-driven merge conflict resolution via Copilot Cloud Agent, a feature first teased in April 2026.

telegram · zaihuapd · May 16, 15:07

**Background**: GitHub Copilot is an AI pair programmer that traditionally operates as a plugin in IDEs like VS Code or JetBrains. The new desktop app aims to provide a more integrated environment for code review and PR management. Agent Merge, powered by Copilot Cloud Agent, automates the resolution of merge conflicts and review comments, reducing manual effort. Previous iterations allowed fixing merge conflicts with a single click on GitHub.com, but the desktop app brings these capabilities into a local, isolated session.

<details><summary>References</summary>
<ul>
<li><a href="https://github.blog/changelog/2026-04-13-fix-merge-conflicts-in-three-clicks-with-copilot-cloud-agent/">Fix merge conflicts in three clicks with Copilot cloud agent</a></li>

</ul>
</details>

**Tags**: `#GitHub`, `#Copilot`, `#AI`, `#developer-tools`, `#desktop-app`

---