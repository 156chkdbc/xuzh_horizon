---
layout: default
title: "Horizon Summary: 2026-07-13 (EN)"
date: 2026-07-13
lang: en
---

> From 32 items, 10 important content pieces were selected

---

1. [vLLM v0.25.0: Model Runner V2 Default, PagedAttention Removed](#item-1) ⭐️ 9.0/10
2. [GPT-5.6 Solves 50-Year-Old Graph Theory Conjecture in 1 Hour](#item-2) ⭐️ 9.0/10
3. [OpenAI Unveils GPT-5.6 Series: Sol, Terra, Luna with Enhanced Capabilities](#item-3) ⭐️ 9.0/10
4. [World's First Invasive BCI Medical Device Approved in China](#item-4) ⭐️ 9.0/10
5. [Terry Tao Builds Apps with LLM Coding Agents](#item-5) ⭐️ 8.0/10
6. [Study: Claude Code wastes 33k tokens before prompt, OpenCode uses 7k](#item-6) ⭐️ 8.0/10
7. [I love LLMs, I hate hype](#item-7) ⭐️ 8.0/10
8. [Apple Sues OpenAI for Stealing Trade Secrets for Hardware](#item-8) ⭐️ 8.0/10
9. [xAI Grok CLI Uploads Entire Codebase and Secrets by Default](#item-9) ⭐️ 8.0/10
10. [Cursor Develops 'Sand' AI Agent to Rival Claude Cowork](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [vLLM v0.25.0: Model Runner V2 Default, PagedAttention Removed](https://github.com/vllm-project/vllm/releases/tag/v0.25.0) ⭐️ 9.0/10

vLLM v0.25.0 was released with 558 commits from 232 contributors. Model Runner V2 is now the default for all dense models, legacy PagedAttention has been removed, and the Transformers backend achieves native vLLM speed. This release marks a major architectural simplification by removing PagedAttention and standardizing on MRv2, leading to cleaner code and potentially better performance. Transformers backend parity allows users to adopt a familiar interface without sacrificing speed, broadening vLLM's appeal. MRv2 now supports EVS, realtime embeddings, prefix caching for Mamba hybrid models, multimodal-prefix bidirectional attention, and dynamic speculative decoding with full CUDA graphs. New models added include LLaVA-OneVision-2, Unlimited OCR, MOSS-Transcribe-Diarize, openai/privacy-filter, and Hy3.

github · khluu · Jul 11, 20:06

**Background**: vLLM is an open-source library for high-performance LLM inference and serving. Model Runner V2 (MRv2) is a ground-up reimplementation of the execution core designed for better modularity and efficiency. PagedAttention was the original attention mechanism; its removal indicates full adoption of the newer V1 and MRv2 backends.

<details><summary>References</summary>
<ul>
<li><a href="https://vllm-website-5zwgmvte0-inferact-inc.vercel.app/blog/mrv2">Model Runner V 2 : A Modular and Faster Core for vLLM | vLLM Blog</a></li>
<li><a href="https://docs.vllm.ai/en/latest/design/model_runner_v2/">Model Runner V 2 Design Document - vLLM</a></li>
<li><a href="https://huggingface.co/blog/dynamic_speculation_lookahead">Faster Assisted Generation with Dynamic Speculation</a></li>

</ul>
</details>

**Tags**: `#vllm`, `#LLM inference`, `#AI frameworks`, `#open source`, `#performance`

---

<a id="item-2"></a>
## [GPT-5.6 Solves 50-Year-Old Graph Theory Conjecture in 1 Hour](https://www.qbitai.com/2026/07/447873.html) ⭐️ 9.0/10

OpenAI's GPT-5.6 Sol Ultra proved the cycle double cover conjecture, an open problem in graph theory for nearly 50 years, in under an hour by coordinating 64 parallel sub-agents and using a carefully crafted prompt. This achievement demonstrates advanced reasoning and multi-agent coordination in AI, marking a paradigm shift in how mathematical research can be conducted. It suggests that large language models can solve deep theoretical problems that have stumped human mathematicians for decades. The proof was generated in under one hour and produced a 3-page PDF. The model transformed the problem into edge labeling and linear equations over finite fields, and OpenAI released the full 700-character prompt that specified acceptance criteria, definitions, boundary conditions, and failure cases without prescribing steps.

telegram · zaihuapd · Jul 12, 03:49

**Background**: The cycle double cover conjecture asks whether every bridgeless graph has a collection of cycles that together contain each edge exactly twice. A bridge in a graph is an edge whose removal increases the number of connected components. This conjecture was independently posed by Szekeres (1973) and Seymour (1979) and is a central open problem in graph theory.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cycle_double_cover_conjecture">Cycle double cover conjecture</a></li>
<li><a href="https://en.wikipedia.org/wiki/Bridge_(graph_theory)">Bridge (graph theory)</a></li>
<li><a href="https://mathworld.wolfram.com/CycleDoubleCoverConjecture.html">Cycle Double Cover Conjecture -- from Wolfram MathWorld</a></li>

</ul>
</details>

**Tags**: `#AI`, `#graph theory`, `#GPT-5.6`, `#breakthrough`, `#mathematics`

---

<a id="item-3"></a>
## [OpenAI Unveils GPT-5.6 Series: Sol, Terra, Luna with Enhanced Capabilities](https://t.me/zaihuapd/42512) ⭐️ 9.0/10

OpenAI announced the GPT-5.6 model family on June 26, 2026, with three variants: Sol (flagship for maximum power), Terra (balanced performance and cost), and Luna (low-cost for high concurrency). The series brings significant improvements in code generation, knowledge work, design, research, and cybersecurity, and introduces max/ultra reasoning modes, multi-agent collaboration, and Programmatic Tool Calling. This release makes advanced AI more accessible and cost-effective via tiered pricing, allowing organizations to choose the right capability level for their needs. The inclusion of reasoning modes and agentic features like multi-agent collaboration pushes the boundaries of autonomous task completion, potentially transforming workflows in coding, research, and security. GPT-5.6 defaults to Sol for general use; Terra offers balanced pricing for most workloads, while Luna is optimized for high concurrency and low cost. The 'max' reasoning mode enables deeper thinking, and 'ultra' mode uses subagents to accelerate complex tasks; Programmatic Tool Calling allows models to interact programmatically with external APIs and tools.

telegram · zaihuapd · Jul 12, 11:19

**Background**: OpenAI's GPT series evolves quickly, with GPT-5.5 released just two months prior. The tiered approach mirrors industry trends toward specialized models for different use cases. Programmatic Tool Calling extends function calling capabilities, enabling autonomous workflows by allowing the model to invoke tools and APIs in a structured way. ChatGPT Work is a new agent designed to turn goals into finished outputs by connecting tools and automating tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.digitalapplied.com/blog/gpt-5-6-sol-terra-luna-preview-guide-2026">GPT - 5 . 6 Sol , Terra & Luna : OpenAI's New Model Family</a></li>
<li><a href="https://www.linkedin.com/posts/vaibhavs10_introducing-gpt-56-sol-terra-and-luna-activity-7476322117161058304-W_mZ">Introducing GPT - 5 . 6 : Sol , Terra and Luna . Sol is our strongest...</a></li>
<li><a href="https://openai.com/index/chatgpt-for-your-most-ambitious-work/">ChatGPT is now a partner for your most ambitious work - OpenAI</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#GPT-5.6`, `#Large Language Models`, `#AI`, `#Generative AI`

---

<a id="item-4"></a>
## [World's First Invasive BCI Medical Device Approved in China](https://t.me/zaihuapd/42515) ⭐️ 9.0/10

China's National Medical Products Administration approved the world's first invasive brain-computer interface medical device, a hand function restoration system for spinal cord injury patients, developed by BrainCo Medical Technology. This marks the first regulatory approval and commercial launch of such a device globally. This approval represents a paradigm shift in neurotechnology, moving brain-computer interfaces from research to clinical application. It offers new hope for quadriplegic patients to regain hand function, potentially improving millions of lives and accelerating investment in BCI technologies. The device uses a minimally invasive epidural implantation technique with wireless power and data transmission, and it assists hand grasping via a pneumatic glove. It is indicated for patients aged 18–60 with tetraplegia due to cervical spinal cord injury.

telegram · zaihuapd · Jul 12, 14:39

**Background**: Brain-computer interfaces (BCIs) enable direct communication between the brain and external devices. Invasive BCIs, which require surgical implantation, typically offer higher signal fidelity but pose greater risks. Previous BCI approvals have been limited to non-invasive or partially invasive systems; this is the first fully invasive BCI to receive regulatory clearance for clinical use.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ecns.cn/m/news/sci-tech/2026-03-17/detail-ihfaunkv7709855.shtml">China approves world's first invasive BCI medical device</a></li>
<li><a href="https://trial.medpath.com/news/china-approves-world-s-first-commercial-brain-computer-interface-for-spinal-cord-injury-treatment">China Approves World's First Commercial Brain - Computer Interface ...</a></li>

</ul>
</details>

**Tags**: `#brain-computer interface`, `#medical device`, `#regulatory approval`, `#neurotechnology`, `#spinal cord injury`

---

<a id="item-5"></a>
## [Terry Tao Builds Apps with LLM Coding Agents](https://terrytao.wordpress.com/2026/07/11/old-and-new-apps-via-modern-coding-agents/) ⭐️ 8.0/10

Fields Medalist Terry Tao used modern LLM coding agents to build visualizations and simple interactive applications for his research papers, demonstrating the accessibility of AI-assisted coding for non-mission-critical tasks. This highlights that AI coding tools are becoming powerful enough for domain experts outside software engineering to create custom software, potentially democratizing software creation for scientists, educators, and hobbyists. Tao noted that since such visualizations are supplements and not mission-critical to his papers, the downside risk of using LLM agents is acceptable, reflecting a pragmatic view of AI trustworthiness.

hackernews · subset · Jul 12, 11:09 · [Discussion](https://news.ycombinator.com/item?id=48880170)

**Background**: LLM coding agents are AI systems that use large language models to write and debug code based on natural language instructions. They can generate complete applications or visualizations from user prompts, lowering the barrier to software development. Such tools have gained traction in education and prototyping, allowing non-programmers to create functional software.

<details><summary>References</summary>
<ul>
<li><a href="https://zencoder.ai/">Zencoder | The AI Coding Agent</a></li>

</ul>
</details>

**Discussion**: Community comments express enthusiasm for LLM-assisted coding, with one user noting it has boosted their CS classes by enabling visualizations they lacked time to build. Another humorously compared Tao's embrace of coding agents to a Michelin-star chef discovering microwave dinners. A comment highlighted the infinite latent demand for software outside traditional spaces, while others appreciated Tao's balanced perspective on trust.

**Tags**: `#LLM`, `#coding agents`, `#software development`, `#education`, `#visualization`

---

<a id="item-6"></a>
## [Study: Claude Code wastes 33k tokens before prompt, OpenCode uses 7k](https://systima.ai/blog/claude-code-vs-opencode-token-overhead) ⭐️ 8.0/10

An empirical study found that Claude Code consumes approximately 33,000 tokens in harness overhead before processing a user prompt, while OpenCode uses only about 7,000 tokens, revealing a significant inefficiency in token consumption. This overhead directly impacts developers' costs and API usage budgets, making OpenCode a more token-efficient choice for agentic coding tasks. It also raises questions about whether Anthropic's design incentivizes higher token consumption. The study logged all requests between the coding tools and Anthropic's endpoint, comparing cache strategies and harness token usage. The authors plan to follow up with more in-depth tasks and qualitative comparisons to address community feedback.

hackernews · systima · Jul 12, 18:25 · [Discussion](https://news.ycombinator.com/item?id=48883275)

**Background**: Tokens are units of text that language models process; each token incurs a cost and contributes to context window limits. Agentic coding tools like Claude Code and OpenCode use system prompts and harness code to orchestrate autonomous coding workflows, which adds overhead. This overhead can vary significantly between tools, affecting both speed and cost.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kdnuggets.com/the-beginners-guide-to-tracking-token-usage-in-llm-apps">The Beginner’s Guide to Tracking Token Usage in LLM ... - KDnuggets</a></li>
<li><a href="https://cloud.google.com/discover/what-is-agentic-coding">What is agentic coding? How it works and use cases | Google Cloud</a></li>
<li><a href="https://www.tembo.io/blog/agentic-ai-coding-tools">Best Agentic AI Coding Tools in 2026: Compared - Tembo.io</a></li>

</ul>
</details>

**Discussion**: Commenters noted that sub-agents burn tokens heavily, with one user reporting 7 sub-agents exhausting their budget before any finished. Others suspected Anthropic profits from token inflation and that tools like pi use even fewer tokens. The study author acknowledged a valid critique about measuring the right metric and promised to improve the analysis.

**Tags**: `#AI coding tools`, `#token efficiency`, `#Claude Code`, `#OpenCode`, `#LLM overhead`

---

<a id="item-7"></a>
## [I love LLMs, I hate hype](https://geohot.github.io//blog/jekyll/update/2026/07/12/i-love-llms.html) ⭐️ 8.0/10

George Hotz published a blog post reflecting on the hype surrounding large language models, arguing that while LLMs create immense value, the frontier labs may not capture it. This critique challenges the sky-high valuations of AI companies and raises important questions about who benefits from AI advancements, impacting investors, developers, and the open source community. The post's main argument is that value creation does not equal value capture, which explains why frontier labs push token-based pricing models while open source alternatives flourish.

hackernews · therepanic · Jul 12, 18:31 · [Discussion](https://news.ycombinator.com/item?id=48883343)

**Discussion**: Commenters largely agree with the value capture argument, with some noting that LLMs have boosted their personal productivity for niche software, but also expressing concern about the future of open source maintenance due to the ease of forking.

**Tags**: `#LLMs`, `#hype`, `#value capture`, `#open source`, `#productivity`

---

<a id="item-8"></a>
## [Apple Sues OpenAI for Stealing Trade Secrets for Hardware](https://t.me/zaihuapd/42502) ⭐️ 8.0/10

On July 10, Apple filed a lawsuit in the U.S. District Court for the Northern District of California against OpenAI, two former employees, and io Products, alleging systematic theft of trade secrets related to product design, manufacturing processes, and supply chain to accelerate OpenAI's consumer hardware development. This high-stakes legal battle between two tech giants could reshape AI hardware competition and set precedents for trade secret protection in the industry. If Apple prevails, it may slow OpenAI's hardware ambitions and deter other companies from poaching talent for confidential information. Apple specifically alleges that former employee Chang Liu accessed internal networks after leaving and downloaded dozens of hardware files, while OpenAI's hardware head Tang Yew Tan sent supplier information to his personal email before resignation and asked job candidates to bring Apple components to interviews. Apple also claims that over 20 former employees have been hired by OpenAI, raising concerns about systematic information leakage.

telegram · zaihuapd · Jul 11, 16:29

**Background**: Apple has long invested heavily in custom hardware, including chips (A-series, M-series) and products like Vision Pro, making its design and supply chain details highly confidential. OpenAI, best known for software like ChatGPT, has been expanding into hardware, reportedly developing AI-specific devices. Trade secret lawsuits are common in Silicon Valley, but this case involves two prominent companies with significant resources, making it particularly notable.

**Tags**: `#Apple`, `#OpenAI`, `#trade secrets`, `#legal`, `#hardware`

---

<a id="item-9"></a>
## [xAI Grok CLI Uploads Entire Codebase and Secrets by Default](https://gist.github.com/cereblab/dc9a40bc26120f4540e4e09b75ffb547) ⭐️ 8.0/10

Security researchers discovered that xAI's Grok Build CLI (version 0.2.93) uploads entire code repositories and sensitive files like .env to xAI servers by default, even with the privacy toggle disabled; xAI subsequently deployed a server-side fix on July 13 adding a disable_codebase_upload field. This flaw poses a critical security and privacy risk for developers using the tool, potentially leaking proprietary code, credentials, and secrets to external servers without consent, which could severely undermine trust in xAI's tooling and AI-assisted development platforms. Packet capture analysis showed that files read by the tool are embedded into model requests and also uploaded to a Google Cloud Storage bucket; entire repositories are uploaded as git bundles even if the prompt explicitly instructs not to open a file, and in a 12 GB repository test, over 5 GiB was uploaded successfully.

telegram · zaihuapd · Jul 12, 04:19

**Background**: Grok Build is xAI's official command-line coding agent, powered by Grok 4.5, designed to assist with complex coding tasks. A git bundle is a single file containing all objects and references of a Git repository, commonly used for offline or network-transportable repository transfer. The tool's privacy setting to 'improve models' was found ineffective at preventing uploads.

<details><summary>References</summary>
<ul>
<li><a href="https://x.ai/cli">Grok Build | SpaceXAI</a></li>
<li><a href="https://git-scm.com/docs/git-bundle">Git - git-bundle Documentation</a></li>

</ul>
</details>

**Tags**: `#security`, `#privacy`, `#xAI`, `#CLI`, `#data leak`

---

<a id="item-10"></a>
## [Cursor Develops 'Sand' AI Agent to Rival Claude Cowork](https://www.theinformation.com/articles/cursor-developing-ai-agent-compete-claude-cowork) ⭐️ 8.0/10

Cursor is secretly developing a general-purpose AI agent codenamed 'Sand', capable of multi-step tasks like email replies and spreadsheet management, aiming to compete directly with Anthropic's Claude Cowork and OpenAI's ChatGPT Work. This move signals Cursor's ambition to expand beyond its code editor niche into the broader enterprise AI assistant market, intensifying competition among AI agents and potentially reshaping how businesses adopt AI for workflow automation. The 'Sand' agent is not yet publicly released, and its development underscores a trend toward multi-step, autonomous AI agents that can operate across various applications and file types.

telegram · zaihuapd · Jul 13, 01:34

**Background**: Cursor is an AI-powered code editor that uses AI agents to assist developers with coding tasks. Claude Cowork by Anthropic and ChatGPT Work by OpenAI are AI assistants that can interact with files, folders, and applications to perform real-world tasks. These tools represent a shift from simple chatbots to autonomous agents capable of executing complex workflows.

<details><summary>References</summary>
<ul>
<li><a href="https://cursor.com/">Cursor: AI coding agent</a></li>
<li><a href="https://claude.com/product/cowork">Claude Cowork | Claude by Anthropic</a></li>
<li><a href="https://chatgpt.com/work/">ChatGPT Work</a></li>

</ul>
</details>

**Tags**: `#AI agent`, `#Cursor`, `#enterprise AI`, `#competition`, `#general AI`

---