---
layout: default
title: "Horizon Summary: 2026-05-31 (EN)"
date: 2026-05-31
lang: en
---

> From 35 items, 14 important content pieces were selected

---

1. [vLLM v0.22.0: DeepSeek V4 Maturity, MRv2, Rust Frontend](#item-1) ⭐️ 9.0/10
2. [Huawei Proposes Tau Law: Time Scaling to Replace Geometric Scaling](#item-2) ⭐️ 9.0/10
3. [Microsoft degrades perpetual Office licenses to view-only mode](#item-3) ⭐️ 8.0/10
4. [Domain Expertise Remains the True Competitive Advantage](#item-4) ⭐️ 8.0/10
5. [Accenture Acquires Ookla for $1.2B to Boost Network Intelligence](#item-5) ⭐️ 8.0/10
6. [Voxel Space (2017) - Deep Dive into Comanche's Terrain Rendering Algorithm](#item-6) ⭐️ 8.0/10
7. [Zig ELF Linker Improvements Promise Faster Iteration](#item-7) ⭐️ 8.0/10
8. [Openrsync: OpenBSD's Secure Rsync Implementation Gains Traction](#item-8) ⭐️ 8.0/10
9. [OpenRouter raises $113M Series B](#item-9) ⭐️ 8.0/10
10. [Pope Leo's first encyclical attacks technological messianism](#item-10) ⭐️ 8.0/10
11. [Anthropic Details Claude Sandboxing Across Products](#item-11) ⭐️ 8.0/10
12. [Running Python ASGI Apps in Browser with Pyodide and Service Workers](#item-12) ⭐️ 8.0/10
13. [SpaceX wins $4.16B US military satellite missile tracking contract](#item-13) ⭐️ 8.0/10
14. [New FROST attack exploits SSD timing to spy on browser activity](#item-14) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [vLLM v0.22.0: DeepSeek V4 Maturity, MRv2, Rust Frontend](https://github.com/vllm-project/vllm/releases/tag/v0.22.0) ⭐️ 9.0/10

vLLM v0.22.0 was released with 459 commits from 230 contributors, introducing DeepSeek V4 maturity with NVFP4 fused MoE and MTP speculative decoding, Model Runner V2 advances, and an experimental Rust frontend. This release significantly enhances LLM inference performance and model support, particularly for DeepSeek V4, and experiments with Rust for potential performance gains, impacting the open-source LLM serving ecosystem. Batch-invariant inference with Cutlass FP8 achieves 28.9% end-to-end latency improvement, and a new multi-tier KV cache offloading framework extends beyond CPU memory to disk. The Rust frontend is experimental and includes a data-parallel supervisor.

github · khluu · May 29, 10:28

**Background**: vLLM is an open-source library for fast LLM inference and serving, widely used in production. DeepSeek V4 is a large Mixture-of-Experts model requiring efficient kernels like NVFP4 fused MoE and MegaMoE. Model Runner V2 is a redesigned inference engine aiming for better performance and flexibility. The Rust frontend explores using Rust for low-level serving components.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/api/vllm/model_executor/layers/fused_moe/experts/trtllm_nvfp4_moe/">trtllm_ nvfp 4 _ moe - vLLM</a></li>
<li><a href="https://vllm-website-nj3unaiki-inferact-inc.vercel.app/blog/deepseek-v4">DeepSeek V4 in vLLM : Efficient Long-context Attention | vLLM Blog</a></li>
<li><a href="https://docs.vllm.ai/en/stable/api/vllm/models/deepseek_v4/nvidia/ops/prepare_megamoe/">prepare_ megamoe - vLLM</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#LLM inference`, `#DeepSeek`, `#open-source`, `#AI systems`

---

<a id="item-2"></a>
## [Huawei Proposes Tau Law: Time Scaling to Replace Geometric Scaling](https://t.me/zaihuapd/41648) ⭐️ 9.0/10

Huawei presented the Tau (τ) Scaling Law at the 2026 IEEE International Symposium on Circuits and Systems (ISCAS), proposing time scaling as a new principle to replace traditional geometric scaling in semiconductor advancement. The company claims to have designed and mass-produced 381 chips over the past six years using this approach and plans to launch a new Kirin mobile chip with logic folding technology in autumn 2026. The Tau Scaling Law could shift the semiconductor industry away from Moore's Law by prioritizing reduction of signal propagation time (τ) over transistor size, potentially enabling continued performance gains despite physical limits. If validated, this approach may help Huawei and the broader Chinese chip industry advance amid geopolitical export restrictions. The law focuses on minimizing the time constant (τ) across device, circuit, and system levels through multi-layer collaborative optimization. Huawei aims to achieve transistor density equivalent to 1.4nm process nodes by 2031 using its logic folding technology, which splits critical gate circuits into vertically stacked active layers with ultra-fine pitch hybrid bonding.

telegram · zaihuapd · May 30, 02:18

**Background**: Moore's Law, which drove semiconductor advancement for decades, predicted that transistor density would double approximately every two years through geometric scaling—shrinking transistor dimensions. However, as physical limits approach, traditional scaling has become increasingly difficult and expensive. The Tau Scaling Law proposes an alternative: instead of shrinking transistors, reduce the signal propagation time (τ) by optimizing resistance and capacitance across all system levels, potentially leveraging 3D stacking techniques like logic folding.

<details><summary>References</summary>
<ul>
<li><a href="https://www.huawei.com/en/news/2026/5/ieee-iscas-tau-scaling">HUAWEI Presents the Tau (τ) Scaling Law, Enabling Breakthroughs in Transistor Density and System Performance - Huawei</a></li>
<li><a href="https://www.yicaiglobal.com/news/huawei-presents-tau-law-to-replace-geometric-scaling-with-time-scaling-in-semiconductor-industry">Huawei Proposes Tau Scaling Law to Replace Moore’s Law in Chip Industry</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-05-27/what-to-know-about-huawei-s-new-ai-chipmaking-plan-logicfolding-tech">What to Know About Huawei’s New AI Chipmaking Plan... - Bloomberg</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#Huawei`, `#Moore's Law`, `#chip design`, `#time scaling`

---

<a id="item-3"></a>
## [Microsoft degrades perpetual Office licenses to view-only mode](https://consumerrights.wiki/w/Microsoft_Office_2019_and_2021_for_Mac_view-only_conversion_(2026)) ⭐️ 8.0/10

Microsoft plans to convert perpetually-licensed Office 2019 and 2021 for Mac to view-only mode after a certain date, effectively removing editing capabilities from products users paid for indefinitely. This move undermines the concept of software ownership, as perpetual licenses are supposed to grant indefinite use of the purchased version. It also pushes users toward Microsoft 365 subscriptions, drawing backlash from consumers concerned about diminishing rights. The change applies specifically to Office 2019 and 2021 for Mac perpetual licenses, with the view-only conversion reportedly scheduled for 2026. Users will still be able to open and view documents, but cannot edit, create, or save changes.

hackernews · antipurist · May 30, 23:26 · [Discussion](https://news.ycombinator.com/item?id=48341578)

**Background**: A perpetual license for Microsoft Office allows users to pay a one-time fee and use that specific version indefinitely, though support and security updates may end after a few years. This is distinct from the subscription-based Microsoft 365, which requires ongoing payment for access. Microsoft has been increasingly pushing subscription models across its products, and this deprecation of offline perpetual licenses is seen as another step in that direction.

<details><summary>References</summary>
<ul>
<li><a href="https://www.compugen.us/blog/microsofts-perpetual-vs.-subscription-licensing-program-explained">Microsoft’s Perpetual vs. Subscription Licensing Program Explained</a></li>
<li><a href="https://www.quora.com/What-is-the-difference-between-an-Office-365-subscription-and-a-perpetual-license-for-Microsoft-Office-products-Are-they-both-subscription-based-but-with-different-terms">What is the difference between an Office 365 subscription and a perpetual license for Microsoft Office products? Are they both subscription-based, but with different terms? - Quora</a></li>

</ul>
</details>

**Discussion**: Community comments express strong anger and calls for boycott, with users like jmward01 urging people to stop buying Microsoft software and 'get mad.' Others note legal implications, such as Australian consumer law, and predict Microsoft will proceed regardless. Some suggest switching to LibreOffice as an alternative.

**Tags**: `#Microsoft`, `#software licensing`, `#consumer rights`, `#Office`, `#perpetual license`

---

<a id="item-4"></a>
## [Domain Expertise Remains the True Competitive Advantage](https://www.brethorsting.com/blog/2026/05/domain-expertise-has-always-been-the-real-moat/) ⭐️ 8.0/10

A recent blog post argues that domain expertise, not AI tools or generalist coding skills, is the enduring competitive advantage for developers and businesses. This perspective challenges the hype around AI replacing developers and highlights the enduring value of deep industry knowledge in a rapidly evolving tech landscape. The post cites examples such as a domain expert's app failing due to poor database design and a charter fishing trip that reveals a gap between domain knowledge and software engineering.

hackernews · aaronbrethorst · May 30, 20:40 · [Discussion](https://news.ycombinator.com/item?id=48340411)

**Background**: "Domain expertise" refers to deep knowledge of a specific industry or field, such as finance or fishing. "Vibe coding" is a term for building software using AI assistants without fully understanding the code. The debate centers on whether AI tools make generalist developers obsolete or whether domain expertise remains critical.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vibe_coding">Vibe coding - Wikipedia</a></li>
<li><a href="https://agentsroom.dev/what-is-vibe-coding">What is Vibe Coding ? Definition , Origin, and How It... | AgentsRoom</a></li>

</ul>
</details>

**Discussion**: Comments largely agree that domain expertise remains crucial. Users share examples of projects failing due to lack of domain knowledge, while some note that software engineering itself is a domain of expertise.

**Tags**: `#domain-expertise`, `#AI`, `#software-engineering`, `#moat`, `#vibe-coding`

---

<a id="item-5"></a>
## [Accenture Acquires Ookla for $1.2B to Boost Network Intelligence](https://newsroom.accenture.com/news/2026/accenture-to-acquire-ookla-to-strengthen-network-intelligence-and-experience-with-data-and-ai-for-enterprises) ⭐️ 8.0/10

Accenture announced it will acquire Ookla, the company behind Speedtest, Downdetector, and other network testing tools, for $1.2 billion. This acquisition allows Accenture to leverage Ookla's vast network performance data and AI capabilities to help telecom operators and enterprises optimize their networks, potentially reshaping the network intelligence services market. Ookla's data platform processes over 250 million consumer-initiated tests per month, supplemented by controlled drive and walk testing, providing granular insights into network performance.

hackernews · Garbage · May 30, 16:28 · [Discussion](https://news.ycombinator.com/item?id=48337987)

**Background**: Ookla is best known for Speedtest.net, a widely used internet speed testing website, and Downdetector, which tracks service outages. The company also offers enterprise-grade network testing and analytics solutions. Accenture is a global professional services firm that has been expanding its network intelligence and AI offerings.

**Discussion**: Community comments highlight that the acquisition is primarily about data monetization, as Ookla sells network performance data to telecom operators for six-figure annual fees. Some users expressed surprise at the high valuation given the apparent simplicity of the products, while former employees noted the company's significant revenue from data programs and awards.

**Tags**: `#acquisition`, `#network intelligence`, `#data monetization`, `#telecom`, `#Accenture`

---

<a id="item-6"></a>
## [Voxel Space (2017) - Deep Dive into Comanche's Terrain Rendering Algorithm](https://s-macke.github.io/VoxelSpace/) ⭐️ 8.0/10

The article provides a detailed technical breakdown of the Voxel Space terrain rendering algorithm used in the 1992 game Comanche: Maximum Overkill, including code samples and historical context. It also features community anecdotes about using the algorithm in modern projects. This algorithm was revolutionary for its time, enabling smooth 3D terrain rendering on hardware as modest as a 386SX. Understanding it provides valuable insights for game developers, retro computing enthusiasts, and anyone interested in efficient real-time graphics techniques. Technically, the algorithm renders a heightmap by drawing vertical lines from a color map, not using true volumetric voxels; it is more akin to a prism-based height map. The entire rendering engine can be implemented in surprisingly few lines of code.

hackernews · davikr · May 30, 14:25 · [Discussion](https://news.ycombinator.com/item?id=48336564)

**Background**: Voxel Space is a terrain rendering technique popularized by NovaLogic's Comanche series in the early 1990s. It uses a heightfield and a color texture to generate a 3D view by casting rays horizontally and sampling the height field to determine screen columns. Unlike true voxel engines that represent volume uniformly, Voxel Space treats the terrain as a 2.5D surface, allowing very fast rendering on CPUs of the era.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/s-macke/voxelspace">s-macke/VoxelSpace: Terrain rendering algorithm in less than 20 lines of code - GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Voxel">Voxel - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community comments express nostalgia and technical appreciation, with one user applying the concept of minimal testing ('oil tank holiday') to code. Another commenter clarifies that the algorithm is not true voxel rendering but a height map technique. Some share ports to modern engines like AGS and C++.

**Tags**: `#voxel`, `#terrain rendering`, `#game development`, `#history`, `#algorithm`

---

<a id="item-7"></a>
## [Zig ELF Linker Improvements Promise Faster Iteration](https://ziglang.org/devlog/2026/#2026-05-30) ⭐️ 8.0/10

The Zig team has released significant improvements to its ELF linker, which enable fast incremental linking and drastically reduce compile times during development. This was announced in the Zig devlog for 2026-05-30. These improvements promise to make Zig a viable C replacement by offering iteration speeds comparable to interpreted languages while maintaining C or Rust-like performance. This could revolutionize systems programming workflows, enabling faster development cycles. The new linker supports incremental compilation for ELF targets, but incremental linking is generally mutually exclusive with link-time optimization (LTO). Thus, this feature is intended for development builds rather than release builds.

hackernews · kristoff_it · May 30, 17:29 · [Discussion](https://news.ycombinator.com/item?id=48338673)

**Background**: ELF (Executable and Linkable Format) is a standard file format for executables, object code, and shared libraries on Unix-like systems. Incremental compilation is a technique that recompiles only the changed parts of a program, speeding up the edit-compile-test loop. Zig is a systems programming language designed to be modern, safe, and practical, often positioned as a potential replacement for C.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Executable_and_Linkable_Format">Executable and Linkable Format - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Incremental_compilation">Incremental compilation</a></li>

</ul>
</details>

**Discussion**: The community was highly enthusiastic, with users like bpavuk predicting Zig will become the definitive C replacement, enabling iteration speeds comparable to Python or JavaScript. Derefr raised a technical concern that incremental linking may preclude link-time optimization, limiting its use to development builds. Overall, the sentiment was very positive, with many expressing excitement about the progress.

**Tags**: `#Zig`, `#ELF Linker`, `#compiler`, `#systems programming`, `#incremental compilation`

---

<a id="item-8"></a>
## [Openrsync: OpenBSD's Secure Rsync Implementation Gains Traction](https://github.com/kristapsdz/openrsync) ⭐️ 8.0/10

OpenBSD's openrsync, a BSD-licensed reimplementation of rsync with pledge and unveil security features, is gaining widespread attention and discussion in the open-source community. This project improves file synchronization security by restricting program capabilities and filesystem access, addressing vulnerabilities in the widely-used rsync tool, and offers a portable alternative for Unix-like systems. Openrsync is available on GitHub and compiles on various UNIX systems, though officially supported on OpenBSD. It currently lacks full rsync compatibility in some edge cases, such as the --rsync-path option behavior.

hackernews · sph · May 30, 10:51 · [Discussion](https://news.ycombinator.com/item?id=48334854)

**Background**: Rsync is a standard Unix tool for efficiently synchronizing files locally or over a network. OpenBSD is known for its proactive security approach, introducing system calls like pledge(2) to restrict process capabilities and unveil(2) to limit filesystem visibility. Openrsync integrates these mechanisms to minimize attack surface.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Openrsync">OpenBSD - Wikipedia</a></li>
<li><a href="https://man.openbsd.org/openrsync.1">openrsync(1) - OpenBSD manual pages</a></li>
<li><a href="https://github.com/kristapsdz/openrsync">GitHub - kristapsdz/openrsync: BSD-licensed implementation of rsync · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenBSD_security_features">OpenBSD security features - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community feedback is generally positive, with users reporting improved stability over time. Some issues remain, such as differing behavior with --rsync-path, and there is discussion about pledge support on Linux. Additionally, users note that openrsync is being developed as part of an RPKI validator, and a Go implementation by the Gokrazy team also exists.

**Tags**: `#rsync`, `#OpenBSD`, `#security`, `#file-synchronization`, `#open-source`

---

<a id="item-9"></a>
## [OpenRouter raises $113M Series B](https://openrouter.ai/announcements/series-b) ⭐️ 8.0/10

OpenRouter announced a $113 million Series B funding round, highlighting its growth as a critical LLM API proxy and billing platform. This funding round underscores the increasing demand for unified access to multiple LLMs and centralized billing management, which simplifies AI development for builders everywhere. The company remains founder-led and founder-controlled, aiming to continue building products for AI developers. OpenRouter charges a small surcharge on expensive models but offers low-friction model experimentation and hard billing caps.

hackernews · freeCandy · May 30, 17:27 · [Discussion](https://news.ycombinator.com/item?id=48338660)

**Background**: An LLM API proxy acts as an intermediary between users and multiple large language model providers, offering a unified API, centralized billing, and easy model switching. OpenRouter is a hosted version of this concept, enabling developers to access many models without managing separate accounts and API keys for each provider.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/Mirrowel/LLM-API-Key-Proxy">GitHub - Mirrowel/LLM-API-Key-Proxy: Universal LLM Gateway: One API, every LLM. OpenAI/Anthropic-compatible endpoints with multi-provider translation and intelligent load-balancing. · GitHub</a></li>
<li><a href="https://docs.litellm.ai/docs/simple_proxy">LiteLLM AI Gateway (LLM Proxy) | liteLLM</a></li>

</ul>
</details>

**Discussion**: Comments were mixed but generally positive: SimonW initially skeptical but now sees value in billing caps and ease of use; numlocked stressed founder control and long-term commitment; minimaxir praised model experimentation but noted the surcharge on expensive models; others questioned the open-source nature of the name and expressed confusion over the branding.

**Tags**: `#LLM`, `#AI Infrastructure`, `#Funding`, `#API Proxy`, `#OpenRouter`

---

<a id="item-10"></a>
## [Pope Leo's first encyclical attacks technological messianism](https://www.economist.com/europe/2026/05/28/leos-first-encyclical-attacks-technological-messianism) ⭐️ 8.0/10

Pope Leo published his first encyclical, which explicitly criticizes technological messianism—the belief that technology, particularly AI and transhumanism, can save humanity. The document targets the rhetoric of tech leaders like Sam Altman and Dario Amodei, who have spoken of creating a religion or building a god. This encyclical marks a significant cultural intervention from a major religious authority, adding moral and philosophical weight to the growing debate over AI, transhumanism, and who should control technology. It could influence public discourse and policy by framing unchecked techno-optimism as a form of idolatry. The encyclical likely argues that technological messianism diverts attention from human and spiritual needs, and calls for a human-centered approach to innovation. It specifically rebukes the idea that AI could achieve consciousness or superintelligence, echoing critics who view current LLMs as pseudo-AI requiring human oversight.

hackernews · 1vuio0pswjnm7 · May 30, 10:30 · [Discussion](https://news.ycombinator.com/item?id=48334710)

**Background**: Technological messianism is the belief that technology will bring about salvation or utopia, often linked to transhumanist goals of enhancing human capabilities through AI, genetic engineering, and nanotechnology. Papal encyclicals are authoritative letters from the Pope to the Catholic Church addressing moral and social issues, carrying significant weight among billions of Catholics worldwide.

<details><summary>References</summary>
<ul>
<li><a href="https://www.catholicity.com/commentary/shea/02282.html">Mark Shea: Technological Messianism</a></li>
<li><a href="https://www.merriam-webster.com/dictionary/messianism">MESSIANISM Definition & Meaning - Merriam-Webster</a></li>
<li><a href="https://en.wikipedia.org/wiki/Transhumanism">Transhumanism - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters engage deeply with the encyclical's themes, with some (like alecco) arguing that AI CEOs exhibit 'AI psychosis' and that LLMs are powerful but not true AI. Others (like merelydev) frame the issue as a power struggle over who controls technology—technologists, users, governments, or now priests. The discussion also references Peter Thiel's views on the antichrist and existential risks.

**Tags**: `#religion`, `#artificial intelligence`, `#technology criticism`, `#transhumanism`, `#philosophy`

---

<a id="item-11"></a>
## [Anthropic Details Claude Sandboxing Across Products](https://simonwillison.net/2026/May/30/how-we-contain-claude/#atom-everything) ⭐️ 8.0/10

Anthropic published a detailed technical overview of sandbox techniques used to contain Claude across its products, including Claude.ai, Claude Code, and Cowork. This addresses a common lack of transparency in sandboxing documentation, helping users and developers assess the security of AI agents and their potential risks. Claude.ai uses gVisor, Claude Code uses Seatbelt on macOS and Bubblewrap on Linux, and Cowork runs full VMs via Apple's Virtualization framework or HCS on Windows.

rss · Simon Willison · May 30, 21:36

**Background**: Sandboxing is a security technique that isolates applications or processes to limit potential damage from exploits or misbehavior. gVisor is a Google-developed container sandbox that implements Linux system calls in userspace, while Seatbelt is Apple's sandbox kernel extension for macOS, and Bubblewrap is a lightweight unprivileged sandboxing tool used by Flatpak and others.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GVisor">gVisor - Wikipedia</a></li>
<li><a href="https://theapplewiki.com/wiki/Dev:Seatbelt">Dev:Seatbelt - The Apple Wiki</a></li>
<li><a href="https://wiki.archlinux.org/title/Bubblewrap">Bubblewrap - ArchWiki</a></li>

</ul>
</details>

**Tags**: `#AI`, `#security`, `#sandbox`, `#Anthropic`, `#Claude`

---

<a id="item-12"></a>
## [Running Python ASGI Apps in Browser with Pyodide and Service Workers](https://simonwillison.net/2026/May/30/pyodide-asgi-browser/#atom-everything) ⭐️ 8.0/10

Simon Willison demonstrated a method to run Python ASGI applications in the browser using Pyodide and a Service Worker, enabling correct execution of JavaScript in script tags, which was previously impossible with Web Workers. This advancement significantly enhances the capability of Python-in-browser applications like Datasette Lite, allowing full support for plugins and features that rely on JavaScript. It opens up new possibilities for running server-side Python frameworks entirely on the client side. The approach uses a Service Worker to intercept network requests and serve responses generated by the ASGI app running in Pyodide, ensuring that embedded script tags are executed by the browser. Simon Willison used Claude Opus 4.8 via Claude Code to develop the solution.

rss · Simon Willison · May 30, 21:02

**Background**: ASGI (Asynchronous Server Gateway Interface) is a standard for async Python web servers and applications, succeeding WSGI. Pyodide is a port of CPython to WebAssembly, allowing Python to run in the browser. Service Workers act as proxy servers in the browser, intercepting network requests. Previously, running Python in the browser with Web Workers prevented JavaScript in script tags from executing because responses were fetched as text.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Asynchronous_Server_Gateway_Interface">Asynchronous Server Gateway Interface - Wikipedia</a></li>
<li><a href="https://github.com/pyodide/pyodide">pyodide / pyodide : Pyodide is a Python distribution for the browser ...</a></li>
<li><a href="https://asgi.readthedocs.io/">ASGI Documentation — ASGI 3.0 documentation</a></li>

</ul>
</details>

**Tags**: `#Python`, `#ASGI`, `#WebAssembly`, `#Service Workers`, `#Pyodide`

---

<a id="item-13"></a>
## [SpaceX wins $4.16B US military satellite missile tracking contract](https://www.bloomberg.com/news/articles/2026-05-29/spacex-wins-4-billion-contract-for-us-golden-dome-satellites) ⭐️ 8.0/10

SpaceX was awarded a $4.16 billion contract by the U.S. Space Force to build a space-based tracking network for identifying and tracking airborne threats such as missiles and aircraft, as part of the Golden Dome defense program. This contract marks a significant expansion of SpaceX's role in national security space systems, potentially reducing coverage gaps of ground-based sensors and enabling tracking of advanced threats like hypersonic missiles. It also reinforces the shift toward commercial partnerships for critical defense infrastructure. The tracking network will integrate space-based sensors, communication systems, and ground processing capabilities. SpaceX had previously participated in Golden Dome's space-based interceptor prototype development and joined a multi-company alliance for the program's underlying software.

telegram · zaihuapd · May 30, 01:53

**Background**: The Golden Dome program is a U.S. missile defense initiative announced in 2025 to protect the entire country from missile attacks. Current missile warning satellites are optimized for traditional ballistic missiles with predictable trajectories, but struggle to track hypersonic missiles that maneuver unpredictably at speeds over Mach 5. Space-based sensors aim to fill detection gaps compared to ground-based radars and aircraft.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Golden_Dome_(missile_defense_system)">Golden Dome (missile defense system) - Wikipedia</a></li>
<li><a href="https://www.airandspaceforces.com/article/enhanced-space-based-missile-tracking/">Enhanced Space - Based Missile Tracking | Air & Space Forces...</a></li>
<li><a href="https://arstechnica.com/space/2025/07/pentagon-may-put-spacex-at-the-center-of-a-sensor-to-shooter-targeting-network/">Pentagon may put SpaceX at the center of... - Ars Technica</a></li>

</ul>
</details>

**Tags**: `#SpaceX`, `#defense`, `#space technology`, `#satellite`, `#military`

---

<a id="item-14"></a>
## [New FROST attack exploits SSD timing to spy on browser activity](https://futurism.com/future-society/websites-spying-solid-state-drive) ⭐️ 8.0/10

Researchers have disclosed a zero-interaction attack named FROST that leverages the browser's Origin Private File System (OPFS) and SSD read/write timing to infer which websites or applications a user is concurrently accessing. FROST achieves high accuracy (88.95% for websites, 95.83% for apps) without requiring any software installation or user interaction, raising significant privacy concerns as it reveals a new side-channel vector through standard web APIs. The attack was tested only on macOS and Linux, but researchers claim Windows is not immune; closing browser tabs when not in use can reduce the risk. FROST uses timing measurements of OPFS operations to create a fingerprint of concurrent activity.

telegram · zaihuapd · May 31, 01:55

**Background**: The Origin Private File System (OPFS) is a browser API that provides a sandboxed file system for each origin, designed for fast I/O operations. Side-channel attacks infer sensitive information by measuring indirect effects like timing variations. FROST exploits the fact that SSD read/write speeds vary depending on concurrent activity, allowing a malicious site to monitor other tabs or apps.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomshardware.com/tech-industry/cyber-security/researchers-say-they-can-spy-on-your-browsing-by-measuring-ssd-activity-through-a-browser-api">Researchers say they can spy on your browsing by measuring SSD activity through a browser API - Tom's Hardware</a></li>
<li><a href="https://arstechnica.com/security/2026/05/websites-have-a-new-way-to-spy-on-visitors-analyzing-their-ssd-activity/">Websites have a new way to spy on visitors: Analyzing their SSD activity - Ars Technica</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/File_System_API/Origin_private_file_system">Origin private file system - Web APIs | MDN</a></li>

</ul>
</details>

**Tags**: `#security`, `#side-channel`, `#SSD`, `#browser privacy`, `#FROST`

---