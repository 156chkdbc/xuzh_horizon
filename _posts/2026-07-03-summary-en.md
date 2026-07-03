---
layout: default
title: "Horizon Summary: 2026-07-03 (EN)"
date: 2026-07-03
lang: en
---

> From 33 items, 13 important content pieces were selected

---

1. [Virginia Bans Sale of Geolocation Data](#item-1) ⭐️ 8.0/10
2. [crustc: Entire Rust compiler translated to C](#item-2) ⭐️ 8.0/10
3. [Linux 6.9 bug breaks LUKS suspend key wiping](#item-3) ⭐️ 8.0/10
4. [PeerTube: A Decentralized, Federated Open-Source Video Platform](#item-4) ⭐️ 8.0/10
5. [Podman v6.0.0 Released with Network Improvements and Quadlet Support](#item-5) ⭐️ 8.0/10
6. [How to Ask for Help from Strangers Effectively](#item-6) ⭐️ 8.0/10
7. [Immich 3.0 Released: Major Update to Self-Hosted Photo Platform](#item-7) ⭐️ 8.0/10
8. [Apple Helped FBI Unmask Anonymous iCloud Email User](#item-8) ⭐️ 8.0/10
9. [Meta Plans to Sell Excess AI Compute, Enters Cloud Market](#item-9) ⭐️ 8.0/10
10. [Cloudflare to Block Mixed-Purpose AI Crawlers from September, Calls Out Google](#item-10) ⭐️ 8.0/10
11. [OpenAI Proposes US Government Take 5% Stake, Including Google & Meta](#item-11) ⭐️ 8.0/10
12. [Major Companies Restrict Employee AI Use Over Soaring Costs](#item-12) ⭐️ 8.0/10
13. [Anthropic in Talks with Samsung for Custom AI Chip Manufacturing](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Virginia Bans Sale of Geolocation Data](https://www.hunton.com/privacy-and-cybersecurity-law-blog/virginia-bans-sale-of-geolocation-data) ⭐️ 8.0/10

Virginia has enacted a ban on the sale of geolocation data, making it unlawful for any entity to sell or offer for sale such data collected from individuals in the state. This ban sets a significant precedent for privacy legislation in the U.S., directly impacting data brokers and tech companies that rely on location data for advertising and profiling. It may influence other states to adopt similar protections. The ban applies broadly to the sale of geolocation data, but enforcement remains a challenge, particularly with out-of-state corporations and evolving technologies like automated license plate readers (ALPR). The law does not specify penalties or enforcement mechanisms in detail.

hackernews · toomuchtodo · Jul 2, 21:03 · [Discussion](https://news.ycombinator.com/item?id=48767347)

**Background**: Geolocation data includes any information that identifies the physical location of a device or individual, such as GPS coordinates or Wi-Fi triangulation. This data is often collected by apps and services without explicit consent, then sold to third parties for advertising, risk assessment, or surveillance. Virginia's move follows growing public concern over privacy abuses, such as location data being used to target individuals visiting sensitive sites like abortion clinics.

**Discussion**: Commenters generally support the ban but highlight enforcement difficulties, such as how to regulate Delaware corporations that sell data collected in Virginia. They note real-world harms, like location data used for anti-abortion ads and car insurance tracking, and question whether ALPR companies can find loopholes.

**Tags**: `#privacy`, `#geolocation`, `#legislation`, `#data protection`, `#Virginia`

---

<a id="item-2"></a>
## [crustc: Entire Rust compiler translated to C](https://github.com/FractalFir/crustc) ⭐️ 8.0/10

A project called crustc has successfully translated the entire rustc compiler (version 1.98.0-nightly) into 46 million lines of C code, producing a functional Rust compiler that can be built with GCC and make. This enables bootstrapping Rust on hardware that lacks LLVM or GCC support, solving a key portability issue and allowing alternative compilers to be built without an existing Rust toolchain. The translated C code is 46 million lines and corresponds to rustc nightly from June 2026 (c712ea946). The project is the 14th known attempt at compiling Rust to C and has been in development for three years.

hackernews · Philpax · Jul 2, 22:57 · [Discussion](https://news.ycombinator.com/item?id=48768464)

**Background**: Bootstrapping is the technique of writing a compiler in its own language, requiring an initial compiler written in another language. Rust's official compiler, rustc, uses LLVM as its backend, which limits portability to platforms where LLVM or GCC is unavailable. Transpilation (source-to-source compilation) converts code from one high-level language to another, like from Rust to C, to leverage existing C compilers on any platform.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/FractalFir/crustc">crustc: entirety of `rustc`, translated to C - GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Bootstrapping_(compilers)">Bootstrapping (compilers)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Transpilation">Transpilation</a></li>

</ul>
</details>

**Discussion**: Commenters praised the dedication, noting the project is the 14th attempt and took three years. Some discussed using diverse double-compiling (DDC) to detect backdoors in the official compiler. Others compared the approach to LLVM's now-revived C backend, suggesting transpiling to C could be more portable.

**Tags**: `#rust`, `#compiler`, `#bootstrapping`, `#transpilation`

---

<a id="item-3"></a>
## [Linux 6.9 bug breaks LUKS suspend key wiping](https://mathstodon.xyz/@iblech/116769502749142438) ⭐️ 8.0/10

A bug introduced in Linux 6.9 caused the `cryptsetup luksSuspend` command to fail to wipe disk-encryption keys from kernel memory when suspending a LUKS device. This regression compromises the security model of disk encryption, potentially exposing encrypted data during suspend-to-RAM, as the master key remains in memory. The issue affects the `cryptsetup luksSuspend` operation, which is meant to block I/O and wipe the encryption key; however, in Linux 6.9 the key wiping step was skipped, leaving the key in kernel memory.

hackernews · IngoBlechschmid · Jul 2, 15:25 · [Discussion](https://news.ycombinator.com/item?id=48763035)

**Background**: LUKS (Linux Unified Key Setup) is a disk encryption specification. The `cryptsetup luksSuspend` command temporarily suspends a LUKS device, blocking all I/O and wiping the encryption key from kernel memory to protect data during sleep. The key must be re-entered upon resume. A failure to wipe the key leaves it vulnerable to cold boot attacks or other memory access.

<details><summary>References</summary>
<ul>
<li><a href="https://www.man7.org/linux//man-pages/man8/cryptsetup-luksSuspend.8.html">cryptsetup-luksSuspend (8) - Linux manual page - man7.org</a></li>
<li><a href="https://en.wikipedia.org/wiki/Linux_Unified_Key_Setup">Linux Unified Key Setup - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community comments expressed mixed opinions: some downplayed the severity, noting that `luksSuspend` is a Debian extension not officially supported, while others debated whether the bug was intentional, with some suspicion of a 'bugdoor'. The discussion also highlighted the value of NixOS tests in catching such regressions.

**Tags**: `#Linux`, `#security`, `#LUKS`, `#disk encryption`, `#kernel`

---

<a id="item-4"></a>
## [PeerTube: A Decentralized, Federated Open-Source Video Platform](https://github.com/Chocobozzz/PeerTube) ⭐️ 8.0/10

PeerTube is a free, decentralized, and federated video platform that uses ActivityPub to enable interoperability across instances, offering an alternative to centralized services like YouTube. It empowers users with greater control over content and privacy, reduces reliance on single corporate entities, and fosters a more resilient and censorship-resistant video ecosystem. The platform uses peer-to-peer technology (WebTorrent) to distribute video loads when videos become popular, and it is part of the Fediverse, allowing cross-platform interaction with other ActivityPub-compatible services.

hackernews · doener · Jul 2, 11:17 · [Discussion](https://news.ycombinator.com/item?id=48759634)

**Background**: Traditional video platforms like YouTube are centralized, meaning all content is hosted on servers controlled by a single company. In contrast, PeerTube is federated: anyone can run their own instance (server) that connects with others via the ActivityPub protocol, forming a network of independent yet interconnected communities. This decentralization enhances resilience and user autonomy.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/PeerTube">PeerTube - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community comments highlight major challenges: professional YouTubers note the lack of monetization makes it unsustainable for high-quality content production, while others point out the absence of popular content and audience. Some appreciate its use for open-source tutorials despite these limitations. Overall, the discussion reflects cautious optimism tempered by realistic concerns about adoption and business models.

**Tags**: `#decentralized video`, `#federated systems`, `#open source`, `#content creation`, `#YouTube alternative`

---

<a id="item-5"></a>
## [Podman v6.0.0 Released with Network Improvements and Quadlet Support](https://blog.podman.io/2026/07/introducing-podman-v6-0-0/) ⭐️ 8.0/10

Podman version 6.0.0 has been officially released, introducing significant network improvements, including default network isolation, and enhanced Quadlet support for declarative container management via systemd unit files. This major release strengthens Podman's position as a leading Docker alternative, offering improved security and Docker-compatible networking while eliminating the need for a central daemon, which simplifies container workflows for developers and DevOps teams. The Podman import path has changed to go.podman.io/podman/v6 as part of migrating to a CNCF-owned organization, and network isolation now defaults to enabled for better Docker compatibility and security.

hackernews · soheilpro · Jul 2, 14:23 · [Discussion](https://news.ycombinator.com/item?id=48762098)

**Background**: Podman is a daemonless, rootless container engine designed as a drop-in replacement for Docker, but it does not require a central daemon, which reduces resource usage and attack surface. Quadlet allows users to define containers, pods, volumes, and networks as systemd unit files, enabling declarative systemd-managed container lifecycles. This update continues Podman's goal of providing a secure, compatible container runtime with easier system integration.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/podman-container-tools/podman/releases">Releases · podman -container-tools/ podman</a></li>
<li><a href="https://docs.podman.io/en/latest/markdown/podman-quadlet.1.html">podman-quadlet — Podman documentation</a></li>
<li><a href="https://www.redhat.com/en/blog/quadlet-podman">Make systemd better for Podman with Quadlet - Enable Sysadmin</a></li>

</ul>
</details>

**Discussion**: Community members praised Podman's ease of migration and superior design compared to Docker, with one user noting that switching from Docker Desktop was seamless with docker-compose files. Others criticized limited distribution support for Ubuntu, which hinders adoption, while Quadlet received positive feedback for rootless container deployment on Rocky Linux.

**Tags**: `#podman`, `#containerization`, `#docker-alternative`, `#release`, `#devops`

---

<a id="item-6"></a>
## [How to Ask for Help from Strangers Effectively](https://pradyuprasad.com/writings/how-to-ask-for-help/) ⭐️ 8.0/10

A practical guide outlines strategies for soliciting help from strangers by demonstrating effort, proof of work, and genuine interest, rather than relying on generic requests. This matters because networking and seeking help are critical for career growth, yet many people fail due to poor communication; the article offers actionable advice to improve success rates. Key strategies include leading with proof of work, being specific about the ask, and showing you've already tried solving the problem yourself, which signals respect for the helper's time.

hackernews · FigurativeVoid · Jul 2, 13:19 · [Discussion](https://news.ycombinator.com/item?id=48761118)

**Background**: In professional networking, cold outreach is common but often ignored. People are more willing to help those who show genuine effort and preparation. The article reframes asking for help as a skill that can be learned.

**Discussion**: Commenters generally agree with the advice, adding personal anecdotes about the importance of proof of work and sincerity. Some debate whether offering to pay upfront or the depth of preparation matters more.

**Tags**: `#networking`, `#career-advice`, `#communication`, `#soft-skills`, `#hacker-news`

---

<a id="item-7"></a>
## [Immich 3.0 Released: Major Update to Self-Hosted Photo Platform](https://github.com/immich-app/immich/discussions/29439) ⭐️ 8.0/10

Immich 3.0, a major update to the self-hosted photo and video management platform, has been released, bringing new features and improvements as discussed in the community announcement. Immich is a popular open-source alternative to Google Photos and Apple Photos, and this major release signals continued development and community engagement, impacting users seeking privacy-focused media management. The release includes community-discussed features; however, some users express disappointment over the lack of end-to-end encryption (E2EE), which remains a desired feature for many self-hosting enthusiasts.

hackernews · hashier · Jul 2, 14:13 · [Discussion](https://news.ycombinator.com/item?id=48761944)

**Background**: Immich is a self-hosted photo and video backup solution that allows users to store and manage their media on their own servers, ensuring privacy and control. It offers features like automatic backup, search, and sharing, similar to cloud services but without third-party data access.

<details><summary>References</summary>
<ul>
<li><a href="https://immich.app/">Immich</a></li>

</ul>
</details>

**Discussion**: The community discussion shows mixed opinions: some users praise Immich as a no-brainer replacement for Apple/Google Photos, while others have switched to alternatives like Ente due to the lack of end-to-end encryption. Technical concerns about iOS sync reliability are also raised.

**Tags**: `#self-hosting`, `#photography`, `#open-source`, `#privacy`

---

<a id="item-8"></a>
## [Apple Helped FBI Unmask Anonymous iCloud Email User](https://t.me/zaihuapd/42302) ⭐️ 8.0/10

Apple provided the FBI with the real iCloud account details linked to an anonymous email address generated by its Hide My Email feature, used to send threatening messages to FBI Director Kash Patel's girlfriend. This case reveals that Apple's privacy-focused Hide My Email feature is not truly anonymous in law enforcement investigations, potentially eroding user trust in Apple's privacy promises and raising questions about the balance between privacy and security. The suspect, Alden Ruml, generated 134 anonymous email aliases via iCloud+ and later admitted to sending the threatening message. The affidavit states that Apple can trace each Hide My Email alias back to the originating iCloud account.

telegram · zaihuapd · Jul 2, 01:03

**Background**: Apple's Hide My Email feature, part of iCloud+, allows users to create unique, random email addresses that forward to their personal inbox, designed to protect privacy when signing up for services. However, Apple retains the mapping between the alias and the user's real account, which can be disclosed under lawful request. This feature is similar to the 'Sign in with Apple' privacy option.

<details><summary>References</summary>
<ul>
<li><a href="https://support.apple.com/zh-cn/guide/icloud/mm9d9012c9e8/icloud">在所有设备的 iCloud+ 中设置并使用隐藏邮件地址 - 官方 Apple 支持 (...</a></li>
<li><a href="https://support.apple.com/zh-cn/guide/icloud/mm1a876f7aed/icloud">在 iCloud.com 上创建和编辑“隐藏邮件地址” - 官方 Apple 支持 (中国)</a></li>
<li><a href="https://cybersecuritynews.com/apple-hide-my-email-vulnerability/">Apple ‘ Hide My Email ’ Vulnerability Exposes Users' Real Email ...</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#Apple`, `#law enforcement`, `#iCloud`, `#anonymity`

---

<a id="item-9"></a>
## [Meta Plans to Sell Excess AI Compute, Enters Cloud Market](https://www.bloomberg.com/news/articles/2026-07-02/south-korean-stocks-tumble-6-as-ai-jitters-hurt-chipmakers) ⭐️ 8.0/10

Meta is planning to sell excess AI computing power and model services to external customers, signaling a move into the cloud computing market. This news, combined with Apple's potential shift to Chinese memory suppliers, caused a sharp drop in South Korean stocks. This strategic shift indicates that Meta may be overinvesting in AI infrastructure, leading to market concerns about oversupply and potential slowdown in AI spending. It could disrupt existing cloud providers like AWS and Azure, and reshape the competitive landscape. The announcement triggered a sell-off in South Korean stocks, with the Kospi index falling up to 7%, and Samsung Electronics and SK Hynix each dropping at least 8%. The Korean exchange temporarily halted programmatic selling of Kospi futures.

telegram · zaihuapd · Jul 2, 02:29

**Background**: AI computing power, or compute, refers to the hardware and software resources needed to train and run large AI models, typically using GPUs. Major tech companies like Meta have been investing heavily in AI infrastructure, leading to concerns about a potential bubble. Cloud computing providers like Amazon Web Services and Microsoft Azure offer compute services to external customers.

**Tags**: `#Meta`, `#AI computing`, `#cloud computing`, `#market impact`, `#tech industry`

---

<a id="item-10"></a>
## [Cloudflare to Block Mixed-Purpose AI Crawlers from September, Calls Out Google](https://techcrunch.com/2026/07/01/cloudflares-new-policy-pushes-ai-companies-to-pay-for-publishers-content/) ⭐️ 8.0/10

Cloudflare announced that from September 15, 2026, it will block mixed-purpose AI crawlers from ad-supported webpages by default, and singled out Google for exploiting the loophole where sites block AI crawlers but allow Googlebot for search. This policy shift marks a significant change in content access economics, potentially forcing AI companies to pay for content and reshaping how publishers monetize their data in the AI era. The default block applies to new Cloudflare customers and free-tier users, targeting crawlers that combine search indexing with AI training. Cloudflare also introduced a 'Pay Per Use' model with initial partners Ceramic.ai and You.com to monetize content consumption by AI.

telegram · zaihuapd · Jul 2, 05:37

**Background**: Mixed-purpose crawlers are bots that simultaneously perform traditional search indexing and AI model training, making it difficult for website owners to allow search while blocking AI use. Cloudflare had previously offered a one-click block for AI crawlers in 2024, and the new default setting extends that protection automatically to all new domains. This addresses a growing concern among publishers that their content is being used to train AI without compensation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.techtimes.com/articles/319554/20260702/cloudflare-separates-ai-crawlers-purpose-opens-door-charging-them-directly.htm">Cloudflare Separates AI Crawlers by Purpose and Opens Door to Charging ...</a></li>
<li><a href="https://digitalmarketreports.com/news/73839/cloudflare-to-block-mixed-use-ai-crawlers-on-ad-supported-pages/">Cloudflare to Block Mixed-Use AI Crawlers on Ad-Supported ...</a></li>
<li><a href="https://www.cloudflare.com/en-ca/press/press-releases/2025/cloudflare-just-changed-how-ai-crawlers-scrape-the-internet-at-large/">Cloudflare Just Changed How AI Crawlers Scrape the... | Cloudflare</a></li>

</ul>
</details>

**Tags**: `#Cloudflare`, `#AI`, `#web scraping`, `#Google`, `#content policy`

---

<a id="item-11"></a>
## [OpenAI Proposes US Government Take 5% Stake, Including Google & Meta](https://www.bloomberg.com/news/articles/2026-07-02/openai-proposes-giving-the-us-government-a-5-stake-ft-says) ⭐️ 8.0/10

OpenAI has proposed that the US government take a 5% equity stake in itself and potentially other major AI companies such as Google and Meta, according to a report. This proposal could reshape AI governance by giving the public a direct share in AI-driven economic gains, but it raises concerns about regulatory control and conflicts of interest among competing firms. CEO Sam Altman and other executives suggested a single government vehicle would hold 5% stakes in OpenAI, Anthropic, Google, and Meta. It remains unclear whether the other companies will accept this arrangement.

telegram · zaihuapd · Jul 2, 06:02

**Background**: OpenAI originally started as a non-profit but later created a capped-profit entity to attract investment. The US government has been increasing its focus on regulating AI, and this proposal would give the public a stake in the AI boom's financial benefits.

**Tags**: `#OpenAI`, `#AI governance`, `#US government`, `#tech policy`

---

<a id="item-12"></a>
## [Major Companies Restrict Employee AI Use Over Soaring Costs](https://www.404media.co/companies-are-throttling-employees-ai-use-because-its-too-expensive/) ⭐️ 8.0/10

Reports indicate that companies including Citi, Atlassian, Adobe, Amazon, and Accenture are restricting employee access to advanced AI models like GPT-5.5 and Claude Opus, citing skyrocketing costs from consumption-based pricing. For example, Atlassian's monthly AI spending jumped from $5 million in August 2025 to over $15 million by May 2026. This trend reveals a critical financial challenge in enterprise AI adoption: the unsustainability of consumption-based pricing when powerful models are widely used. It may force organizations to rethink AI deployment strategies, potentially slowing innovation or shifting toward more cost-efficient models. Citi fully disabled GPT-5.5 and Claude Opus on June 24 due to excessive AI credit consumption, while Atlassian terminated unlimited usage and introduced cost-tracking dashboards. Similarly, Adobe ended its unlimited Claude contract, and Amazon employees discovered previously unknown token usage caps after a leaderboard was shut down.

telegram · zaihuapd · Jul 2, 13:59

**Background**: Many AI platforms, including OpenAI and Anthropic, charge based on token consumption or 'AI credits,' similar to a metered utility. This consumption-based pricing can lead to unpredictable costs, especially when employees freely access high-end models. Companies are now implementing controls such as usage caps and cost dashboards to manage expenses.

<details><summary>References</summary>
<ul>
<li><a href="https://tokenmix.ai/blog/github-copilot-ai-credits-billing-2026">GitHub Copilot AI Credits 2026: Prices, Limits, Cost Math</a></li>
<li><a href="https://support.microsoft.com/en-us/Microsoft-365-Copilot/ai-credits-and-limits-for-microsoft-365-subscriptions">AI credits and limits for Microsoft 365 subscriptions</a></li>
<li><a href="https://www.ibbaka.com/ibbaka-market-blog/the-evolution-of-ai-pricing-models-from-consumption-to-hybrid-and-generative-approaches">The Evolution of AI Pricing Models: From Consumption to Hybrid and...</a></li>

</ul>
</details>

**Tags**: `#AI cost`, `#enterprise AI`, `#usage restrictions`, `#generative AI`, `#business impact`

---

<a id="item-13"></a>
## [Anthropic in Talks with Samsung for Custom AI Chip Manufacturing](https://www.theinformation.com/articles/anthropic-talks-samsung-manufacture-custom-ai-chip) ⭐️ 8.0/10

Anthropic has begun developing its own AI chip and is in talks with Samsung Electronics for potential manufacturing collaboration, aiming to strengthen control over the computing infrastructure behind its Claude model. This move signals a trend toward vertical integration in AI, where major AI companies seek to reduce dependence on external chip suppliers like Nvidia and optimize hardware-software co-design. If successful, it could give Anthropic a competitive edge in performance and cost for its AI services. The project is still in early stages, and Anthropic is entering the custom chip arena later than competitors like OpenAI and Google. Specific chip architecture or timeline details have not been disclosed.

telegram · zaihuapd · Jul 2, 15:57

**Background**: AI chips are specialized processors designed to accelerate machine learning workloads, such as training and inference of large language models. Currently, companies like Nvidia dominate the market with GPUs, but many tech giants are designing their own chips to improve efficiency and reduce costs. Anthropic's effort mirrors similar initiatives by OpenAI and other AI labs.

**Tags**: `#AI芯片`, `#Anthropic`, `#三星`, `#自研硬件`

---