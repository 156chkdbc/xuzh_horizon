---
layout: default
title: "Horizon Summary: 2026-08-03 (EN)"
date: 2026-08-03
lang: en
---

> From 35 items, 7 important content pieces were selected

---

1. [OpenAI Astra Scores Breakthroughs on Ten Math Problems](#item-1) ⭐️ 9.0/10
2. [Karpathy's Pelican Tweet Sparks LLM Vector Graphics Benchmark Debate](#item-2) ⭐️ 8.0/10
3. [Kakehashi: Userspace Layer Runs macOS CLI Binaries on Linux ARM](#item-3) ⭐️ 8.0/10
4. [F*: A General-Purpose Proof-Oriented Programming Language](#item-4) ⭐️ 8.0/10
5. [eBay executives jailed, $56M payout for harassment campaign](#item-5) ⭐️ 8.0/10
6. [Microsoft-Backed Open Letter Supports Open-Weight AI Models](#item-6) ⭐️ 8.0/10
7. [Microsoft Confirms Copilot 'Super App' Launch This Year](#item-7) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI Astra Scores Breakthroughs on Ten Math Problems](https://openai.com/index/ten-advances-in-mathematics/) ⭐️ 9.0/10

OpenAI announced that an internal version of its next-generation Astra model produced new results on ten long-standing open problems in mathematics and theoretical computer science, at a reported cost of under $2,000 per problem at GPT-5.6 Sol token prices. The AI-generated arguments were organized into papers by human collaborators, formalized in the Lean proof assistant, and published in the openai/ten-proofs repository. These results mark one of the strongest demonstrations yet that AI can make original headway on problems that have resisted mathematicians for decades or longer. If verified, they could accelerate the shift toward 'big mathematics' — large-scale human-machine collaboration in research — though the mathematical community has not yet validated the proofs. The ten problems span high-dimensional sphere packing, the existence of non-sofic groups, a counterexample to Connes' rigidity conjecture, arithmetic circuit lower bounds, quantum parallel repetition, hardness of the nearest vector problem, and multicolor Ramsey numbers. OpenAI was transparent that the mathematical arguments are AI-generated and that humans handled organization and formalization, and it released Lean 4 formalizations, a paper, and an LLM-generated reasoning walkthrough.

telegram · zaihuapd · Aug 1, 07:59

**Background**: Lean is an open-source proof assistant and functional programming language based on the calculus of inductive constructions; it lets mathematicians specify theorems and verify proofs mechanically. The problems targeted by Astra are famous open questions — for example, Connes' rigidity conjecture asks whether certain group von Neumann algebras uniquely determine their underlying group, and sofic groups are a class of groups approximable by finite symmetric groups. The use of a proof assistant is significant because it provides a machine-checkable guarantee, but the underlying mathematical arguments still need human scrutiny.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Lean_theorem_prover">Lean theorem prover</a></li>
<li><a href="https://math.ucsd.edu/seminar/connes-rigidity-conjecture">On Connes' rigidity conjecture | Department of Mathematics</a></li>
<li><a href="https://en.wikipedia.org/wiki/Sofic_group">Sofic group</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters and observers expressed a mix of excitement and caution, comparing the moment to Deep Blue's chess victory and quoting Terence Tao's vision of 'big mathematics.' Some mathematicians reacted with what one essay called a 'profound spiritual crisis,' while others noted the lack of information about problems where the model failed and asked OpenAI to release the actual prompts used.

**Tags**: `#OpenAI`, `#AI research`, `#mathematics`, `#theorem proving`, `#machine learning`

---

<a id="item-2"></a>
## [Karpathy's Pelican Tweet Sparks LLM Vector Graphics Benchmark Debate](https://twitter.com/karpathy/status/2083749667410727319) ⭐️ 8.0/10

Andrej Karpathy tweeted about LLMs drawing a pelican, using the example to highlight vector graphics as a new benchmark for testing physical world understanding. The tweet quickly gained traction on Hacker News, where commenters debated the merits and reproducibility of such qualitative benchmarks. This matters because it points to a shift from using generated images purely for visual appeal toward using vector graphics to expose whether models genuinely understand physical concepts. It could influence how the AI community designs future benchmarks for evaluating LLM reasoning beyond text. The tweet itself appears to be a link to an xcancel mirror, and the original prompt Karpathy used was not included in the post, prompting reproducibility concerns. Commenters compared it to Simon Willison's pelican SVG benchmark and noted earlier examples like Microsoft's GPT-4 evaluation asking for a TikZ unicorn.

hackernews · delichon · Aug 2, 04:05 · [Discussion](https://news.ycombinator.com/item?id=49140998)

**Background**: Vector graphics describe images using geometric primitives like paths and shapes, and SVG is a widely used text-based format, making it easy for LLMs to generate as code. Drawing a recognizable pelican in SVG requires not only syntax knowledge but a mental model of the bird's shape and proportions, which tests physical reasoning. Earlier work such as Chat2SVG and LLM4SVG has explored LLM-based vector graphic generation, and Simon Willison's pelican SVG benchmark from November 2025 popularized the idea of using such prompts as a qualitative test.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2025/Nov/25/llm-svg-generation-benchmark/">LLM SVG Generation Benchmark</a></li>
<li><a href="https://chat2svg.github.io/">Chat2SVG: Vector Graphics Generation with Large Language Models and Image Diffusion Models</a></li>

</ul>
</details>

**Discussion**: Commenters were divided: some agreed with jmugan that poor outputs are the point and such benchmarks expose physical understanding, while didibus questioned whether any LLM had actually drawn a correct pelican. consumer451 noted the missing prompt makes Karpathy's demo non-reproducible, and iDon pointed to Microsoft's earlier GPT-4 TikZ unicorn evaluation as a precedent.

**Tags**: `#AI`, `#LLM`, `#benchmarks`, `#vector graphics`, `#Karpathy`

---

<a id="item-3"></a>
## [Kakehashi: Userspace Layer Runs macOS CLI Binaries on Linux ARM](https://github.com/wie-project/kakehashi) ⭐️ 8.0/10

Kakehashi is an experimental userspace translation layer that runs macOS ARM64 CLI binaries natively on Linux aarch64. Working prototypes include 7-Zip, curl, and Xcode's Git, verified on Docker/Colima and UTM. This addresses a long-standing compatibility gap by bringing macOS binaries to Linux ARM without a full OS emulation layer like Darling. It could open up macOS CLI tooling and workflows to Linux ARM users (e.g. Apple Silicon-era binaries) much like Wine/Proton did for Windows apps. The project is CLI-first and has no JIT; it loads Darwin Mach-O binaries on Linux aarch64, maps a freestanding libSystem, and translates BSD syscalls. Current 7-Zip performance is about 5.2x slower than native Linux, with a planned optimization roadmap to reduce the gap.

hackernews · vlad_kalinkin · Aug 2, 16:26 · [Discussion](https://news.ycombinator.com/item?id=49145937)

**Background**: Mach-O is the executable format used by macOS and iOS, while Linux uses ELF, so binaries are not directly interchangeable. A compatibility layer translates foreign system calls and provides library shims so foreign binaries can run on the host OS. Kakehashi follows a similar philosophy to Darling and Wine, but focuses specifically on macOS CLI binaries on Linux ARM64 and is implemented as a userspace tool installed via Cargo.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/wie-project/kakehashi">GitHub - wie-project/kakehashi: Userspace macOS translation layer for Linux ARM64 · GitHub</a></li>
<li><a href="https://news.ycombinator.com/item?id=49145937">Show HN: Kakehashi – Experimental userspace to run macOS binaries on Linux ARM | Hacker News</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mach-O">Mach-O - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters showed strong interest and compared Kakehashi to Darling, asking whether efforts could be merged given Darling's open ARM64 PR. Some questioned the naming and noted the project is still early-stage, while one user asked about a ROM-style approach that executes the original binary without redistributing rewritten libraries.

**Tags**: `#macOS`, `#Linux`, `#ARM`, `#compatibility`, `#userspace`

---

<a id="item-4"></a>
## [F*: A General-Purpose Proof-Oriented Programming Language](https://fstar-lang.org/) ⭐️ 8.0/10

A Hacker News post about F*, a general-purpose proof-oriented programming language for formal verification, generated strong community interest with 159 points and 69 comments. The discussion emphasized F*'s maturity and practical use in migrating existing C codebases to verified code. F* is a significant and mature proof-oriented language widely used in formal verification and security research, such as Project Everest. The strong Hacker News engagement signals growing interest in practical formal verification tools that can improve software security and correctness. F* combines dependent types with SMT solving and tactic-based interactive theorem proving, and by default compiles to OCaml. It can also extract code to C or WebAssembly via KaRaMeL and to assembly via Vale, but by default F* only verifies input code rather than executing it.

hackernews · ducktective · Aug 2, 12:31 · [Discussion](https://news.ycombinator.com/item?id=49143925)

**Background**: Formal verification involves proving that a program satisfies a formal specification of its behavior, providing strong correctness guarantees. F* is a high-level, multi-paradigm functional programming language inspired by ML and OCaml, designed for program verification and secure software development. Its expressive, dependently typed core logic enables proof-oriented programming across different paradigms.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/F*_(programming_language)">F* (programming language) - Wikipedia</a></li>
<li><a href="https://fstar-lang.org/">F*: A Proof-Oriented Programming Language</a></li>
<li><a href="https://github.com/FStarLang/FStar">GitHub - FStarLang/FStar: A Proof-oriented Programming ... Proof-oriented Programming in F* - fstar-lang.org F* (programming language) - Wikipedia F*: A general-purpose proof-oriented programming language ... FStar/README.md at master · FStarLang/FStar · GitHub Proof-Oriented Programming in F* - mtzguido.github.io</a></li>

</ul>
</details>

**Discussion**: Commenters had mixed reactions: one criticized the F* homepage for lacking code examples, asking to see syntax and use cases upfront. Others praised F* for expressing external libraries while incrementally migrating C codebases, and a beginner asked whether F* is used in industry and for what software. A joke about responsive stylesheets and side effects also appeared.

**Tags**: `#formal verification`, `#programming languages`, `#proof assistants`, `#security`, `#functional programming`

---

<a id="item-5"></a>
## [eBay executives jailed, $56M payout for harassment campaign](https://www.ft.com/content/06ec1b03-d4af-40cf-b12a-4ba5a410f6d2) ⭐️ 8.0/10

eBay executives orchestrated a campaign of harassment and intimidation against the Steiners, a couple who had criticized the company. The scheme led to a $56 million payout and prison sentences for several eBay security team members, including a 57-month sentence for former Senior Director Jim Baugh. This case highlights the dangers of corporate security teams overstepping their authority to retaliate against critics. It sends a strong signal to technology companies that such behavior will have serious legal and financial consequences, and reinforces the need for accountability and oversight in corporate security operations. Seven members of eBay's security team, including former police captains, were involved in the harassment campaign, according to prosecutors. Sentences varied: Brian Gilbert, a former Senior Manager, received time served, one year of supervised release, and a $20,000 fine; Jim Baugh received 57 months in prison.

hackernews · JumpCrisscross · Aug 2, 19:19 · [Discussion](https://news.ycombinator.com/item?id=49147435)

**Background**: eBay is a global online marketplace. This case involves eBay's Global Security Team, a unit tasked with protecting the company, which prosecutors say instead worked together to harass and intimidate the Steiners, a couple who had been critical of eBay. The actions included threats and surveillance, and the case resulted in criminal sentences and a $56 million payout to the victims.

**Discussion**: Commenters questioned whether the harassment was limited to one couple, suggesting other critics may have been targeted. They also expressed concern about the involvement of former police captains and hoped their careers would be investigated. Some shifted to criticizing eBay's business practices, including high fees, while one commenter cited a general principle about human behavior when supervision is lacking.

**Tags**: `#security`, `#corporate ethics`, `#legal`, `#eBay`, `#accountability`

---

<a id="item-6"></a>
## [Microsoft-Backed Open Letter Supports Open-Weight AI Models](https://simonwillison.net/2026/Aug/2/open-letters/#atom-everything) ⭐️ 8.0/10

Simon Willison highlighted a flurry of recent open letters on AI development, led by Microsoft's 'Open Weights and American AI Leadership' letter signed by 235 companies including NVIDIA, Amazon, and OpenAI. Anthropic published a contrasting response, and a separate letter called 'Pacing the Frontier' gathered 1,324 frontier AI employees. This signals major industry alignment in favor of open-weight AI models, directly countering potential US government restrictions on safety grounds. The split between Anthropic and Microsoft-backed signatories highlights a deepening policy divide over AI openness and risk. The Microsoft letter explicitly defends distillation as a legitimate model-development technique, while Anthropic's response calls for cracking down on industrial-scale distillation operations. The 'Pacing the Frontier' letter, signed by figures like OpenAI's Jakub Pachocki and Anthropic's Dario Amodei, urges international governance to pace automated AI development.

rss · Simon Willison · Aug 2, 04:16

**Background**: Open-weight AI models publish their trained parameters (weights), allowing anyone to inspect, fine-tune, and deploy them, unlike closed models offered only through APIs. Proponents argue this transparency fosters innovation and distributed scrutiny; critics warn the same access could empower malicious actors or authoritarian governments.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/open-weight-ai-models-why-every-enterprise-should-paying-misra-gi2qc">Open - Weight AI Models : Why Every Enterprise Should Be Paying...</a></li>
<li><a href="https://infercom.ai/blog/open-weight-models-explained/">Open - Weight AI Models : Why They're a Strategic Advantage | Infercom</a></li>

</ul>
</details>

**Tags**: `#AI`, `#open source`, `#policy`, `#AI safety`, `#Microsoft`

---

<a id="item-7"></a>
## [Microsoft Confirms Copilot 'Super App' Launch This Year](https://www.theverge.com/tech/972927/microsoft-copilot-super-app-confirmed) ⭐️ 8.0/10

Microsoft CEO Satya Nadella confirmed on Wednesday's earnings call that the company will launch an AI 'super app' this year, combining Copilot's chat, coding, and agentic capabilities for both consumers and businesses. The app will merge experiences including code features into a single platform this quarter. This move unifies Microsoft's fragmented AI tools into one workspace, directly competing with OpenAI's ChatGPT Work and signaling an industry shift toward all-in-one AI platforms. It could reshape developer workflows and how businesses deploy AI agents at scale. The super app will integrate Copilot chat, GitHub Copilot, Copilot Cowork, and Autopilot systems, according to a Fortune report cited by Nadella. Microsoft's last quarter revenue reached $90 billion, driven largely by AI and cloud growth.

telegram · zaihuapd · Aug 1, 13:18

**Background**: Microsoft's Copilot is evolving from a pure chat assistant into 'Cowork' and 'Autopilots'—agentic systems that can plan, execute, and deliver work with user approval. Agentic AI refers to intelligent agents that pursue goals and use tools with varying autonomy. Competitor OpenAI recently launched ChatGPT Work, which integrates ChatGPT and Codex into a team-oriented workspace, highlighting the broader trend of consolidating AI capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Agentic_AI">Agentic AI</a></li>
<li><a href="https://www.microsoft.com/en-us/microsoft-365/blog/2026/03/09/copilot-cowork-a-new-way-of-getting-work-done/">Copilot Cowork: A new way of getting work done | Microsoft ...</a></li>
<li><a href="https://openai.com/chatgpt-work/">ChatGPT Work for every team | OpenAI</a></li>

</ul>
</details>

**Tags**: `#Microsoft`, `#Copilot`, `#AI`, `#Super App`, `#Developer Tools`

---