---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

 Education
======
* **National University of Singapore (NUS)**, Singapore
  * M.Eng in Computer Engineering (Incoming)
  * Jan 2026 - Jan 2027

* **Beijing University of Posts and Telecommunications (BUPT)**, Beijing, China
  * B.Eng in Software Engineering
  * Sept 2020 - July 2024
  * **Honors**: Outstanding Undergraduate Scholarship (2021, 2022)
  * **Relevant Coursework**: AI Fundamentals (95), Data Mining (96), Probability & Stochastic Processes (95), Numerical Analysis (90), Algorithms & Data Structures (92).

 Experience
======
* **Baidu**, Beijing, China
  * *Algorithm Engineer* (Full-time)
  * Nov 2024 - Jan 2026
  * **Honors**: Baidu Q1 Award; Baidu 2024 Top Team Award.

* **Institute for AI Industry Research (AIR), Tsinghua University**, Beijing, China
  * *Algorithm Intern*
  * Mar 2024 - Oct 2024

 Projects
======
**Lightning Model Training (Foundation Model)** | *Baidu* | *Apr 2025 - Jan 2026*
* **Overview**: Core member leading the full-parameter training of a 100B parameter model using 768 H800 GPUs within a 2000-card cluster. Involved in the full lifecycle from pre-training to post-training.
* **Megatron Optimization**: Developed an online distillation module based on Megatron-LM. Implemented new model classes and custom operators, refactored data loading pipelines for real-time teacher inference, and optimized loss calculation from per-token to per-sequence.
* **RL Training & Consistency**: Addressed training-inference inconsistency in SGLang (Rollout) by introducing the ICE-POP algorithm, aligning generation and training distributions to improve instruction following and reasoning stability.
* **Data Engineering**: Constructed a 5M high-quality instruction tuning dataset. Designed a multi-stage cleaning pipeline involving rule-based filtering, LLM-Judge scoring for safety/compliance, and rejection sampling with multi-turn response evaluation.
* **Strategy**: Executed "General Knowledge Injection" and "Annealing" strategies during pre-training. Employed hierarchical annealing with short-text high-quality data followed by long-context training.

**E-commerce Specialized Model** | *Baidu* | *Feb 2025 - Mar 2025*
* **Pipeline**: Adopted DeepSeek-R1 training workflow. Generated diverse response pairs by adjusting temperature and querying online models.
* **Reward Modeling**: Built a voting workflow on Dify to construct a high-quality preference dataset. Trained the Sky Reward Model and filtered the top 50% data for SFT.
* **RL Training**: Conducted GRPO reinforcement learning using SFT and Sky Reward models. Enforced strict constraints (length, diversity, language consistency) to prevent reward hacking.
* **Results**: The specialized model significantly outperformed the online baseline (91/100 wins in human eval) and maintained a lead against other models like api6.

**Multimodal Image Discretization & Recommendation** | *Baidu* | *Nov 2024 - Jan 2025*
* **Architecture**: Integrated VQ-VAE into Qwen2.5-VL-7B to convert continuous image features into discrete token sequences, trained with end-to-end LM loss.
* **Optimization**: Replaced VQ-VAE with RQ-VAE (Residual Quantized VAE) to solve codebook collapse issues, using residual quantization to enhance feature diversity.
* **Application**: Generated high-quality discrete image IDs for downstream recommendation systems. Validated semantic distinctiveness via cluster analysis (high Silhouette Coefficient).

**Dynamic Attention** | *Tsinghua AIR* | *Aug 2024 - Jan 2025*
* **Method**: Introduced a linear layer (`h_proj`) to compute dynamic thresholds for attention heads, filtering weights to optimize context processing.
* **Efficiency**: Applied Top-k selection to handle long-context data, maintaining summarization accuracy while avoiding performance degradation.
* **Sparse Attention**: Utilized VectorDB for sparse attention, reducing time complexity from $O(n^2)$ to $O(n \log n)$.

 Publications
======
* **[AAAI'26]** **AdaFuse: Accelerating Dynamic Adapter Inference via Token-Level Pre-Gating and Fused Kernel Optimization.**
  * **Qiyang Li**, Rui Kong, Yuchen Li†, Hengyi Cai, Shuaiqiang Wang, Linghe Kong, Guihai Chen, Dawei Yin.
  * *The 40th Annual AAAI Conference on Artificial Intelligence (AAAI)*, 2026. (CCF-A)

* **[Nature Communications]** **Accelerate Large Language Model Reasoning with Statistical Language Patterns — A Shannon's Legacy.**
  * Yuchen Li*, **Qiyang Li***, Rui Kong, Hengyi Cai, Shuaiqiang Wang, Shahid Mumtaz, Guihai Chen, Linghe Kong, Dawei Yin.
  * *Nature Communications*. (Major Revision, Co-First Author)

* **[Preprint]** **Test-time Reward Augmentation Improves Large Language Model Reasoning.**
  * **Qiyang Li**, Rui Kong, Yuchen Li, Hengyi Cai, Danni Wang, Haojie Zhang, Jiamin Chen, Yu Wang, Jiashu Zhao, Jimmy Huang, Haoyi Xiong, Shuaiqiang Wang.
  * *arXiv preprint*, 2025.

* **[TMC]** **FlexSpec: Frozen Drafts Meet Evolving Targets in Edge-Cloud Collaborative LLM Speculative Decoding.**
  * Yuchen Li, Rui Kong, Zhonghao Lyu, **Qiyang Li**, Xinran Chen, Hengyi Cai, Lingyong Yan, Shuaiqiang Wang, Jiashu Zhao, Guangxu Zhu, Linghe Kong, Guihai Chen, Haoyi Xiong, Dawei Yin.
  * *IEEE Transactions on Mobile Computing (TMC)*. (Under Review, CCF-A)

 Competitions & Awards
======
* **Second Prize**, APMCM Asia-Pacific Mathematical Contest in Modeling (2022)
* **Meritorious Winner (M Prize)**, MCM/ICM (US Mathematical Contest in Modeling)
* **Grand Prize**, Beijing "Te Ruan Cup" (Software Competition)
* **First Prize**, Beijing University Mathematics Competition; **Second Prize**, National University Mathematics Competition
* **First Prize**, Undergraduate Innovation and Entrepreneurship Exhibition
* **Second Prize**, Beijing Mechanical Innovation Design Competition

 Skills
======
* **Distributed Training**: Expert in Megatron-LM and DeepSpeed. Experienced with 3D Parallelism (TP/PP/DP), ZeRO optimization, and communication tuning on large-scale clusters (2000+ H800s).
* **Post-Training**: Proficient in SFT, RLHF (PPO/GRPO/DPO), Model Distillation, and Pruning.
* **Data Engineering**: Skilled in constructing large-scale datasets (millions of samples), LLM-Judge evaluation, and Rejection Sampling pipelines.
* **Frontier Tech**: Deep understanding of latest LLM advancements (DeepSeek-R1, V2, Agents). Strong ability in paper reproduction and engineering implementation.
