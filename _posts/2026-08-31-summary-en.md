---
layout: default
title: "Horizon Summary: 2026-08-31 (EN)"
date: 2026-08-31
lang: en
---

> From 29 items, 8 important content pieces were selected

---

1. [Sony Music Sues Anthropic for Using Pirated Content to Train Claude](#item-1) ⭐️ 9.0/10
2. [Kernel.org's Anubis Anti-Bot System Draws Sharp Community Criticism](#item-2) ⭐️ 8.0/10
3. [Critical QubesOS flaw allows code execution via copy-to-VM error reporting](#item-3) ⭐️ 8.0/10
4. [Omarchy vulnerability lets any user process escalate to root](#item-4) ⭐️ 8.0/10
5. [Simon Willison Explains ChatGPT Work's Two Products](#item-5) ⭐️ 8.0/10
6. [Tencent Releases Hy4 Preview, a 770B-Parameter Open-Weight LLM](#item-6) ⭐️ 8.0/10
7. [Apple Unveils M6 and M5 Ultra Chips with 2nm and Quad-Die Design](#item-7) ⭐️ 8.0/10
8. [Claude Shared Links Indexed by Google, Exposing Sensitive Data](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Sony Music Sues Anthropic for Using Pirated Content to Train Claude](https://www.musicbusinessworldwide.com/files/2026/08/COMPLAINT-in-Sony_Music_Publishing_US_LLC_e.pdf) ⭐️ 9.0/10

Sony Music Publishing, Warner Chappell Music, and other publishers filed a lawsuit in California federal court against Anthropic and its founders, alleging that Anthropic illegally downloaded over 7 million books from piracy libraries such as LibGen and PiLiMi and scraped lyrics to train its Claude AI models. The plaintiffs seek statutory damages of up to $150,000 per work and a permanent injunction, noting that similar previous lawsuits have already led to a $1.5 billion settlement. This lawsuit is a significant legal challenge to Anthropic and the broader AI industry, with the potential to set a precedent on whether copyrighted works can be used to train AI models. A ruling against Anthropic could lead to substantial financial damages, force AI companies to radically change how they collect training data, and have ripple effects across music publishing, book publishing, and generative AI. The complaint notably alleges that Anthropic removed copyright management information (CMI) from scraped lyrics, a separate violation under the Digital Millennium Copyright Act (17 U.S.C. § 1202). The defendants include Anthropic and its founders, and the suit cites the use of LibGen and PiLiMi shadow libraries; PiLiMi (Pirate Library Mirror) has previously admitted to deliberately violating copyright law in most countries.

telegram · zaihuapd · Aug 30, 01:00

**Background**: LibGen (Library Genesis) is a shadow library project that provides free access to paywalled scholarly articles and books, often without authorization, and publishers have accused it of internet piracy. PiLiMi (Pirate Library Mirror) is an anonymous effort that mirrored shadow libraries and has acknowledged deliberately violating copyright law. The DMCA's Section 1202 protects 'copyright management information' such as title, author, and copyright notices, making it illegal to remove or alter that information from a work. This lawsuit is part of a growing wave of litigation by authors, artists, and publishers against AI companies over the unlicensed use of copyrighted material in training data.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LibGen">LibGen</a></li>
<li><a href="https://en.wikipedia.org/wiki/Anna's_Archive">Anna's Archive - Wikipedia</a></li>
<li><a href="https://www.law.cornell.edu/uscode/text/17/1202">17 U.S. Code § 1202 - Integrity of copyright management information</a></li>

</ul>
</details>

**Tags**: `#AI`, `#copyright`, `#legal`, `#Anthropic`, `#music`

---

<a id="item-2"></a>
## [Kernel.org's Anubis Anti-Bot System Draws Sharp Community Criticism](https://people.kernel.org/monsieuricon/creepy-crawlies) ⭐️ 8.0/10

The kernel.org team's blog post 'Creepy Crawlies' defends its use of the Anubis proof-of-work anti-bot system to fend off AI crawlers, but community replies highlight severe usability problems. Commenters report that Anubis difficulty level 6 makes mobile access nearly impossible, and experts argue that proof-of-work inherently benefits bot operators over human users. Because kernel.org hosts the Linux kernel's canonical git repositories, anti-bot measures that frustrate legitimate users can harm the very community they aim to protect. This debate reflects a wider industry struggle to stop AI scrapers without collateral damage to mobile and low-resource users. Anubis uses hash-based proof-of-work challenges and is now deployed on kernel.org, lists.ffmpeg.org, and other FOSS sites. Kernel.org reportedly spends 14 CPU cores serving AI crawler requests, and commenters note that cgit's parameterized URLs generate billions of crawler-visible links.

hackernews · zdw · Aug 29, 17:49 · [Discussion](https://news.ycombinator.com/item?id=49491791)

**Background**: Anubis is an open-source "web AI firewall" that requires visitors to solve a proof-of-work challenge before viewing a page, in order to deter scripted scraping. Proof-of-work systems force clients to spend computational resources, which is intended to make bulk crawling expensive for bots. However, low-power mobile devices can struggle to solve the same puzzles, and sophisticated bot operators can use faster hardware or residential proxies to bypass the cost.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anubis_(software)">Anubis (software) - Wikipedia</a></li>
<li><a href="https://elsolitario.org/en/2026/08/30/kernel-org-ai-bots-anubis-cpu/">Kernel.org Burns 14 CPU Cores Tracking AI Crawlers</a></li>
<li><a href="https://github.com/TecharoHQ/anubis">Anubis - GitHub</a></li>

</ul>
</details>

**Discussion**: Commenters split between advocates for stronger anti-bot measures and critics of proof-of-work. Semiquaver calls Anubis's mobile experience 'unusable' at difficulty 6, while robotmay prefers LLM-based honeypot traps over PoW to waste scraper resources. Mzajc defends the challenge by noting bots indiscriminately hammer cgit servers, and tptacek echoes Tavis Ormandy's year-old critique that every scraper request is productive to the scraper, making PoW a poor defense.

**Tags**: `#anti-bot`, `#proof-of-work`, `#web scraping`, `#kernel.org`, `#infrastructure`

---

<a id="item-3"></a>
## [Critical QubesOS flaw allows code execution via copy-to-VM error reporting](https://www.qubes-os.org/news/2026/08/29/qsb-118/) ⭐️ 8.0/10

QubesOS disclosed QSB-118 on August 29, 2026, describing a critical vulnerability in the Dom0 copy-to-VM error reporting backchannel. A malicious qube can inject arbitrary commands into Dom0 when qvm-copy-to-vm is used from Dom0. This vulnerability undermines the core security boundary of QubesOS, potentially allowing a compromised or malicious VM to take over the entire system via Dom0. It highlights that even highly security-focused systems still have attack surface, and serves as an important case study for secure OS design. The VM variant of qvm-copy-to-vm is not affected, since its error reporting function does not use system(). The attack requires the user to copy a file from Dom0 to a malicious qube, meaning it is not a remote attack but does require no further user interaction once that action is taken.

hackernews · vntok · Aug 30, 08:51 · [Discussion](https://news.ycombinator.com/item?id=49496918)

**Background**: QubesOS is a security-focused desktop operating system that uses the Xen hypervisor to isolate applications and tasks into separate virtual machines (qubes). Dom0 is the privileged management domain that controls all other qubes, and qvm-copy-to-vm is a command-line tool for copying files between qubes. The error reporting backchannel in Dom0 invoked system() in a way that allowed command injection from a malicious qube.

<details><summary>References</summary>
<ul>
<li><a href="https://www.qubes-os.org/news/2026/08/29/qsb-118/">QSB-118: Dom0 arbitrary code execution in qvm-copy-to-vm error reporting | Qubes OS</a></li>
<li><a href="https://news.ycombinator.com/item?id=49496918">Arbitrary code execution in QubesOS via copy-to-VM error reporting backchannel | Hacker News</a></li>
<li><a href="http://www.mail-archive.com/qubes-users@googlegroups.com/msg39111.html">[qubes-users] QSB-118: Dom0 arbitrary code execution in qvm-copy-to-vm error reporting</a></li>

</ul>
</details>

**Discussion**: Community members generally acknowledged the severity but noted that the attack surface is limited, since Dom0 should not be used for regular or untrusted work. Some commented on the project's evolution after founder Joanna Rutkowska left, while one user questioned whether QubesOS is inherently more secure than BSD jails; responses emphasized the different security models and QubesOS's strength in compartmentalization.

**Tags**: `#security`, `#qubes`, `#vulnerability`, `#arbitrary code execution`, `#operating systems`

---

<a id="item-4"></a>
## [Omarchy vulnerability lets any user process escalate to root](https://0xcc.io/posts/omarchy-root-creds/) ⭐️ 8.0/10

A security researcher disclosed that Omarchy, an Arch-based Linux distribution, contains a default Docker configuration flaw allowing any user process to escalate to root without a password or sudo prompt. The issue is fixed in Omarchy 4.0.1. Because Omarchy is promoted as a modern, opinionated desktop OS, this flaw undermines trust in distributions that prioritize convenience over hardening, especially those associated with AI-assisted development. It also highlights the broader security risks of hype-driven and 'vibecoded' software, prompting users to question whether to trust new distros. The vulnerability stems from Omarchy's default Docker configuration, which effectively lets every program in the user's desktop session reach root without a password, sudo, or privilege prompt. Users are urged to update to 4.0.1, which removes the dangerous default configuration.

hackernews · trap0xcc · Aug 30, 15:59 · [Discussion](https://news.ycombinator.com/item?id=49499854)

**Background**: Omarchy is an opinionated Arch Linux-based distribution created by DHH (David Heinemeier Hansson), founder of 37signals, aimed at delivering a beautiful and practical desktop operating system. It gained attention partly through influencer hype, leading some security observers to warn against using 'vibecoded' distros that may skip rigorous review. Additionally, Linux desktop environments generally lack robust per-app sandboxing comparable to macOS, making privilege escalation issues particularly serious.

<details><summary>References</summary>
<ul>
<li><a href="https://0xcc.io/posts/omarchy-root-creds/">Omarchy : Any User Process Can Escalate to Root</a></li>
<li><a href="https://cyberpanel.net/blog/omarchy-linux-guide">Omarchy Linux : What Is It and Is It Worth Trying? 5 Min Read</a></li>
<li><a href="https://github.com/basecamp/omarchy">GitHub - basecamp/ omarchy : Beautiful, Modern & Opinionated Linux</a></li>

</ul>
</details>

**Discussion**: Community comments are largely skeptical and cautionary. Some argue that 'vibecoded' distros should not be trusted, pointing to an earlier Omarchy bug where USB descriptors flowed straight into the shell. Others advise sticking with mainstream distros like Ubuntu or using archinstall instead of hyped derivatives, while several note that Linux desktop sandboxing is weak, so any malicious process can already cause serious harm even without root.

**Tags**: `#security`, `#vulnerability`, `#linux`, `#privilege-escalation`, `#distro`

---

<a id="item-5"></a>
## [Simon Willison Explains ChatGPT Work's Two Products](https://simonwillison.net/2026/Aug/30/understanding-chatgpt-work/) ⭐️ 8.0/10

Simon Willison clarifies that OpenAI's ChatGPT Work actually consists of two distinct products: a cloud version (Work Cloud) and a local desktop app (Work Local, formerly Codex), and details the cloud version's exclusive features such as model selection, a persistent filesystem, and a headless browser. This clarification helps users and developers understand which ChatGPT Work offering to use, reducing confusion around a powerful but poorly described product. It also highlights how OpenAI is segmenting its AI offerings for different user needs and subscription tiers. Work Cloud offers GPT-5.6 Sol, Luna, and Terra models with reasoning levels from Light to Ultra, as well as GPT-5.5, while Chat offers a different selection including 5.6 Instant and Pro, with higher reasoning levels restricted to $100/month+ subscribers. Work is available only to $20/month and up subscribers, and Work Cloud includes code execution with internet access, a headless Chrome browser, a persistent shared filesystem, ChatGPT Sites publishing, sub-agents, and scheduled prompt automations.

rss · Simon Willison · Aug 30, 23:59

**Background**: ChatGPT Work is OpenAI's product aimed at helping users complete ambitious tasks with clear outcomes, such as creating briefs, decks, analyses, and workflows. It builds on OpenAI's Codex, an AI coding agent that can write code and fix bugs, which was released in April 2025 as Codex CLI and is available through ChatGPT and a desktop app. The GPT-5.6 models named Sol, Luna, and Terra appear to be the same models available through the OpenAI API, each with different capabilities and reasoning levels.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_Codex_(AI_agent)">OpenAI Codex (AI agent) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#ChatGPT`, `#OpenAI`, `#AI tools`, `#product analysis`, `#Simon Willison`

---

<a id="item-6"></a>
## [Tencent Releases Hy4 Preview, a 770B-Parameter Open-Weight LLM](https://simonwillison.net/2026/Aug/29/hy4/) ⭐️ 8.0/10

Tencent released Hy4 Preview, a new open-weight text-only LLM with 770B total parameters (49B active) and a 1M-token context window. The model weights, totaling 1.56TB, are available on Hugging Face. This is a major step up from Tencent's previous Hy3 model, nearly tripling total parameters and quadrupling the context window. It signals intensifying competition in open-weight frontier models, giving developers access to a very large MoE-style model with a million-token context. Hy4 uses reasoning effort levels 'high' (default) and 'no_think' (reasoning disabled), as shown in its chat template. It supports text input only, with no vision capabilities. Simon Willison's test showed the reasoning trace uses truncated English prose, likely for token efficiency.

rss · Simon Willison · Aug 29, 23:53

**Background**: Hy4 appears to use a Mixture-of-Experts (MoE) architecture, indicated by the large gap between total (770B) and active (49B) parameters. In MoE models, only a subset of parameters is activated per token, improving efficiency. An open-weight model shares trained weights but not necessarily training data or full open-source license, which is a key distinction in the AI community. A 1M-token context window lets models process entire codebases or long documents in a single pass.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://www.mindstudio.ai/blog/claude-1m-token-context-window-ai-agents">Claude 1M Token Context Window: What It Means for AI Agents and Long-Running Tasks | MindStudio</a></li>
<li><a href="https://deasadiqbal.medium.com/understanding-open-weights-vs-open-source-models-988b50ce64d7">Understanding Open Weights vs. Open Source Models | by Asad Iqbal | Medium</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#Tencent`, `#open-source`, `#AI`, `#Hugging Face`

---

<a id="item-7"></a>
## [Apple Unveils M6 and M5 Ultra Chips with 2nm and Quad-Die Design](https://t.me/zaihuapd/43505) ⭐️ 8.0/10

Apple announced the M6 and M5 Ultra chips, with the M6 debuting as its first 2nm processor (12-core CPU, 12-core GPU, dual 16-core Neural Engine, up to 170GB/s memory bandwidth) and the M5 Ultra featuring a quad-die architecture with up to 36 CPU cores, 80 GPU cores, 512GB memory, and 1.2TB/s bandwidth. This marks Apple's first move to 2nm process technology and the first quad-die design in the M series, delivering significant performance and memory bandwidth gains for AI and pro workloads. It strengthens Apple Silicon's competitive position against Intel, AMD, and other custom chip efforts. The M5 Ultra uses next-generation UltraFusion technology to connect two dual-die M5 Max chips into a unified processor. Apple also integrated dedicated Neural Accelerators into every GPU core across both families, boosting on-device AI performance.

telegram · zaihuapd · Aug 30, 16:41

**Background**: 2nm process refers to the latest generation of semiconductor fabrication nodes, offering higher transistor density and efficiency. In Apple Silicon, unified memory is a single pool of high-speed memory shared by the CPU, GPU, and Neural Engine, which avoids the separate system RAM and VRAM found in traditional PCs. The M6's 170GB/s and M5 Ultra's 1.2TB/s bandwidth enable large AI models to run locally without copying data between memory pools.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/2_nm_process">2 nm process - Wikipedia</a></li>
<li><a href="https://au.pcmag.com/processors/119512/apple-m5-ultra-and-m6-silicon-explained">Apple M5 Ultra and M6 Silicon Explained: 2nm Tech, Quad - Die Chips...</a></li>
<li><a href="https://www.hoxtonmacs.co.uk/blogs/news/what-is-unified-memory">What is Unified Memory – Hoxton Macs</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#chip design`, `#M6`, `#M5 Ultra`, `#hardware`

---

<a id="item-8"></a>
## [Claude Shared Links Indexed by Google, Exposing Sensitive Data](https://t.me/zaihuapd/43511) ⭐️ 8.0/10

A privacy flaw in Claude's shared conversation feature lets search engines index public links, exposing sensitive user data such as API keys, crypto wallets, resumes, legal records, internal project files, and social security numbers. Anthropic has not yet patched it, while ChatGPT faced a similar issue about a year ago and fixed it quickly. This is a major privacy vulnerability because indexed pages make sensitive data permanently discoverable via search, affecting any Claude user who shared a conversation. It erodes trust in AI assistants and underscores a recurring security gap across AI chatbots. The root cause is the absence of a noindex robots meta tag (or X-Robots-Tag) on Claude's shared conversation pages. Exposed data reportedly includes API keys, cryptocurrency wallets, resumes, attorney-client consultations, internal company documents, and social security numbers; users are advised to manually remove sensitive chats under Settings > Shared Conversations.

telegram · zaihuapd · Aug 31, 03:22

**Background**: Claude is a family of large language models created by Anthropic, first released as an AI chatbot in March 2023. The noindex directive is an HTML meta tag (or HTTP header) that tells search engines not to include a page in their results; without it, shared links can be indexed. A similar privacy incident with ChatGPT's shared links occurred roughly a year ago, which was quickly fixed.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_(AI)">Claude (AI)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Noindex">noindex - Wikipedia</a></li>
<li><a href="https://developers.google.com/search/docs/crawling-indexing/block-indexing">Block Search Indexing with noindex | Google Search Central ...</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#security`, `#claude`, `#vulnerability`, `#data-leak`

---