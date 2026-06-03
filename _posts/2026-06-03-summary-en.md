---
layout: default
title: "Horizon Summary: 2026-06-03 (EN)"
date: 2026-06-03
lang: en
---

> From 36 items, 7 important content pieces were selected

---

1. [Hackers Exploit Meta AI Bot to Hijack Instagram Accounts](#item-1) ⭐️ 9.0/10
2. [CT scans reveal BYD build quality and vertical integration](#item-2) ⭐️ 8.0/10
3. [Walking Tour of Seattle's Surveillance Infrastructure (2020)](#item-3) ⭐️ 8.0/10
4. [KDE Plasma's Last X11 Release Signals Full Wayland Transition](#item-4) ⭐️ 8.0/10
5. [Microsoft Unveils Efficient MAI LLMs with Low Active Parameters](#item-5) ⭐️ 8.0/10
6. [Trump signs AI executive order for voluntary model reviews](#item-6) ⭐️ 8.0/10
7. [Google Pays Play Store Devs for Code to Train AI](#item-7) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Hackers Exploit Meta AI Bot to Hijack Instagram Accounts](https://simonwillison.net/2026/Jun/1/hackers-simply-asked-meta-ai/#atom-everything) ⭐️ 9.0/10

Hackers successfully took over high-profile Instagram accounts by simply asking Meta's AI support chatbot to change the linked email address, a vulnerability verified by multiple sources. This vulnerability demonstrates a critical failure in integrating AI with account recovery systems, allowing unauthorized account takeovers with minimal effort and highlighting dangers of insufficient safeguards. The attack involved starting a conversation with Meta's AI support bot and requesting to link a new email address for the target account, bypassing typical verification steps as the chatbot was wired to fast-forward through the entire account recovery process.

rss · Simon Willison · Jun 1, 21:14

**Background**: Prompt injection is a type of attack where malicious inputs trick an AI model into performing unintended actions. In this case, the AI chatbot lacked proper guardrails to distinguish legitimate requests from malicious ones, allowing simple prompts to trigger account recovery workflows. This incident is similar to other prompt injection attacks on AI-powered systems.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>
<li><a href="https://krebsonsecurity.com/2026/06/hackers-used-metas-ai-support-bot-to-seize-instagram-accounts/">Hackers Used Meta’s AI Support Bot to Seize Instagram Accounts ...</a></li>
<li><a href="https://www.bbc.com/news/articles/c98rzr72dpyo">Meta AI chatbot enabled hackers to access others' Instagram accounts</a></li>

</ul>
</details>

**Tags**: `#security`, `#AI`, `#Meta`, `#Instagram`, `#vulnerability`

---

<a id="item-2"></a>
## [CT scans reveal BYD build quality and vertical integration](https://www.lumafield.com/scan-of-the-month/byd) ⭐️ 8.0/10

LumaField published CT scans of BYD car parts, revealing impressive build quality and extensive vertical integration, challenging the 'Chinese car bad' narrative. This provides objective, data-driven evidence of BYD's manufacturing quality, potentially shifting consumer perceptions. It also highlights BYD's strategic vertical integration, a model historically used by Ford at scale. The scans show heavy-duty components like control arms and subframes. A community correction notes that the mechanical backup key is not hinged but pulls out via a clip.

hackernews · viasfo · Jun 2, 20:30 · [Discussion](https://news.ycombinator.com/item?id=48375824)

**Background**: Vertical integration refers to a company controlling multiple stages of production, from raw materials to final assembly. BYD produces about 75% of its components, similar to Tesla but at a larger production scale (4.6 million vehicles per year compared to Tesla's 1.6 million). Traditional automakers like Ford only produce around 25% of their components. CT scanning uses X-rays to create detailed 3D images of internal structures, enabling non-destructive quality analysis.

<details><summary>References</summary>
<ul>
<li><a href="https://supplychain360.io/operations/teslas-vertical-integration-revolutionizes-supply-chains/">Tesla's Vertical Integration Revolutionizes Supply Chains</a></li>
<li><a href="https://www.forbes.com/councils/forbesbusinesscouncil/2024/01/29/why-vertical-integration-is-the-path-to-strategic-advantage/">Why Vertical Integration Is The Path To Strategic Advantage</a></li>

</ul>
</details>

**Discussion**: A master technician praised BYD's heavy-duty components, contradicting negative stereotypes. Another user corrected a detail about the key mechanism. Commenters also noted BYD's organizational innovation and its scale of vertical integration compared to Tesla and Ford.

**Tags**: `#automotive`, `#engineering`, `#manufacturing`, `#BYD`, `#CT scanning`

---

<a id="item-3"></a>
## [Walking Tour of Seattle's Surveillance Infrastructure (2020)](https://coveillance.org/a-walking-tour-of-surveillance-infrastructure-in-seattle/) ⭐️ 8.0/10

The article provides a detailed on-the-ground examination of surveillance cameras in Seattle, documenting how these devices are deployed and the social agreements they enforce. This analysis is significant because it sparks high-engagement discussion on privacy, ethics, and technology, revealing how urban surveillance shapes social norms and raises concerns about a surveillance state. The article uses language like 'kinds of gazes' and 'encoding ways of seeing,' which some community members criticize as overly academic and inaccessible.

hackernews · eustoria · Jun 2, 13:24 · [Discussion](https://news.ycombinator.com/item?id=48369980)

**Background**: Urban surveillance infrastructure, including cameras and sensors, is increasingly common in cities worldwide. These systems are often justified for public safety and crime prevention, but critics argue they infringe on privacy and may reinforce societal inequalities. The discussion in Seattle reflects broader debates about the trade-off between security and civil liberties.

**Discussion**: Community comments express mixed views: some argue surveillance is necessary for safety given high crime rates and reluctance of juries to convict without video evidence, while others criticize the academic language of the article and worry about the erosion of freedom.

**Tags**: `#surveillance`, `#privacy`, `#ethics`, `#technology`, `#seattle`

---

<a id="item-4"></a>
## [KDE Plasma's Last X11 Release Signals Full Wayland Transition](https://blog.davidedmundson.co.uk/blog/596/) ⭐️ 8.0/10

KDE Plasma's upcoming release will be the last to support X11, meaning all future releases will exclusively use the Wayland display server protocol. This transition impacts millions of Linux desktop users, as Wayland offers improved security and performance but still lacks some features of X11, such as full accessibility support and window management capabilities. Moving to a single code path via Wayland will enable faster development and innovation, but users relying on X11-specific features like voice input tools (e.g., Talon) or per-application keyboard layouts may face regressions.

hackernews · jandeboevrie · Jun 2, 14:16 · [Discussion](https://news.ycombinator.com/item?id=48370588)

**Background**: X11 is the legacy display server protocol for Unix-like systems, while Wayland is its modern replacement designed to be simpler and more secure. KDE Plasma, a popular desktop environment, has been gradually improving Wayland support and now plans to drop X11 entirely.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Wayland_display_server">Wayland display server</a></li>
<li><a href="https://en.wikipedia.org/wiki/X_display_server">X display server</a></li>

</ul>
</details>

**Discussion**: Community comments express concern about accessibility regressions in Wayland, with some users noting missing features like persistent window positions and per-application keyboard layouts. Others praise KDE's progress in pushing Wayland forward.

**Tags**: `#KDE`, `#Wayland`, `#Linux desktop`, `#X11`, `#accessibility`

---

<a id="item-5"></a>
## [Microsoft Unveils Efficient MAI LLMs with Low Active Parameters](https://simonwillison.net/2026/Jun/2/microsofts-new-models/#atom-everything) ⭐️ 8.0/10

Microsoft announced two new text LLMs: MAI-Thinking-1, a 1 trillion parameter reasoning model with only 35 billion active parameters, and MAI-Code-1-Flash, a 137 billion parameter code model with 5 billion active parameters, both using Mixture-of-Experts architecture. These models demonstrate that high performance can be achieved with significantly fewer active parameters, potentially reducing deployment costs and energy consumption. They also highlight Microsoft's investment in efficient AI, though the training data still relies on large-scale web crawling with ongoing licensing debates. MAI-Thinking-1 is a reasoning model for select early partners, while MAI-Code-1-Flash is rolling out to GitHub Copilot users in VS Code. The training data includes a proprietary crawl filtered from 1.2 trillion to 794 billion pages, plus Common Crawl, with filtering for AI-generated content and adult/ piracy domains.

rss · Simon Willison · Jun 2, 22:21

**Background**: Mixture-of-Experts (MoE) architecture activates only a subset of parameters per input, reducing computation while maintaining model capacity. Total parameter count includes all parameters, while active parameters are those used in a single forward pass; this distinction is key to understanding models like MAI-Thinking-1 (1T total, 35B active).

<details><summary>References</summary>
<ul>
<li><a href="https://www.f22labs.com/blogs/active-vs-total-parameters-whats-the-difference/">Active vs Total Parameters: What's the Difference?</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Microsoft`, `#LLMs`, `#model efficiency`

---

<a id="item-6"></a>
## [Trump signs AI executive order for voluntary model reviews](https://www.whitehouse.gov/presidential-actions/2026/06/promoting-advanced-artificial-intelligence-innovation-and-security/) ⭐️ 8.0/10

On June 2, 2026, President Donald Trump signed an executive order establishing a voluntary framework for AI developers to submit advanced AI models to the government for cybersecurity review 30 days before public release. This order signals the U.S. government's intent to balance AI innovation with national security through a collaborative, non-mandatory approach, potentially setting a precedent for future AI regulation. The review period was shortened from an initially proposed 90 days to 30 days after industry pushback, and the order explicitly prohibits any mandatory government licensing or pre-approval mechanisms.

telegram · zaihuapd · Jun 2, 16:44

**Background**: The executive order targets "covered frontier models" — the most advanced and potentially risky AI systems. It also directs the Treasury, Defense, and Homeland Security departments to create an AI cybersecurity clearinghouse to coordinate vulnerability scanning and patching. This voluntary review builds on earlier debates about whether AI should be regulated like drugs or medical devices.

<details><summary>References</summary>
<ul>
<li><a href="https://www.implicator.ai/trump-signs-ai-order-for-voluntary-pre-release-cyber-reviews/">Trump signs voluntary AI cyber review order</a></li>
<li><a href="https://thenextweb.com/news/trump-signs-downsized-ai-executive-order-voluntary-review">Trump signs narrowed AI order with voluntary 30-day model review</a></li>
<li><a href="https://federalnewsnetwork.com/cybersecurity/2026/06/ai-executive-order-sets-stage-for-new-cybersecurity-directives/">AI executive order sets stage for new cybersecurity directives | Federal News Network</a></li>

</ul>
</details>

**Tags**: `#AI regulation`, `#executive order`, `#cybersecurity`, `#US policy`, `#AI safety`

---

<a id="item-7"></a>
## [Google Pays Play Store Devs for Code to Train AI](https://www.neowin.net/reports/google-wants-to-pay-play-store-developers-for-code-to-train-its-ai/) ⭐️ 8.0/10

Google is privately contacting Android developers to offer payment for non-exclusive access to their private codebases, which will be used to train its AI models and improve development tools. This move helps Google narrow the gap with competitors like GitHub Copilot and Claude Code in AI-assisted coding, and offers developers a new revenue stream while potentially leading to better Android development tools. The arrangement is non-exclusive, meaning developers retain 100% intellectual property rights and can license their code elsewhere. Google plans to use the code to train its Gemini models and enhance tools like Antigravity 2.0.

telegram · zaihuapd · Jun 3, 02:47

**Background**: Large language models for code generation, such as GitHub Copilot and Claude Code, rely on vast codebases for training. Google's Gemini competes in this space but has lagged behind. To catch up, Google is pursuing a novel data sourcing strategy by directly incentivizing developers to contribute high-quality private code.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://antigravity.google/product/antigravity-2">Google Antigravity - Antigravity 2.0</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Google`, `#Android`, `#Code Generation`, `#Developer Tools`

---