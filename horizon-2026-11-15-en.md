# Horizon Daily - 2026-11-15

> From 8 items, 3 important content pieces were selected

---

**Technology News**
1. [SpaceX Successfully Catches Starship Upper Stage During Flight 15](#item-tech-news-1) ⭐️ 8.0/10
2. [Meta FAIR and NYU Researchers Train 200+ MLLMs to Unbundle Vision Encoding](#item-tech-news-2) ⭐️ 8.0/10
3. [Developer Creates Open-Source Tool to Accelerate cudaMemcpy Pageable Transfers 5x on B300](#item-tech-news-3) ⭐️ 8.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [SpaceX Successfully Catches Starship Upper Stage During Flight 15](https://www.spacex.com/launches/starship-flight-15) ⭐️ 8.0/10

SpaceX successfully caught the Starship upper stage during Flight 15, marking a major milestone for fully reusable rocket systems. The test flight demonstrated the first catch of a reusable upper stage since the space shuttle era. The event was documented via official company video and launch communications.

hackernews · ls612 · Nov 14, 21:22 · [Discussion](https://news.ycombinator.com/item?id=50500963)

**「Background」** Starship is SpaceX's next-generation heavy-lift launch system designed for full reusability of both booster and upper stage components. Previous development flights focused on iterative testing of launch, controlled descent, and landing maneuvers.

**「Impact」** Demonstrating a reusable upper stage paves the way for reduced payload delivery costs and increased launch cadences once operational reflight procedures are established.

**「Community Discussion」** Community members praised the engineering achievement as a historic milestone, noting it is the first reusable upper stage demonstration since the Space Shuttle. Commenters highlighted that success depends on heat shield durability and future capabilities like catching boosters and reflying hardware.

**Tags**: `#SpaceX`, `#Starship`, `#Aerospace Engineering`, `#Reusable Rockets`

---

<a id="item-tech-news-2"></a>
### [Meta FAIR and NYU Researchers Train 200+ MLLMs to Unbundle Vision Encoding](https://www.reddit.com/r/MachineLearning/comments/1xx1k2o/meta_fair_nyu_unbundling_multimodal_vision/) ⭐️ 8.0/10

A joint research effort by Meta FAIR and NYU trained over 200 multimodal large language models from scratch to evaluate different vision encoding strategies. The study found that separate encoder pretraining is optional, whereas vision-only parameters are essential for multimodal performance. Additionally, placing vision processing before the LLM is optional, as an "in-fusion" approach that adds zero-initialized vision-only weights to the LLM's first 8 layers performs on par with separate encoders. The experiments utilized Qwen3-1.7B and 4B configurations tested across 16 VQA benchmarks and 12 language benchmarks.

reddit · r/MachineLearning · /u/trungh98 · Nov 15, 17:38

**「Background」** Published multimodal models have diverged on vision encoder strategies, with models like Gemma 4 12B dropping the encoder, Kimi K3 training encoders from scratch, and Inkling 2 Small reintroducing an encoder. Existing models have varied in data, compute, and pretraining choices, preventing a clear consensus.

**「Impact」** Encoder-free models trailed across backbone sizes from 0.6B to 6.4B and required approximately 3x the compute to match performance, demonstrating that vision-only parameters are required. The evaluated "in-fusion" placement achieved about 13% lower time to first token compared to standard separate encoders while maintaining comparable VQA performance.

**Tags**: `#multimodal models`, `#vision encoder`, `#artificial intelligence`, `#machine learning research`

---

<a id="item-tech-news-3"></a>
### [Developer Creates Open-Source Tool to Accelerate cudaMemcpy Pageable Transfers 5x on B300](https://www.reddit.com/r/MachineLearning/comments/1xx2n25/making_cudamemcpy_5x_faster_on_a_b300_p/) ⭐️ 8.0/10

A developer has released an open-source tool designed to accelerate pageable CPU-to-GPU cudaMemcpy memory transfers. Benchmarks shared by the author show that copying a 1 GB tensor on a B300 system improved from 10.2 GB/s to 51.5 GB/s using the tool. The implementation and tuning utility are available via GitHub and an accompanying blog post.

reddit · r/MachineLearning · /u/makneeee · Nov 15, 18:20

**「Background」** Standard pageable host memory transfers in CUDA can often be a performance bottleneck compared to pinned \(page-locked\) memory operations. The newly released tool aims to optimize these host-to-device and device-to-host pathways without requiring manual code rewrites.

**「Impact」** Machine learning engineers and systems developers working with unpinned host tensors can achieve significantly faster data transfer speeds between the CPU and GPU by integrating the tuning utility into their workflows.

**Tags**: `#CUDA`, `#GPU memory`, `#Performance Optimization`, `#Machine Learning Hardware`

---

