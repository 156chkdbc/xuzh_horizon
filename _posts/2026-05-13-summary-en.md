---
layout: default
title: "Horizon Summary: 2026-05-13 (EN)"
date: 2026-05-13
lang: en
---

> From 42 items, 13 important content pieces were selected

---

1. [Six CVEs Released for Serious dnsmasq Vulnerabilities](#item-1) ⭐️ 9.0/10
2. [DuckDB Introduces Quack Remote Protocol for Client-Server Architecture](#item-2) ⭐️ 9.0/10
3. [Canada’s Bill C-22 Revives Surveillance Nightmare with Backdoors](#item-3) ⭐️ 9.0/10
4. [Restore Full BambuNetwork for Bambu Lab Printers](#item-4) ⭐️ 8.0/10
5. [Needle: 26M Parameter Tool-Calling Model Open-Sourced](#item-5) ⭐️ 8.0/10
6. [Mitchell Hashimoto Critiques Risk-Averse Tech Decision Makers](#item-6) ⭐️ 8.0/10
7. [Shore: AI must cut maintenance costs to match productivity gains](#item-7) ⭐️ 8.0/10
8. [Your AI Use Is Breaking My Brain](#item-8) ⭐️ 8.0/10
9. [Unitree unveils GD01, first mass-produced manned deformable mecha](#item-9) ⭐️ 8.0/10
10. [Commerce Department Removes AI Safety Test Details](#item-10) ⭐️ 8.0/10
11. [SpaceX and Google in Talks for Orbital Data Center Launches](#item-11) ⭐️ 8.0/10
12. [Google Unveils Googlebook to Replace Chromebook with Gemini AI](#item-12) ⭐️ 8.0/10
13. [Google Announces Gemini Intelligence for Pixel and Samsung Devices](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Six CVEs Released for Serious dnsmasq Vulnerabilities](https://lists.thekelleys.org.uk/pipermail/dnsmasq-discuss/2026q2/018471.html) ⭐️ 9.0/10

CERT has released six new CVEs for serious security vulnerabilities in dnsmasq, a widely used DNS/DHCP server. The vulnerabilities impact memory safety and could lead to remote code execution. Given dnsmasq's pervasive presence in home routers, IoT devices, and Android, these vulnerabilities pose a significant threat to network security. This event also reignites debate about memory-safe languages in critical infrastructure. The six CVEs cover various memory corruption issues such as buffer overflows and use-after-free. Patches have been released in the latest dnsmasq version, but many distributions still run outdated versions.

hackernews · chizhik-pyzhik · May 12, 18:12 · [Discussion](https://news.ycombinator.com/item?id=48112042)

**Background**: dnsmasq is a lightweight daemon providing DNS caching, DHCP server, TFTP, and network boot features, commonly used in small networks and embedded devices. CVE (Common Vulnerabilities and Exposures) is a standardized system for identifying and cataloging security vulnerabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Dnsmasq">Dnsmasq</a></li>
<li><a href="https://en.wikipedia.org/wiki/Common_Vulnerabilities_and_Exposures">Common Vulnerabilities and Exposures - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community comments highlight the urgency of moving from memory-unsafe languages like C to memory-safe languages like Rust or Go, especially for critical network services. There is also frustration with Debian's slow patching of old dnsmasq versions, and concerns about OpenWRT users awaiting a fixed build.

**Tags**: `#security`, `#dnsmasq`, `#CVE`, `#memory safety`, `#open source`

---

<a id="item-2"></a>
## [DuckDB Introduces Quack Remote Protocol for Client-Server Architecture](https://duckdb.org/2026/05/12/quack-remote-protocol) ⭐️ 9.0/10

DuckDB announced the Quack remote protocol, enabling a client-server architecture that supports remote queries and horizontal scaling. This transforms DuckDB from a purely embedded database into a system capable of multi-process and remote access, broadening its use cases for analytics at scale. Quack builds on proven technologies like HTTP and is designed to be simple to set up, fast, and support multiple concurrent writers.

hackernews · aduffy · May 12, 17:54 · [Discussion](https://news.ycombinator.com/item?id=48111765)

**Background**: DuckDB is an in-process SQL database optimized for analytical queries, traditionally used as an embedded database without a separate server. Quack introduces a lightweight remote protocol, allowing clients to connect to a DuckDB server over the network, similar to traditional relational databases.

<details><summary>References</summary>
<ul>
<li><a href="https://duckdb.org/2026/05/12/quack-remote-protocol">Quack: The DuckDB Client - Server Protocol – DuckDB</a></li>
<li><a href="https://news.ycombinator.com/item?id=48111765">Quack: The DuckDB Client-Server Protocol | Hacker News</a></li>

</ul>
</details>

**Discussion**: Community comments are enthusiastic, with users appreciating the timing and practical benefits for sensor data and horizontal scaling. Some debate DuckDB's identity, but most see Quack as a natural evolution.

**Tags**: `#duckdb`, `#database`, `#protocol`, `#analytics`, `#scaling`

---

<a id="item-3"></a>
## [Canada’s Bill C-22 Revives Surveillance Nightmare with Backdoors](https://www.eff.org/deeplinks/2026/05/canadas-bill-c-22-repackaged-version-last-years-surveillance-nightmare) ⭐️ 9.0/10

The Electronic Frontier Foundation (EFF) warns that Canada's Bill C-22, a reintroduced surveillance bill, would mandate data retention and encryption backdoors, potentially forcing encrypted services like Signal to block Canadian users. If passed, this legislation would undermine end-to-end encryption and privacy rights, setting a dangerous precedent for other countries and threatening the availability of secure communication tools for Canadians. The bill requires telecommunications providers to retain metadata and implement capabilities that allow law enforcement to access encrypted communications, which technologists say is effectively an encryption backdoor.

hackernews · Brajeshwar · May 12, 17:35 · [Discussion](https://news.ycombinator.com/item?id=48111531)

**Background**: Mandatory data retention laws require companies to store user communications data for a set period, often used for surveillance. Encryption backdoors are deliberate vulnerabilities inserted into encryption systems to allow third-party access. Similar attempts in other countries have faced strong opposition from privacy advocates and tech companies.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Data_retention">Data retention - Wikipedia</a></li>
<li><a href="https://www.eff.org/issues/mandatory-data-retention">Mandatory Data Retention | Electronic Frontier Foundation</a></li>
<li><a href="https://www.internetsociety.org/blog/2025/05/what-is-an-encryption-backdoor/">What Is an Encryption Backdoor? - Internet Society</a></li>

</ul>
</details>

**Discussion**: The HN community expresses strong opposition, with commenters urging Canadians to contact their MPs. Some view the bill as a sign of government overreach, while others hope it will drive innovation in censorship-circumvention tools. A few commenters request French translations of the article to aid local advocacy.

**Tags**: `#surveillance`, `#encryption`, `#Canada`, `#privacy`, `#backdoors`

---

<a id="item-4"></a>
## [Restore Full BambuNetwork for Bambu Lab Printers](https://github.com/FULU-Foundation/OrcaSlicer-bambulab) ⭐️ 8.0/10

A GitHub repository was created to restore full BambuNetwork support for Bambu Lab printers, bypassing the company's controversial cloud authentication changes. This move could significantly impact user autonomy and open-source 3D printing, as it challenges Bambu Lab's control over printer access and raises questions about vendor lock-in. The repository appears to be a clone of an earlier state that sparked controversy, and the change means users must use Bambu Studio or Bambu Connect for cloud printing, while LAN Developer Mode disables cloud features.

hackernews · Murfalo · May 12, 21:55 · [Discussion](https://news.ycombinator.com/item?id=48115127)

**Background**: Bambu Lab recently implemented a new authorization system that requires cloud authentication even for LAN-based operations, unless users switch to LAN Developer Mode which disables cloud connectivity. This change has been controversial among users who value local control and third-party software like OrcaSlicer. The GitHub repository aims to restore the previous functionality that allowed direct network printing without mandatory cloud authentication.

<details><summary>References</summary>
<ul>
<li><a href="https://consumerrights.wiki/w/Bambu_Lab_Authorization_Control_System">Bambu Lab Authorization Control System - Consumer Rights Wiki</a></li>
<li><a href="https://www.xda-developers.com/finally-have-full-control-bambu-lab-printer-ditched-bambu-cloud/">I finally have full control of my Bambu Lab printer, but it meant ditching Bambu's cloud</a></li>

</ul>
</details>

**Discussion**: The community comments show mixed reactions: some users are concerned about Bambu Lab's motivations and the loss of local control, while others criticize the squashing of git history in the repository. There is also debate about the definition of 'full support' and whether it should include cloud tethering.

**Tags**: `#3D printing`, `#open-source`, `#firmware`, `#controversy`, `#Bambu Lab`

---

<a id="item-5"></a>
## [Needle: 26M Parameter Tool-Calling Model Open-Sourced](https://github.com/cactus-compute/needle) ⭐️ 8.0/10

Needle, a 26M parameter function-calling model built entirely from attention layers without MLPs, has been open-sourced. It achieves 6000 tok/s prefill and 1200 tok/s decode on consumer devices, trained on 200B tokens of pretraining and 2B tokens of synthesized function-calling data. This demonstrates that tiny, specialized models can outperform larger models on tool-calling tasks, enabling budget-friendly agentic systems on phones, watches, and other consumer devices. It challenges the assumption that large reasoning models are necessary for structured JSON output and tool use. The model uses 'Simple Attention Networks' with only attention and gating, completely removing feed-forward networks (FFNs). It was post-trained on data synthesized via Gemini covering 15 tool categories like timers, messaging, navigation, and smart home.

hackernews · HenryNdubuaku · May 12, 18:03 · [Discussion](https://news.ycombinator.com/item?id=48111896)

**Background**: Tool calling (also known as function calling) is the ability of an AI model to invoke external tools or APIs by outputting structured JSON, enabling it to perform actions beyond text generation. Traditional transformer models rely on feed-forward layers to store factual knowledge, but Needle's approach shows that for tasks where relevant information is provided in the input (e.g., tool definitions), attention alone suffices, eliminating the need for large memorization capacity.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@rajguntuku07/tool-calling-in-ai-3336c50b51ae">Tool Calling in AI . AI has developed so much, and there is | Medium</a></li>
<li><a href="https://github.com/cactus-compute/needle/blob/main/docs/simple_attention_networks.md">needle/docs/ simple _ attention _ networks .md at main...</a></li>
<li><a href="https://grokipedia.com/page/tool-calling-ai">Tool calling (AI)</a></li>

</ul>
</details>

**Discussion**: Commenters expressed interest in the model's discriminatory power for complex tool use, with one noting that simple weather queries are easily handled and asking about more nuanced cases. Others suggested publishing a live demo for easier testing, and appreciated the push for tiny models to enable privacy-first desktop and mobile agents.

**Tags**: `#tool calling`, `#small language models`, `#attention networks`, `#efficient inference`, `#open-source`

---

<a id="item-6"></a>
## [Mitchell Hashimoto Critiques Risk-Averse Tech Decision Makers](https://simonwillison.net/2026/May/12/mitchell-hashimoto/#atom-everything) ⭐️ 8.0/10

Mitchell Hashimoto, co-founder of HashiCorp, sharply criticized Technical Decision Makers (TDMs) for prioritizing job security over innovation, describing them as risk-averse followers of analyst trends. This critique resonates deeply in the tech industry, highlighting a cultural tension between innovative engineers and enterprise decision-makers who rely on Gartner and McKinsey reports, potentially stifling real progress. Hashimoto made the remarks in a Lobsters discussion about Redis's homepage design, contrasting TDMs' 9-to-5 mindset with hobbyist developers who explore new technologies on weekends.

rss · Simon Willison · May 12, 22:21

**Background**: Mitchell Hashimoto is a well-known figure in DevOps and infrastructure, having co-founded HashiCorp, which created tools like Terraform and Vagrant. Technical Decision Makers (TDMs) are individuals in organizations who choose which technologies to adopt, often influenced by analyst firms like Gartner.

**Tags**: `#decision-making`, `#enterprise`, `#analyst influence`, `#risk aversion`

---

<a id="item-7"></a>
## [Shore: AI must cut maintenance costs to match productivity gains](https://simonwillison.net/2026/May/11/james-shore/#atom-everything) ⭐️ 8.0/10

James Shore argues that AI coding agents must reduce maintenance costs by the same factor they boost code production, or teams risk unsustainable technical debt. This insight highlights a critical pitfall in AI-assisted development: without proportional maintenance cost reduction, productivity gains will be offset by exponentially growing maintenance burdens, potentially crippling long-term software projects. Shore uses simple math: doubling code output while holding maintenance costs steady doubles total maintenance costs; quadrupling output without proportional reduction increases costs fourfold. He warns that current AI tools primarily generate code, not reduce maintenance.

rss · Simon Willison · May 11, 19:48

**Background**: Technical debt refers to the implied cost of future rework caused by choosing an easy solution now instead of a better approach that would take longer. In software, maintenance costs often outweigh initial development costs over a project's lifetime. AI coding agents can boost initial productivity but may generate code that is harder to maintain, increasing long-term costs.

**Tags**: `#AI-assisted-development`, `#software-maintenance`, `#productivity`, `#technical-debt`

---

<a id="item-8"></a>
## [Your AI Use Is Breaking My Brain](https://simonwillison.net/2026/May/11/zombie-internet/#atom-everything) ⭐️ 8.0/10

Jason Koebler published an article on 404 Media criticizing the pervasive use of AI-generated content online, coining the term 'Zombie Internet' to describe the confusing mix of human and AI writing, and arguing that filtering such content is mentally exhausting. This article captures a growing frustration with AI-generated slop online, providing a memorable term that highlights the erosion of content authenticity and the psychological burden on users. It adds to the debate about the future of the internet and human-AI interaction. Koebler distinguishes the 'Zombie Internet' from the 'Dead Internet' theory by emphasizing that it involves real people interacting with AI agents and AI-augmented individuals, not just bots. The term originally referred to compromised computers used for cyberattacks, but Koebler repurposes it to describe the current online environment.

rss · Simon Willison · May 11, 19:21

**Background**: The 'Dead Internet' theory is a conspiracy theory claiming that most internet activity since 2016 is generated by bots and algorithms, not humans. The term 'Zombie Internet' had earlier cybersecurity connotations but is now used by Koebler to describe a more nuanced reality where humans and AI intermingle, creating a confusing and exhausting online experience. This concept has gained traction as AI-generated content proliferates across social media and publishing platforms.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Dead_Internet_theory">Dead Internet theory</a></li>
<li><a href="https://www.fastcompany.com/91489308/zombie-internet-devastating-consequences-advertising-social-media-human-web-dead-internet-moltbook-ai-tbpn">The ‘zombie internet’ has arrived—and it has devastating consequences for advertising, social media, and the human web</a></li>

</ul>
</details>

**Tags**: `#AI impact`, `#internet culture`, `#content quality`, `#zombie internet`, `#information overload`

---

<a id="item-9"></a>
## [Unitree unveils GD01, first mass-produced manned deformable mecha](https://m.mydrivers.com/newsview/1121657.html) ⭐️ 8.0/10

Unitree has unveiled the GD01, the world's first mass-produced manned deformable mecha, pricing starts at 3.9 million yuan. The vehicle can transform between bipedal and quadrupedal modes for different terrains. This marks a significant milestone in robotics and consumer hardware, being the first mass-produced manned mecha. While the high price limits its audience, it showcases advanced deformation technology and could inspire future applications in tourism, special operations, and luxury transport. The GD01 weighs approximately 500 kg, uses high-strength alloys and precision servo drives, and can punch through a brick wall in demonstrations. It is designed for civilian transport, with a focus on entertainment, special operations, and private high-end mobility.

telegram · zaihuapd · May 12, 05:25

**Background**: Mecha refers to large humanoid or animal-like machines, often depicted in science fiction. A transforming mecha can change its shape, typically between a vehicle and a robot, a concept pioneered by Japanese designers in the 1980s. Servo drives are electronic amplifiers that control motor torque, speed, and position, essential for precise movements in robotics like the GD01's deformation and locomotion.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Servo_drive">Servo drive - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mecha">Mecha - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#robotics`, `#mecha`, `#unitree`, `#hardware`, `#innovation`

---

<a id="item-10"></a>
## [Commerce Department Removes AI Safety Test Details](https://www.reuters.com/legal/litigation/microsoft-google-xai-security-test-details-deleted-us-government-website-2026-05-11/) ⭐️ 8.0/10

The US Commerce Department removed web pages detailing agreements with Google, xAI, and Microsoft for pre-deployment AI security testing by government scientists. The pages initially showed a 404 error and now redirect to the Center for AI Standards and Innovation (CAISI) website. This removal raises concerns about transparency and potential policy shifts in AI governance. It could signal a reduction in government oversight of AI safety, affecting public trust and the regulatory landscape for frontier AI models. The removed pages described voluntary agreements for pre-deployment security testing of advanced AI models. The reason for removal is unclear, and the Commerce Department and White House have not commented.

telegram · zaihuapd · May 12, 13:38

**Background**: AI safety institutes were established after the 2023 AI Safety Summit; the US counterpart was renamed to Center for AI Standards and Innovation (CAISI) in 2025. Pre-deployment testing involves red-teaming and vulnerability assessments before AI models are released to the public.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Center_for_AI_Standards_and_Innovation">Center for AI Standards and Innovation</a></li>
<li><a href="https://en.wikipedia.org/wiki/Artificial_intelligence_safety_institute">Artificial intelligence safety institute - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#government regulation`, `#transparency`, `#big tech`, `#policy`

---

<a id="item-11"></a>
## [SpaceX and Google in Talks for Orbital Data Center Launches](https://www.wsj.com/tech/spacex-google-in-talks-to-explore-data-centers-in-orbit-7b7799e2) ⭐️ 8.0/10

SpaceX and Google are discussing a rocket launch agreement to deploy Google's orbital data centers under Project Suncatcher, with prototype satellites potentially launching by 2027. This collaboration could accelerate space-based AI computing infrastructure, reducing reliance on terrestrial data centers and enabling low-latency edge computing globally. Google has partnered with Planet Labs for satellite development and aims to leverage space-based solar power. SpaceX is also pitching orbital data centers as a key value driver for its upcoming IPO.

telegram · zaihuapd · May 12, 16:28

**Background**: Orbital data centers are proposed facilities in space that use solar power and free-space optical links for networking, bypassing Earth's energy and land constraints. Google's Project Suncatcher aims to deploy AI data centers in orbit, potentially offering up to 8x power advantage due to constant sunlight and cooling efficiency.

<details><summary>References</summary>
<ul>
<li><a href="https://arstechnica.com/google/2025/11/meet-project-suncatcher-googles-plan-to-put-ai-data-centers-in-space/">Meet Project Suncatcher , Google ’s plan to put AI data centers in...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Space-based_data_center">Space-based data center - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Planet_Labs">Planet Labs - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#space`, `#data center`, `#satellite`, `#Google`, `#SpaceX`

---

<a id="item-12"></a>
## [Google Unveils Googlebook to Replace Chromebook with Gemini AI](https://www.techpowerup.com/348969/google-prepares-googlebook-as-a-chromebook-successor-powered-by-gemini) ⭐️ 8.0/10

Google announced the Googlebook laptop line, replacing Chromebook, with deep Gemini AI integration and Aluminium OS, a fusion of Android and ChromeOS, launching in fall 2026 with partners like Acer, ASUS, Dell, HP, and Lenovo. This marks a major shift in Google's computing strategy, moving from web-centric ChromeOS to a more capable Android-based OS with powerful AI features, potentially redefining laptop productivity and competition with Windows and macOS. Googlebooks will feature a hardware 'Glowbar' (RGB LED strip), a 'Magic Pointer' that provides AI-powered context and image generation based on screen content, and 'Cast My Apps' for controlling Android phones from the laptop. Aluminium OS is based on Android 16 and merges ChromeOS capabilities.

telegram · zaihuapd · May 13, 00:02

**Background**: Chromebooks are laptops running ChromeOS, a web-centric operating system from Google. Google now plans to replace them with Googlebook, running Aluminium OS—a fusion of Android and ChromeOS—to better support native apps and AI. Gemini is Google's multimodal AI model family; this integration aims to make the laptop more intelligent and context-aware.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/products-and-platforms/platforms/android/meet-googlebook/">Introducing Googlebook, designed for Gemini Intelligence</a></li>
<li><a href="https://9to5google.com/2026/05/12/deepmind-googlebook-magic-pointer/">DeepMind details Googlebook ‘ Magic Pointer ’ with demos you can try...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Aluminium_OS">Aluminium OS</a></li>

</ul>
</details>

**Tags**: `#Google`, `#Chromebook`, `#Gemini AI`, `#AI`, `#hardware`

---

<a id="item-13"></a>
## [Google Announces Gemini Intelligence for Pixel and Samsung Devices](https://9to5google.com/2026/05/12/gemini-intelligence-announcement/) ⭐️ 8.0/10

Google announced Gemini Intelligence, a suite of AI features for high-end Android devices, launching this summer on Pixel and Samsung Galaxy smartphones. This marks Google's major push into on-device AI, competing with Apple Intelligence and enhancing user productivity through automation and contextual understanding. Features include a new Material 3 visual language, task automation with screen context, Rambler speech input that converts natural speech into polished text, and custom widget creation via natural language.

telegram · zaihuapd · May 13, 00:32

**Background**: Material 3 is Google's latest design system with dynamic theming. Rambler was first presented as a research project and is now integrated into Gboard. On-device AI processing preserves user privacy while enabling new capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/products-and-platforms/platforms/android/gemini-intelligence/">A smarter, more proactive Android with Gemini Intelligence</a></li>
<li><a href="https://9to5google.com/2026/05/12/gemini-intelligence-announcement/">Gemini Intelligence brings gen UI widgets, Gboard 'Rambler' to Android, debuting on Pixel & Samsung</a></li>
<li><a href="https://en.wikipedia.org/wiki/Material_Design">Material Design - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Google`, `#Android`, `#Gemini`, `#Consumer Tech`

---