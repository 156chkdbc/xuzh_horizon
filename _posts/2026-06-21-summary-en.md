---
layout: default
title: "Horizon Summary: 2026-06-21 (EN)"
date: 2026-06-21
lang: en
---

> From 22 items, 5 important content pieces were selected

---

1. [3D Optical Fiber Micro-Tweezer Achieves 100,000x Force Boost](#item-1) ⭐️ 9.0/10
2. [SMPTE Makes Its Standards Freely Accessible](#item-2) ⭐️ 8.0/10
3. [Plagiarism of Obscure Sorrows by AI Site](#item-3) ⭐️ 8.0/10
4. [IETF Proposes HTTP QUERY Method with Body but Safe Semantics](#item-4) ⭐️ 8.0/10
5. [Tencent tests AI agent for WeChat, faces compute bottleneck](#item-5) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [3D Optical Fiber Micro-Tweezer Achieves 100,000x Force Boost](https://www.stdaily.com/web/gdxw/2026-06/19/content_534836.html) ⭐️ 9.0/10

Researchers from Anhui University and the University of Science and Technology of China have developed a novel 3D optical fiber micro-tweezer using femtosecond laser composite manufacturing. The device achieves precise manipulation of microscale objects with a force output 100,000 times greater than traditional optical tweezers, as published in Nature. This breakthrough overcomes the fundamental limitations of conventional optical tweezers, such as weak force and inability to manipulate opaque objects, and addresses the precision constraints of mechanical micro-grippers in confined spaces. It enables transformative applications in single-cell manipulation, micro-surgery, and biomedical research. The micro-tweezer integrates light transmission, photothermal conversion, material response, and mechanical output into a single optical fiber tip. By adjusting the input light power, continuous and precise force control is achieved, allowing operation in spaces as small as 100 micrometers.

telegram · zaihuapd · Jun 20, 15:19

**Background**: Traditional optical tweezers use focused laser beams to trap particles but exert forces only in the picoNewton range and cannot handle opaque objects. Mechanical micro-grippers, while stronger, are bulky and lack precision in tight spaces. This new approach combines photothermal effects with microstructured mechanical output, leveraging femtosecond laser fabrication to create a compact, high-force manipulator.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nature.com/articles/s41378-024-00757-7">Thermo-optical tweezers based on photothermal waveguides | Microsystems & Nanoengineering</a></li>
<li><a href="https://pubs.rsc.org/en/content/articlelanding/2024/mh/d4mh00500g">Femtosecond laser composite manufactured double-bionic...</a></li>

</ul>
</details>

**Tags**: `#optical tweezers`, `#biomedical engineering`, `#nanophotonics`, `#cell manipulation`, `#Nature`

---

<a id="item-2"></a>
## [SMPTE Makes Its Standards Freely Accessible](https://www.smpte.org/blog/smpte-makes-its-standards-freely-accessible-openingstandards-library-to-the-global-media-technology-community) ⭐️ 8.0/10

SMPTE has announced that it is making its entire library of over 800 standards freely available to the public, removing all previous paywalls as of now. This move fosters open standards in media technology, encouraging innovation, interoperability, and broader adoption across the industry. The initiative includes modernizing the standards development process through GitHub workflows, HTML-based authoring, and an integrated publishing pipeline.

hackernews · zdw · Jun 20, 17:01 · [Discussion](https://news.ycombinator.com/item?id=48610827)

**Background**: SMPTE (Society of Motion Picture and Television Engineers) is a globally recognized standards body that develops technical standards for motion imaging and television. These standards cover areas such as video compression, broadcast formats, and audio synchronization, and are critical for ensuring compatibility across devices and systems. Previously, access to these standards required a fee, which limited their adoption, especially among smaller developers and open-source projects.

<details><summary>References</summary>
<ul>
<li><a href="https://www.smpte.org/standards/overview">Standards Overview | Society of Motion Picture & Television ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Category:SMPTE_standards">Category: SMPTE standards - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The community reaction is overwhelmingly positive, with commenters applauding the move as long overdue and essential for open development. Some highlight the historical success of free standards like those from IETF, while others note the modernization efforts such as GitHub integration as a welcome change.

**Tags**: `#standards`, `#open-access`, `#media-technology`, `#SMPTE`, `#broadcasting`

---

<a id="item-3"></a>
## [Plagiarism of Obscure Sorrows by AI Site](https://waxy.org/2026/06/the-wholesale-plagiarism-of-obscure-sorrows/) ⭐️ 8.0/10

An article details how the entire book "Obscure Sorrows" by John Koenig was plagiarized verbatim on an AI-generated site, Qontour, which monetized the stolen content via Amazon affiliate links. This incident underscores the growing threat of AI-assisted plagiarism and the inadequacy of current copyright enforcement, leaving creators vulnerable. It highlights urgent need for platform accountability and updated legal frameworks. The plagiarized site contained the full foreword and all 311 neologisms from the book, and was monetized through Amazon Associates affiliate links. The site owner, Prompt Digital Inc (DBA Qontour), is a Webflow premium partner.

hackernews · ridesisapis · Jun 20, 18:05 · [Discussion](https://news.ycombinator.com/item?id=48611411)

**Background**: The Digital Millennium Copyright Act (DMCA) provides online service providers with a safe harbor from copyright liability if they promptly remove infringing content upon notification. However, AI-generated plagiarism presents new challenges, as automated systems can rapidly produce and host infringing content, complicating enforcement. This case exemplifies the gap between existing law and emerging technology.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DMCA_takedown_notice">DMCA takedown notice</a></li>
<li><a href="https://www.dmca.com/">Protect Your Online Content and Brand with DMCA Takedown ...</a></li>

</ul>
</details>

**Discussion**: Commenters shared similar experiences of AI-assisted theft, noting that DMCA takedowns are designed for such cases but often fail when platforms require court orders. Others pointed out that the plagiarist is a Webflow partner, calling for platform responsibility.

**Tags**: `#plagiarism`, `#AI`, `#copyright`, `#DMCA`, `#ethics`

---

<a id="item-4"></a>
## [IETF Proposes HTTP QUERY Method with Body but Safe Semantics](https://httpwg.org/http-extensions/draft-ietf-httpbis-safe-method-w-body.html) ⭐️ 8.0/10

The IETF HTTP Working Group has published a draft specification for a new HTTP QUERY method that allows sending query parameters in the request body while maintaining the safe and idempotent properties of GET. This draft was published on 27 May 2025 and expires in December 2026. This addresses a long-standing limitation where POST queries cannot be safely cached or retried, enabling more robust and efficient API interactions. If standardized, it could simplify RESTful API designs and improve performance through caching intermediaries. The QUERY method includes a new 'Accept-Query' response header so servers can declare supported query format media types. The draft is still under discussion and may change before finalization.

telegram · zaihuapd · Jun 20, 06:28

**Background**: HTTP methods are classified as safe (read-only, no side effects) or idempotent (multiple identical requests have the same effect as a single request). GET is both safe and idempotent, but its query string is limited in length. POST is neither safe nor idempotent because it typically creates or modifies resources, making caching and automatic retries problematic.

<details><summary>References</summary>
<ul>
<li><a href="https://httpwg.org/http-extensions/draft-ietf-httpbis-safe-method-w-body.html">The HTTP QUERY Method</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Glossary/Safe/HTTP">Safe (HTTP Methods) - Glossary - MDN Web Docs</a></li>
<li><a href="https://www.ietf.org/archive/id/draft-ietf-httpbis-safe-method-w-body-02.html">The HTTP QUERY Method</a></li>

</ul>
</details>

**Tags**: `#HTTP`, `#IETF`, `#network protocol`, `#specification`, `#query method`

---

<a id="item-5"></a>
## [Tencent tests AI agent for WeChat, faces compute bottleneck](https://t.me/zaihuapd/42072) ⭐️ 8.0/10

Tencent is testing an AI agent prototype integrated into WeChat, accessible via a right swipe on the main interface, allowing users to complete tasks like ordering coffee by voice or text commands. The company plans to apply for regulatory compliance approval as early as this month, followed by small-scale external testing before a phased rollout. This move signals Tencent's entry into the AI agent space, a key battlefield in China's AI competition where rivals Alibaba and ByteDance have already integrated similar features into their apps and seen rapid monthly active user growth. WeChat's massive user base (over 1 billion) could make this one of the largest deployments of AI agents, potentially reshaping how users interact with apps and services. Tencent faces a compute bottleneck: it has not stockpiled large quantities of Nvidia chips, and domestic semiconductor supply remains tight, making full-scale deployment costly and near-term profitability uncertain. The agent will invoke mini-programs to complete tasks, leveraging WeChat's existing ecosystem.

telegram · zaihuapd · Jun 20, 09:23

**Background**: AI agents are software programs that can autonomously perform tasks by perceiving their environment and taking actions, often powered by large language models. They have gained popularity in 2024-2025, with companies integrating them into apps to automate workflows like booking tickets or ordering food. Compute bottlenecks, especially GPU shortages and memory bandwidth limits, are common challenges in deploying AI models at scale, as highlighted by industry reports.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent - Wikipedia</a></li>
<li><a href="https://cloud.google.com/discover/what-are-ai-agents">What are AI agents? Definition, examples, and types | Google Cloud</a></li>
<li><a href="https://www.gradient.ai/blog/performance-bottlenecks-in-deploying-llms-a-primer-for-ml-researchers">Gradient Blog: Performance bottlenecks in deploying ...</a></li>

</ul>
</details>

**Tags**: `#AI agent`, `#WeChat`, `#Tencent`, `#AI competition`, `#compute bottleneck`

---