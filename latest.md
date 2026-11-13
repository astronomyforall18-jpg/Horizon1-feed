# Horizon Daily - 2026-11-13

> From 7 items, 3 important content pieces were selected

---

**Technology News**
1. [Engineers Scale 1-Trillion Parameter MoE Model to 384 GH200 GPUs Using TorchTitan](#item-tech-news-1) ⭐️ 8.0/10
2. [Four Frontier AI Models Nearly Ace 7-Part Materials Science Research Test](#item-tech-news-2) ⭐️ 8.0/10
3. [Reverse Engineering a Coway Air Purifier to Remove Cloud Dependency](#item-tech-news-3) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Engineers Scale 1-Trillion Parameter MoE Model to 384 GH200 GPUs Using TorchTitan](https://www.reddit.com/r/MachineLearning/comments/1xvce5h/scaling_to_1t_moe_on_torchtitan_p/) ⭐️ 8.0/10

Engineers scaling a 1-trillion parameter Mixture of Experts model across 384 GH200 GPUs on the JUPITER supercomputer achieved a performance of approximately 1,300 tokens per second per GPU using TorchTitan. The training setup combined 384-way Fully Sharded Data Parallel \(FSDP\) and 4-way Expert Parallelism \(EP\), avoiding Pipeline Parallelism to reduce iteration delays. Optimizations included full activation checkpointing, Grace CPU offloading via the C2C link, custom Newton-Schulz execution on GPUs, workload bucketing, and modified gradient communication strategies.

reddit · r/MachineLearning · /u/f14-bertolotti · Nov 13, 16:28

**「Background」** Large-scale distributed training of frontier-scale models often encounters hardware bottlenecks, particularly around inter-node network bandwidth and GPU memory management. On the JUPITER supercomputer, InfiniBand provides limited bandwidth compared to local NVLink and Grace-Hopper links, requiring careful communication reduction and memory optimization techniques to maintain training efficiency.

**「Impact」** The engineering team increased training throughput by 14 times compared to their starting baseline, demonstrating that publicly funded Hopper-generation clusters can execute frontier-scale distributed training when network bandwidth and memory allocator constraints are properly addressed.

**Tags**: `#Machine Learning`, `#Distributed Training`, `#PyTorch`, `#Hardware Acceleration`

---

<a id="item-tech-news-2"></a>
### [Four Frontier AI Models Nearly Ace 7-Part Materials Science Research Test](https://www.reddit.com/r/MachineLearning/comments/1xvgf6h/four_frontier_models_scored_978100_on_a_7part/) ⭐️ 8.0/10

A materials-science researcher developed a seven-part technical evaluation measuring everyday research tasks, which four frontier AI models scored between 97.8 and 100 on. Tested models included Gemini 4 Carbon, Gemini 4 Hydrogen, Claude Opus 5.5, and Claude Fable 5.2, each completing the test across three fresh runs in 7 to 24 minutes with web search and code execution enabled. The author noted that minor point losses stemmed solely from formatting trivia, while the models successfully handled messy dataset reductions, crystal structure density functions, physics calculations, manuscript critiques with planted errors, and refutations of false premises. The creator plans to develop longer-horizon, multi-hour simulated lab campaign benchmarks to better assess open-ended research workflows.

reddit · r/MachineLearning · /u/v\_aravind · Nov 13, 18:58

**「Background」** The author, a researcher working in graphene and 2D materials, designed the test using synthetic data and code-computed answer keys to reflect realistic tasks in a research group. The evaluation methodology aligns with existing benchmarks like FrontierScience, METR time horizons, and PaperBench, highlighting a trend where bounded tasks with known procedures become saturated by frontier models.

**Tags**: `#AI Benchmarks`, `#Materials Science`, `#Large Language Models`, `#Model Evaluation`

---

<a id="item-tech-news-3"></a>
### [Reverse Engineering a Coway Air Purifier to Remove Cloud Dependency](https://scottjg.com/posts/2026-11-11-reverse-engineering-my-coway-air-purifier-to-ditch-the-cloud/) ⭐️ 7.0/10

An engineer successfully reverse-engineered their Coway air purifier to eliminate cloud reliance and achieve local control. The project highlights a growing trend of liberating IoT devices from mandatory cloud services. Affected users are smart home enthusiasts seeking local hardware management.

hackernews · scottjg · Nov 12, 22:03 · [Discussion](https://news.ycombinator.com/item?id=50474959)

**「Background」** Many modern consumer IoT devices rely on external cloud infrastructure for core functionality and mobile app control, restricting users to vendor-managed ecosystems.

**「Impact」** Users can regain local control over their Coway air purifiers, bypassing cloud dependencies and maintaining functionality without external server connections.

**「Community Discussion」** Commenters noted that many consumer devices contain glaring security flaws, such as downloading root CA certificates over plain HTTP, making them vulnerable to man-in-the-middle attacks. Several users observed that Large Language Models are increasingly accelerating these reverse-engineering efforts by helping handle tedious tasks.

**Tags**: `#reverse engineering`, `#IoT`, `#smart home`, `#open source`

---

