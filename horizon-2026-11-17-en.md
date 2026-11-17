# Horizon Daily - 2026-11-17

> From 13 items, 6 important content pieces were selected

---

**Technology News**
1. [vLLM v0.34.0 Released with Extensible KV Cache and Model Runner V2](#item-tech-news-1) ⭐️ 8.0/10
2. [Phrack Magazine Releases Issue 73](#item-tech-news-2) ⭐️ 8.0/10
3. [Microsoft Introduces MAI Code 2 and Code 2 Flash Models](#item-tech-news-3) ⭐️ 8.0/10
4. [Nvidia Stops Disclosing Singapore Sales as Subsidiary Revenues Reach $104 Billion](#item-tech-news-4) ⭐️ 7.0/10
5. [Highly Classified US National Security Communications Network Experiences Outage](#item-tech-news-5) ⭐️ 7.0/10
6. [Simon Willison Releases Complete Rewrite of Datasette Lite Using Service Workers and Pyodide](#item-tech-news-6) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [vLLM v0.34.0 Released with Extensible KV Cache and Model Runner V2](https://github.com/vllm-project/vllm/releases/tag/v0.34.0) ⭐️ 8.0/10

vLLM version 0.34.0 introduces 10 new model integrations, activates the extensible KV cache by default, and completely removes Model Runner V1 in favor of Model Runner V2. The release brings performance speedups on hardware such as Blackwell and MI355X, alongside breaking changes including a default block size of 64, dropped ROCm 7.2 support, and a requirement for huggingface\_hub &gt;= 2.0.0.

github · khluu · Nov 16, 23:22

**「Background」** vLLM is an open-source large language model inference and serving engine designed for high throughput and memory efficiency. Prior versions maintained legacy support for Model Runner V1 and used fixed KV cache memory sizing estimates calculated before warmup.

**「Impact」** Users upgrading to v0.34.0 must remove legacy configurations such as VLLM\_USE\_V2\_MODEL\_RUNNER=0, adapt to a default block size of 64, and update dependencies including huggingface\_hub, as existing setups relying on deprecated flags or older ROCm artifacts will fail at startup.

**Tags**: `#vllm`, `#llm inference`, `#machine learning`, `#open source`

---

<a id="item-tech-news-2"></a>
### [Phrack Magazine Releases Issue 73](https://phrack.org/issues/73/introduction_md) ⭐️ 8.0/10

The 73rd issue of the iconic hacker magazine Phrack has been officially released. This publication continues the long-standing tradition of the digital zine, focusing on computer security, hacker culture, and software engineering.

hackernews · notmine1337 · Nov 17, 18:31 · [Discussion](https://news.ycombinator.com/item?id=50535992)

**「Background」** Phrack is a legendary computer hacker magazine founded in 1985 that has historically published influential technical articles and research within the security and underground programming communities.

**「Community Discussion」** Commenters expressed nostalgia and enthusiasm for the ongoing publication of the magazine, reminiscing about classic past issues like issue 49 and highlighting the value of documenting historical hacker lore.

**Tags**: `#Computer Security`, `#Hacker Culture`, `#Open Source History`

---

<a id="item-tech-news-3"></a>
### [Microsoft Introduces MAI Code 2 and Code 2 Flash Models](https://microsoft.ai/news/introducing-mai-code-2-and-mai-code-2-flash/) ⭐️ 8.0/10

Microsoft introduced the MAI Code 2 and Code 2 Flash models, expanding its offerings in the AI code generation space. The release highlights the accelerating development pace of specialized coding models within the industry. No additional technical specifications, pricing details, or availability dates were provided in the announcement.

hackernews · lemonish97 · Nov 17, 18:25 · [Discussion](https://news.ycombinator.com/item?id=50535885)

**「Background」** The introduction follows earlier Microsoft AI research releases, such as the MAI-Thinking-1 model, which provided in-depth technical documentation. Major technology companies continue to develop and deploy specialized large language models targeted at software engineering and developer workflows.

**「Community Discussion」** Hacker News commenters debated the sustainability of competitive leads among frontier AI labs and questioned the methods used to rapidly close performance gaps. Some users reported canceling existing developer subscriptions like GitHub Copilot in favor of newer, more cost-effective alternatives, while others emphasized the ongoing value of detailed technical reports from AI research teams.

**Tags**: `#artificial intelligence`, `#code generation`, `#large language models`, `#microsoft`

---

<a id="item-tech-news-4"></a>
### [Nvidia Stops Disclosing Singapore Sales as Subsidiary Revenues Reach $104 Billion](https://www.ft.com/content/dbde7a30-548c-4f9d-a4be-7898a0c24dcf) ⭐️ 7.0/10

Nvidia has ceased disclosing the scale of its business in Singapore after revenues for its Singaporean subsidiary reached $104 billion. The reporting change follows a period when the city-state accounted for a substantial portion of the company's worldwide revenues, driven by regional supply chain routing through original equipment manufacturers, original design manufacturers, and resellers. Nvidia altered its SEC filings after July 2025, switching its geographic revenue breakdown from customer billing locations to customer headquarters.

hackernews · louiereederson · Nov 17, 17:12 · [Discussion](https://news.ycombinator.com/item?id=50534631)

**「Background」** Singapore serves as a major regional hub where massive volumes of graphics processing units and semiconductor orders are routed before reaching end destinations globally. Industry observers note that the city-state does not possess the physical datacenter infrastructure or electrical capacity required to consume such large volumes of hardware locally.

**「Community Discussion」** Community members discussed the mechanics of Nvidia's financial reporting, noting that end customers typically purchase chips through a network of intermediaries rather than directly from Nvidia. Commenters debated the implications of routing large volumes of chips through Singaporean entities and pointed out that SEC filing adjustments effectively removed Singapore as a distinct line item by shifting from billing locations to customer headquarters.

**Tags**: `#Nvidia`, `#Artificial Intelligence`, `#Supply Chain`, `#Semiconductors`

---

<a id="item-tech-news-5"></a>
### [Highly Classified US National Security Communications Network Experiences Outage](https://www.cnn.com/2026/11/17/politics/highly-classified-national-security-communications-network-goes-down) ⭐️ 7.0/10

A highly classified US national security communications network suffered an unexpected outage, drawing public attention and prompting speculation regarding its cause. Specific technical details concerning the failure and its restoration timeline remain undisclosed.

hackernews · monkeydust · Nov 17, 15:38 · [Discussion](https://news.ycombinator.com/item?id=50532849)

**「Background」** The incident involves critical government infrastructure utilized for classified national security communications, raising questions among observers regarding public disclosure protocols for internal agency systems.

**「Community Discussion」** Commenters debated whether recent high-profile service outages reflect a broader increase in failure rates or heightened reporting visibility, while others discussed potential factors including broader tech industry downsizing and the role of AI-assisted exploits.

**Tags**: `#infrastructure outage`, `#national security`, `#cybersecurity`, `#government systems`

---

<a id="item-tech-news-6"></a>
### [Simon Willison Releases Complete Rewrite of Datasette Lite Using Service Workers and Pyodide](https://simonwillison.net/2026/Nov/17/datasette-lite/) ⭐️ 7.0/10

Simon Willison has released a complete rewrite of Datasette Lite, utilizing service workers and Pyodide to run the full server-side Datasette Python application directly in the browser via WebAssembly. The updated tool allows users to load specific PyPI releases, GitHub references, and SQLite versions, as well as install plugins directly via URL parameters. This release resolves prior limitations where injected HTML from a web worker prevented client-side JavaScript execution.

rss · Simon Willison · Nov 17, 16:48

**「Background」** Datasette Lite was originally launched in May 2022 as a port of the Datasette Python application to the browser using WebAssembly and Pyodide. The initial implementation relied on a web worker hack that simulated requests and injected the resulting HTML into the page using innerHTML, which broke features depending on client-side JavaScript execution.

**「Impact」** Developers can now create fully functional, URL-addressable demos of work-in-progress features, bug reproductions, and plugins using client-side SQLite databases and custom metadata files, eliminating the need to spin up a dedicated web server.

**Tags**: `#WebAssembly`, `#Python`, `#Datasette`, `#Pyodide`, `#Browser Architecture`

---

