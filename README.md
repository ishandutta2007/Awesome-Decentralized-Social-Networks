# Awesome-Decentralized-Social-Networks

## Top Decentralized Social Networks Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Federated Protocols, Community Moderation & Link Aggregation*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Decentralized Social Networks**. These tools enable communities to own their social graph and content—from federated link aggregators where independent servers sync with each other to self-hosted forums that give administrators complete control over moderation and data.



**Examples** include Lemmy, Mastodon, Discourse, Flarum, NodeBB, Friendica, PieFed, Mbin, Hubzilla, and GoToSocial (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, federated communication, and open community infrastructure—ideal for community managers, privacy advocates, and organizations seeking transparent, vendor-independent social platforms.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



### Sector Overview & Market Dynamics

The global dedicated online community and enterprise social network platform market is estimated at approximately $1.5B to $2.2B (expected to surpass $5B+ by the early 2030s), while the broader social networking ecosystem exceeds $150B+. The sector exhibits a bifurcated market structure: the consumer social layer is concentrated and dominated by winner-take-most ad platforms, whereas the community and discussion software SaaS space is moderately-to-highly fragmented across creator niches, developer forums, and enterprise customer-success hubs.

## SaaS/Hosted Platforms

| Product | Company Size (Valuation / Revenue) | Starting Tier Pricing | Free Tier / Trial Limits | Description |
| :--- | :--- | :--- | :--- | :--- |
| **Reddit** | ~$30B–$35B market cap ($2.2B FY2025 revenue) | $0 (Ad-supported user model); Reddit Premium starts at $5.99/mo | Free forever plan with full access to browse, post, and create communities (ad-supported; API subject to standard free tier rate limits: 100 queries/min) | The centralized link aggregator standard. Fully proprietary and cloud-hosted. **No federation, no self-hosting**—the platform operator controls moderation policy, API access, and data. Best for communities that prioritize network effects and reach over sovereignty. |
| **Khoros Communities** | ~$250M–$284M annual revenue (Acquired by IgniteTech, private) | Starts at ~$50,000/year (~$4,166/mo entry mid-market/enterprise contract) | No free tier or public self-serve trial (requires a scheduled sales-assisted demo) | Enterprise community platform. Fully proprietary and cloud-hosted. **No federation or self-hosting**—best for large enterprises needing integrated social customer care. |
| **Circle.so** | ~$55M–$68M ARR ($33M+ funding, private) | $89/mo (billed annually) or $99/mo (billed monthly) on Professional Plan | 14-day free trial on Professional and Business plans (full feature access, up to 3 admins and 10 moderators; no credit card required) | Centralized community platform for creators and businesses. Fully proprietary and cloud-hosted. **No federation or self-hosting**—best for creators wanting a polished, managed community experience. |
| **Discourse (Hosted)** | ~$10M–$15M ARR (Private) | $0/mo (Free Managed Plan); Paid managed plans start at $100/mo (Standard) | Free forever managed plan hosted on `.discourse.group` subdomain (limited to 2 staff seats, 5GB storage, 20,000 monthly emails, and community plugin set) | **Official managed hosting** for Discourse forums. Features **business-class hosting** with automatic updates and support. **Note**: The software itself is open source (GPL v2)—hosting is a convenience service. **Best for**: teams wanting Discourse's features without server management. |
| **Mighty Networks** | ~$8M–$10M annual revenue (~$100M–$250M valuation, private) | $79/mo (billed annually) or $95/mo (billed monthly) on Launch Plan ($29/mo on Explore Plan) | 14-day free trial with full Growth Plan features (unlimited members, events, spaces, and course creation testing; no credit card required) | Centralized community and course platform. Fully proprietary and cloud-hosted. **No federation or self-hosting**—best for creators combining community with paid content. |



## Open-Source GitHub Projects



- **Lemmy**  

  **A link aggregator and forum for the fediverse** (AGPL-3.0) — **the Reddit alternative** . **Server is written in Rust** for high performance; **front end is ~80kB gzipped**; **supports arm64 / Raspberry Pi** . **Federated architecture**: anyone can run a server, and **all servers are federated (think email)**—a user on one server can subscribe to forums on any other server and discuss with users registered elsewhere . **Features**: **live-updating comment threads**, **full vote scores (+/-) like old Reddit**, **themes (light, dark, solarized)**, **integrated image uploading**, **user tagging with @ and community tagging with !**, **notifications on replies and tags**, **private messaging**, **RSS/Atom feeds**, **cross-posting with similar post search**, and **moderation abilities** (public logs, sticky posts, lock/remove/restore, ban/unban, transfer communities) . **Can fully erase your data**, replacing all posts and comments . **Deployment**: Docker and Ansible . **The reference implementation for federated link aggregation** — **the dominant "Threadiverse" platform** with 423 servers and roughly 43,000 MAU, ahead of Misskey and Pleroma .



- **Mastodon**  

  **Your self-hosted, globally interconnected microblogging community** (AGPLv3) — **the flagship fediverse platform** . **Based on ActivityPub** with no vendor lock-in—users on one server can seamlessly communicate with users on another, including non-Mastodon software that implements ActivityPub . **Features**: **real-time chronological timelines**, **media attachments**, **safety and moderation tools** (private posts, locked accounts, phrase filtering, muting, blocking, reporting), **OAuth2 and REST/Streaming APIs** for a rich app ecosystem . **Mastodon 4.6** (June 2026) adds **email newsletters** (reaching readers without a fediverse account—deliberately off by default due to server costs), **Collections** (shareable lists of up to 25 profiles, with opt-in requirements and abuse prevention), **redesigned profiles** with in-place editing and alt text for profile pictures/headers, and **accessibility improvements** sponsored in part by the Dutch government . **The largest fediverse platform** with roughly **735,000 MAU**—still a fraction of centralized alternatives . **Best for**: organizations and individuals wanting **microblogging with federation** and a proven moderation model.



- **Discourse**  

  **A platform for community discussion. Free, open, simple** (GPL v2) — **the forum standard** . **Battle-tested for over a decade** with a **flattened discussion** model (no threading pain), **self-learning moderation**, and **seamless web-only interface** . **Tech stack**: **Ruby on Rails** API, **Ember.js** front end, **PostgreSQL**, **Redis** . **Recent additions**: **built-in MCP server** (disabled by default) letting AI apps search, read, summarize, and write to your community after user approval; **Ask AI dashboard** showing what users are asking and tracking unanswered questions . **Rich text editor** now edits dates, polls, tables, and graphviz diagrams without switching to Markdown . **Requirements**: **Ruby 3.2+, PostgreSQL 13, Redis 7** — **resource-heavy (~1–2 GB RAM)** compared to lighter alternatives . **The reference implementation for long-form community discussion**.



- **Flarum**  

  **Simple forum software for building great communities** (MIT) — **the lightweight modern choice** . **Fast and simple**—no clutter, no bloat, no complex dependencies; **built with PHP** and powered by **Mithril.js** for a tiny frontend footprint . **Beautiful and responsive**—consistent and intuitive across platforms out-of-the-box. **Powerful and extensible**—**1,600+ community extensions** covering tags, mentions, SSO, OAuth, file uploads, SEO, analytics, and more; **JSON:API compliant REST API** for custom integrations . **Flarum 2.0.0** released October 2026 . **Resource footprint**: **~256 MB RAM**—**significantly lighter than Discourse** . **Best for**: teams wanting **a fast, clean forum with minimal resource requirements** and a rich extension ecosystem.



- **NodeBB**  

  **Node.js based forum software built for the modern web** (GPL-3) — **the real-time choice** . **Powered by Node.js**, supports **Redis, MongoDB, or PostgreSQL**; utilizes **web sockets for instant interactions and real-time notifications** . **Takes the best of the modern web**: **real-time streaming discussions**, **mobile responsiveness**, and **rich RESTful read/write APIs**—while staying true to bulletin board hierarchies, local user accounts, and asynchronous messaging . **Theming engine** is highly flexible; base theme uses **Bootstrap 5** . **ActivityPub federation support** via plugins—v4.15.0 added **fediverse chat privileges** and **opportunistic backfilling** of remote topics . **Requirements**: **Node.js 22+, MongoDB 5+ or Redis 7.2+** . **The reference implementation for real-time forum software**.



- **Friendica**  

  **Your open and free social network** (AGPLv3) — **the multi-protocol bridge** . **Connects to a federated communications network of thousands of servers called the Fediverse**—you can interact with anyone on Friendica, **Mastodon, Lemmy, Diaspora, Misskey, Peertube, Pixelfed, Pleroma**, and many more . **Receiving content from Tumblr, WordPress, and RSS is also possible** . **The oldest active federated social network** (running since 2010)—**six years before Mastodon** . **Protocol breadth is the core goal**: ActivityPub, Diaspora, DFRN, OStatus, email via IMAP/SMTP, RSS/Atom, and plugins for Bluesky and WordPress . **UX is closer to a classic social network** (rich BBCode editor, circle-based contact management, events with RSVPs, granular per-post privacy) than a microblog stream . **Runs on PHP and MySQL**—**if you can run WordPress, you can run Friendica** . **The "federation world champion"** —actively maintained but largely absent from fediverse growth conversations .



- **PieFed**  

  **A growing Lemmy alternative** with **76 servers and around 4,800 MAU** . **Part of the Threadiverse**—link aggregation and threaded discussion on ActivityPub. **Best for**: communities wanting a Lemmy-compatible alternative with different moderation or UX choices.



- **Mbin**  

  **A Threadiverse platform** with **around 1,300 MAU** . **Federates via ActivityPub**—Mastodon users can follow Mbin communities. **Best for**: smaller communities exploring the link aggregation model.



- **Hubzilla**  

  **Created by Mike Macgirvin** (the developer behind DFRN, the protocol Friendica used before ActivityPub) — **the nomadic identity choice** . **Speaks ActivityPub and its own Zot (now Nomad) protocol simultaneously** . **Nomadic identity**: your account can be **cloned across multiple hubs**—if one hub goes offline, your identity, social graph, and content survive intact on the others . **Goes well beyond what ActivityPub's built-in account migration supports**—closer to true portable identity than anything else in the fediverse. **The trade-off**: **considerably harder to set up and administer** than Friendica; **~1,450 MAU** reflects a specialist audience . **Best for**: power users who prioritize **portable identity and protocol flexibility** over ease of deployment.



- **GoToSocial**  

  **Exists for people who want a personal fediverse presence but find Mastodon too resource-heavy to self-host** . **Currently in beta** with a **v1.0 release projected for 2026** . **Best for**: individuals wanting a **lightweight personal fediverse server**.



### Additional Strong Open-Source Options



- **Discourse AI** — Official AI plugin for Discourse (GPL v2) . **Adds AI-powered search, summaries, and chatbot functionality** to self-hosted Discourse forums .

- **NodeBB ActivityPub** — Federation plugin for NodeBB (GPL-3) . **Bridges NodeBB forums to the fediverse**—Mastodon users can follow and interact with NodeBB content .

- **Lemmy UI** — Frontend for Lemmy (AGPL-3.0) . **The ~80kB gzipped frontend**—clean, mobile-friendly interface .

- Community **n8n** workflows for fediverse cross-posting automation and community moderation alerting.



**Frameworks for building custom systems**: Combine **Lemmy** for federated link aggregation with **Mastodon** for microblogging, **Discourse** or **Flarum** for long-form discussion, **Friendica** for multi-protocol bridging, and **Hubzilla** for nomadic identity—creating a comprehensive decentralized social stack.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Decentralized social networks handling user content and social graphs must be evaluated for **moderation effectiveness**, **federation metadata leakage**, and **long-term project viability**.

- **The "Reddit alternative" distinction matters.** **Lemmy** is the dominant federated link aggregator—**423 servers and ~43,000 MAU**—with Reddit-like voting, cross-posting, and moderation . **But the interaction model (communities as primary unit, upvotes rather than boosts) is different enough that the Threadiverse and microblog social graphs rarely overlap** . **Choose based on whether you want discussions or broadcasts.**

- **The "forum software" distinction is about depth vs. lightness.** **Discourse** is battle-tested for a decade with flattened discussion and self-learning moderation—**but requires 1–2 GB RAM and a complex Rails/Ember stack** . **Flarum** is **~256 MB RAM** with 1,600+ extensions—**significantly lighter and simpler** . **NodeBB** brings **real-time web sockets and REST APIs** to the forum model . **Match the tool to your operational capacity and community size.**

- **Friendica's protocol breadth is unique and underappreciated.** It **connects to Mastodon, Lemmy, Diaspora, Misskey, Peertube, Pixelfed, Pleroma**, and more—**plus email, RSS, Tumblr, WordPress, and Bluesky via plugins** . **It's the "federation world champion"** that the growth conversations ignore . **If you want one timeline spanning multiple networks, Friendica is the only serious option.**

- **Hubzilla's nomadic identity is genuinely novel.** **Clone your account across multiple hubs**—if one goes offline, your identity, social graph, and content survive . **This is closer to true portable identity than anything else in the fediverse.** **But the complexity is real**—Hubzilla is harder to set up than Friendica, and its ~1,450 MAU reflects a specialist audience .

- **Mastodon's email newsletters are a strategic bet on growth.** **Reaching readers without a fediverse account**—just an inbox—**lowers the barrier to following a creator** . **But it's off by default** due to server costs, and **it doesn't solve the network effects problem** that keeps Mastodon at ~735,000 MAU . **The feature extends the institutional hosting bet**—giving organizations a reason to choose Mastodon over other publishing platforms.

- Self-hosted open-source solutions require proper server management, moderation policy, and ongoing maintenance. **Decentralized does not mean zero-maintenance**—it means you own the moderation, the upgrades, and the backups.



---



**Made for community managers, privacy advocates, and organizations building transparent decentralized social solutions.**  

Let's make Decentralized Social Networks more open, data-driven, and federated.
