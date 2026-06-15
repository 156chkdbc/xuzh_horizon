---
layout: default
title: "Horizon Summary: 2026-06-15 (EN)"
date: 2026-06-15
lang: en
---

> From 32 items, 8 important content pieces were selected

---

1. [Pyodide 314.0 enables publishing WASM wheels to PyPI](#item-1) ⭐️ 9.0/10
2. [Rio de Janeiro's 'homegrown' LLM exposed as weighted merge of existing models](#item-2) ⭐️ 8.0/10
3. [Formal Methods Vital for AI-Generated Code Verification](#item-3) ⭐️ 8.0/10
4. [Prescient Satirical Talk on JavaScript's Fate](#item-4) ⭐️ 8.0/10
5. [Why AI Hasn’t Replaced Software Engineers, and Won’t](#item-5) ⭐️ 8.0/10
6. [75 US Data Center Projects Worth $130B Blocked in Q1 2026](#item-6) ⭐️ 8.0/10
7. [Huawei Open-Sources Pangu 2.0 with 505B Parameters](#item-7) ⭐️ 8.0/10
8. [US Government Restricts Anthropic's Mythos Models Over National Security](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Pyodide 314.0 enables publishing WASM wheels to PyPI](https://simonwillison.net/2026/Jun/13/publishing-wasm-wheels/#atom-everything) ⭐️ 9.0/10

Pyodide 314.0 now allows package maintainers to publish Python packages built for WebAssembly (WASM wheels) directly to PyPI, using the new PyEmscripten platform tag defined in PEP 783. This was previously restricted to Pyodide maintainers. This significantly reduces the maintenance burden on Pyodide core maintainers and empowers the wider Python community to contribute packages for Python in the browser. It is a long-awaited feature that could accelerate adoption of Python WASM runtimes. The new platform tag is `pyemscripten_2026_0_wasm32` (PEP 783). A demonstration package, luau-wasm, was published by Simon Willison, showing how to compile C++ extensions to WASM and distribute them via PyPI using GitHub Actions and cibuildwheel.

rss · Simon Willison · Jun 13, 23:55

**Background**: Pyodide is a Python distribution for WebAssembly that runs in the browser. Previously, Pyodide maintainers had to manually build and host over 300 packages, creating a bottleneck. PEP 783, finalized in 2025, defined the PyEmscripten platform tag to enable WASM wheels on PyPI.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jun/13/publishing-wasm-wheels/">Publishing WASM wheels to PyPI for use with Pyodide</a></li>
<li><a href="https://peps.python.org/pep-0783/">PEP 783 – Emscripten Packaging | peps.python.org</a></li>
<li><a href="https://pyodide.org/en/stable/console.html">pyodide .org/en/stable/console.html</a></li>

</ul>
</details>

**Tags**: `#Pyodide`, `#WASM`, `#PyPI`, `#Python packaging`, `#web assembly`

---

<a id="item-2"></a>
## [Rio de Janeiro's 'homegrown' LLM exposed as weighted merge of existing models](https://github.com/nex-agi/Nex-N2/issues/4) ⭐️ 8.0/10

An investigation revealed that Rio de Janeiro's LLM, Rio-3.5-Open-397B, is not a novel fine-tune but a weighted merge (60% Nex-N2 Pro + 40% Qwen3.5-397B-A17B) with minimal modifications, contradicting claims of being a homegrown model. This incident raises critical questions about transparency and attribution in open-source AI development, especially when public institutions claim credit for models that are essentially merges of existing work. The analysis showed that every weight tensor in the Rio model is a linear combination of the two source models to thousands of standard deviations, unlike typical fine-tunes which show more variation.

hackernews · unrvl22 · Jun 14, 15:37 · [Discussion](https://news.ycombinator.com/item?id=48528371)

**Background**: Model merging is a technique that combines parameters from multiple pre-trained LLMs into a single model without additional training, often using methods like weighted averaging or SLERP. It has become a common way to create new models cheaply, but raises ethical and attribution issues when presented as original work.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/blog/mlabonne/merge-models">Merge Large Language Models with mergekit</a></li>
<li><a href="https://developer.nvidia.com/blog/an-introduction-to-model-merging-for-llms/">An Introduction to Model Merging for LLMs | NVIDIA Technical Blog</a></li>

</ul>
</details>

**Discussion**: Community commenters expressed concern over the lack of transparency, with some speculating that the model may have been intended to include a distillation step that was not uploaded. Others noted the robustness of deep learning models to linear combinations of weights.

**Tags**: `#LLM`, `#open-source`, `#model merging`, `#ethics`, `#AI transparency`

---

<a id="item-3"></a>
## [Formal Methods Vital for AI-Generated Code Verification](https://blog.janestreet.com/formal-methods-at-jane-street-index/?from_theconsensus=1) ⭐️ 8.0/10

Jane Street's blog post discusses how formal methods, including proof automation and expressive type systems, will become more crucial as AI generates large codebases requiring robust verification. This shift emphasizes verification over code writing, potentially changing the role of programmers and improving software reliability in an era of AI-generated code. The post compares historical proof automation tools like the Boyer-Moore prover with modern approaches, while community comments highlight practical uses of expressive types in Scala 3 to prevent code quality issues.

hackernews · eatonphil · Jun 14, 12:35 · [Discussion](https://news.ycombinator.com/item?id=48526633)

**Background**: Formal methods are mathematically rigorous techniques for specifying, developing, and verifying software systems. They employ logic, formal languages, and type systems to ensure correctness. With AI generating massive codebases, manual verification becomes impractical, making formal methods increasingly important.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Formal_methods">Formal methods</a></li>
<li><a href="https://www.galois.com/what-are-formal-methods">What Are Formal Methods? | Galois</a></li>
<li><a href="https://en.wikipedia.org/wiki/Proof_automation">Proof automation</a></li>

</ul>
</details>

**Discussion**: Community comments show a range of perspectives: Animats recalls early proof automation successes; winwang uses expressive types in Scala 3 to prevent 'noun accretion' in AI-generated code; brap questions whether formal specs merely duplicate tests or implementations. Overall, discussion is engaged but varied.

**Tags**: `#formal methods`, `#programming`, `#software verification`, `#AI`, `#type systems`

---

<a id="item-4"></a>
## [Prescient Satirical Talk on JavaScript's Fate](https://www.destroyallsoftware.com/talks/the-birth-and-death-of-javascript) ⭐️ 8.0/10

A satirical talk from 2014 by Gary Bernhardt predicted that JavaScript would become the universal compilation target for web applications, leading to a catastrophic system collapse in the 2020s. It is now considered remarkably accurate given subsequent developments like WebAssembly and the expansion of JavaScript into various environments. This talk has become a cultural touchstone in the JavaScript community, sparking discussions about language evolution, compilation targets, and the risks of monoculture. Its predictions have partly materialized with JavaScript's dominance in browsers, servers (Node.js), and desktop apps (Electron), highlighting the enduring relevance of its critique. The talk was delivered in 2014, before WebAssembly was announced (2015) and before TypeScript gained widespread adoption. It specifically referenced asm.js as a compilation target, a precursor to WebAssembly. The title 'The Birth and Death of JavaScript' is a playful take on the lifecycle of programming languages.

hackernews · subset · Jun 14, 12:38 · [Discussion](https://news.ycombinator.com/item?id=48526661)

**Background**: A compilation target is the language or format that a compiler outputs. In web development, JavaScript is the native language of browsers. To run other languages on the web, they must be compiled to JavaScript. In 2014, asm.js was an early optimization to compile C/C++ to a subset of JavaScript for better performance, which later evolved into WebAssembly (Wasm)—a low-level binary format for near-native speed in browsers. The talk satirically exaggerates these trends to foresee a fragile ecosystem where everything is compiled to JavaScript.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Compiler">Compiler - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/WebAssembly">WebAssembly</a></li>

</ul>
</details>

**Discussion**: Commenters noted the talk's prescience, with one remarking that the predicted disaster between 2020-2025 was accurate in type but wrong in specific cause. Others observed that JavaScript indeed became a compilation target via WebAssembly, and technologies like TypeScript and Electron have expanded its reach. The overall sentiment is appreciation for the talk's humor and foresight.

**Tags**: `#javascript`, `#webassembly`, `#programming-humor`, `#predictions`, `#compilation-target`

---

<a id="item-5"></a>
## [Why AI Hasn’t Replaced Software Engineers, and Won’t](https://simonwillison.net/2026/Jun/14/why-ai-hasnt-replaced-software-engineers/#atom-everything) ⭐️ 8.0/10

Arvind Narayanan and Sayash Kapoor argue that data rejects the narrative of AI causing mass layoffs in software engineering, citing that not a single company in New York checked the AI disclosure box in WARN Act filings in the first year. They identify three real bottlenecks that resist automation: deciding what to build, verifying what is delivered, and deep human understanding of the codebase and business. This challenges the widespread belief that AI will soon automate software engineering jobs, suggesting that software engineers are more insulated than commonly assumed, and other professions are even more cushioned from AI disruption. The analysis provides evidence-based counter-narrative to AI hype around job displacement. The essay uses New York's WARN Act AI disclosure requirement, which had zero companies reporting AI-related layoffs in its first year (March 2025–March 2026). It also emphasizes that software engineering involves much more than typing code, such as meetings and debugging, which require deep contextual understanding.

rss · Simon Willison · Jun 14, 23:54

**Background**: The WARN Act (Worker Adjustment and Retraining Notification Act) is a U.S. law that requires employers with 100 or more employees to provide 60 days' advance notice of mass layoffs or plant closings. In March 2025, New York became the first state to add an AI disclosure checkbox to WARN filings, allowing companies to indicate if layoffs were due to AI. The fact that no company checked this box in the first year suggests that AI has not yet caused widespread job losses in software engineering.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WARN_Act">WARN Act</a></li>

</ul>
</details>

**Tags**: `#AI`, `#software engineering`, `#job displacement`, `#labor market`, `#data analysis`

---

<a id="item-6"></a>
## [75 US Data Center Projects Worth $130B Blocked in Q1 2026](https://www.tomshardware.com/tech-industry/artificial-intelligence/more-than-75-data-center-build-outs-worth-usd130-billion-have-been-successfully-blocked-in-the-first-four-months-of-2026-bipartisan-opposition-mounts-nationwide-over-fears-of-soaring-power-and-water-costs) ⭐️ 8.0/10

In the first quarter of 2026, over 75 data center construction projects across the United States, valued at approximately $130 billion, were successfully blocked or delayed due to mounting bipartisan and community opposition over their energy and water consumption. This wave of opposition threatens to slow the expansion of AI and cloud computing infrastructure, potentially increasing costs and delays for tech companies and impacting the nation's digital economy. The number of active grassroots opposition groups surged from 396 to 833 across 49 states, and both state legislatures and some federal lawmakers have introduced bills to pause or regulate new data center construction.

telegram · zaihuapd · Jun 14, 03:03

**Background**: Data centers are large facilities housing thousands of servers that consume massive amounts of electricity and water for cooling, especially as AI workloads rise. This has sparked concerns about grid strain, rising utility costs, and environmental impact, leading to bipartisan coalitions of local officials and residents opposing new projects.

**Tags**: `#data centers`, `#energy`, `#infrastructure`, `#regulation`, `#AI`

---

<a id="item-7"></a>
## [Huawei Open-Sources Pangu 2.0 with 505B Parameters](https://t.me/zaihuapd/41948) ⭐️ 8.0/10

At Huawei Developer Conference 2026, Huawei announced the open-source Pangu 2.0 model (openPangu 2.0), including a 505B-parameter Pro version and a 92B-parameter Flash version, both supporting a 512K token context window. The company plans to open-source seven major components starting June 30, including pre-training code. This release marks a significant move by Huawei to democratize large language model technology, potentially challenging dominant players like OpenAI and Google. With its native optimization for Ascend AI chips and HarmonyOS, the open-source Pangu 2.0 could accelerate AI adoption in China and beyond. The 505B Pro variant offers state-of-the-art parameter count, while the 92B Flash variant provides a more efficient option. Both models are designed to be friendly to Ascend computing power and are adapted for HarmonyOS, with open-sourcing of components beginning June 30.

telegram · zaihuapd · Jun 14, 08:05

**Background**: Huawei's Ascend AI chips are neural processing units (NPUs) designed for high-performance AI computing, used in data centers and edge devices. The 512K context window allows the model to process large amounts of text in a single pass, enabling applications like long-document analysis and multi-turn conversations. Pangu is Huawei's foundational large model series, first released in 2021.

<details><summary>References</summary>
<ul>
<li><a href="https://e.huawei.com/cn/products/computing/ascend">昇腾计算-华为Ascend-AI计算-华为企业业务</a></li>
<li><a href="https://devtk.ai/zh/blog/llm-context-window-explained/">LLM 上下文窗口详解：从 4K 到 1M Token（2026） - DevTk.AI</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/1913660152676094004">一文看懂华为昇腾芯片 - 知乎 - 知乎专栏</a></li>

</ul>
</details>

**Tags**: `#open-source`, `#large language model`, `#Huawei`, `#AI`, `#Pangu`

---

<a id="item-8"></a>
## [US Government Restricts Anthropic's Mythos Models Over National Security](https://t.me/zaihuapd/41949) ⭐️ 8.0/10

The U.S. government issued an export control letter to Anthropic, ordering the suspension of access to its Fable 5 and Mythos 5 models for foreign nationals, both inside and outside the U.S. Anthropic has complied by closing access to these models for all customers. This marks a significant escalation in U.S. export controls on advanced AI models, directly impacting model availability and setting a precedent for future AI regulation. It highlights growing national security concerns over AI capabilities and potential misuse through jailbreaking. The Commerce Department's action is reportedly linked to concerns that the models could be jailbroken to pose security risks. Anthropic clarified that other Claude models are unaffected, and the company is working to restore access as soon as possible.

telegram · zaihuapd · Jun 14, 09:06

**Background**: AI jailbreaking refers to techniques that bypass the ethical guardrails of AI systems, allowing them to perform restricted actions. The U.S. Bureau of Industry and Security (BIS) has increasingly applied export controls to advanced AI model weights, as seen in January 2025 rules. Claude Mythos is a model developed by Anthropic for tasks like cybersecurity vulnerability discovery, and it has not been publicly released.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Mythos">Claude Mythos - Wikipedia</a></li>
<li><a href="https://www.anthropic.com/claude/mythos">Claude Mythos - Anthropic</a></li>
<li><a href="https://www.sidley.com/en/insights/newsupdates/2025/01/new-us-export-controls-on-advanced-computing-items-and-artificial-intelligence-model-weights">New U.S. Export Controls on Advanced Computing Items and ...</a></li>

</ul>
</details>

**Tags**: `#AI regulation`, `#export controls`, `#Anthropic`, `#national security`, `#model access`

---