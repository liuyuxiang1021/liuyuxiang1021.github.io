---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

<div class="language-switcher" role="group" aria-label="Language switcher">
  <button type="button" class="language-switcher__button is-active" data-language-button="en">EN</button>
  <button type="button" class="language-switcher__button" data-language-button="zh">中文</button>
</div>

<div class="language-panel language-panel--en" data-language-panel="en" markdown="1">

Hi, I'm **Yuxiang Liu (刘宇翔)**. Welcome to my homepage!

I am an undergraduate student at the College of Intelligence and Computing, **Tianjin University (TJU)**.

My research interests include **3D Reconstruction**, **multimodal video-audio generation**, and **egocentric spatiotemporal reasoning**.

My work has been accepted by **ICML 2026**, and my team won **first place** in the Skeleton Tracking Challenge at the **CVPR 2025 Global 3D Human Poses (G3P) Workshop**. I have also received the **National Scholarship** for two consecutive years.

**My Email:** lyx1021@tju.edu.cn

# 🔥 News {#news}
- *2026.09*: &nbsp;🚀 Released [**EgoTSR++**](https://arxiv.org/abs/2609.31751), a framework for egocentric spatiotemporal reasoning and task-progress understanding.
- *2026.08*: &nbsp;🚀 Released [**TurboT2VA**](https://arxiv.org/abs/2608.24674), our framework for fast joint text-to-video-audio generation, achieving **54.67× generator-only speedup** at high resolution on a single NVIDIA H20.
- *2026.05*: &nbsp;🎉 Paper accepted by **ICML 2026**: [**EgoTSR**](https://arxiv.org/abs/2604.10517) — Evolving Ego-Centric Task-Oriented Spatiotemporal Reasoning via Curriculum Learning.
- *2025.12*: &nbsp;⭐ Awarded the **National Scholarship** for the academic year 2024-2025.
- *2025.06*: &nbsp;🏆 Won **first place** in the Skeleton Tracking Challenge at the [CVPR 2025 G3P Workshop](https://g3p-workshop.github.io/).
- *2024.12*: &nbsp;⭐ Awarded the **National Scholarship** for the academic year 2023-2024.

# 📝 Publications {#publications}
(* co-first author, † corresponding author)

- [**EgoTSR++: Egocentric Spatiotemporal Reasoning for Task Progress Understanding**](https://arxiv.org/abs/2609.31751)
  <br>
  Xiaoda Yang\*, Can Wang\*, **Yuxiang Liu**, Pengfei Zhou, Jianwen Lou, Shuicheng Yan<sup>†</sup>
  <br>
  *arXiv preprint, 2026* &nbsp;\[[**Paper**](https://arxiv.org/abs/2609.31751)\]
  - Introduced a framework for diagnosing and improving order-robust task-progress understanding in egocentric scenarios.
  - Built **SpatialLogic-Bench** to evaluate physical state pairs in both original and order-swapped presentations, exposing input-order bias in representative VLMs.
  - Combined bidirectional supervision, failure-aware data, and a progressive CoT-to-Tag curriculum, achieving **92.4% long-horizon accuracy** and improving non-monotonic trajectory understanding.

- [**TurboT2VA: Fast Large-Scale Text-to-Video-Audio Generation via Score-Regularized Consistency Distillation**](https://arxiv.org/abs/2608.24674)
  <br>
  Xiaoda Yang\*, **Yuxiang Liu**\*, Kaiwen Zheng, Yuan Liu, Yibo Lai, Shengpeng Ji, Kai Jiang, Jianfei Chen, Shan Yang, Sen Liang, Xiaobin Hu, Shuicheng Yan, Jintao Zhang<sup>†</sup>, Jun Zhu<sup>†</sup>, Zhou Zhao<sup>†</sup>
  <br>
  *arXiv preprint, 2026* &nbsp;\[[**Paper**](https://arxiv.org/abs/2608.24674) | [**Code & Demos**](https://github.com/thu-ml/TurboDiffusion/tree/main/turbot2va)\]
  - Proposed **TurboT2VA**, a score-regularized consistency distillation framework that accelerates a **19B-parameter** joint video-audio model while preserving quality, diversity, and synchronization.
  - Distilled a **40-step teacher into a 4-step student** with progressive discrete consistency warm-up, continuous consistency refinement, and joint consistency–distribution matching, achieving **20.1× generator speedup** at 512×768 resolution.
  - Combined W8A8 quantization, fused operators, and modality-aware sparse attention to achieve **54.67× generator-only speedup** at 1024×1792 resolution on a single **NVIDIA H20** (318.74s → 5.83s).

- [**From Perception to Planning: Evolving Ego-Centric Task-Oriented Spatiotemporal Reasoning via Curriculum Learning**](https://arxiv.org/abs/2604.10517)
  <br>
  Xiaoda Yang\*, **Yuxiang Liu**\*, Shenzhou Gao, Can Wang, Jingyang Xue, Lixin Yang, Yao Mu, Tao Jin, Shuicheng Yan, Zhimeng Zhang, Zhou Zhao<sup>†</sup>
  <br>
  *ICML 2026* &nbsp;\[[**Paper**](https://arxiv.org/abs/2604.10517) | [**Code**](https://github.com/Collab-Gen/EgoTSR)\]
  - Proposed **EgoTSR**, a curriculum-based framework for learning task-oriented spatiotemporal reasoning that evolves from explicit spatial understanding to long-horizon planning.
  - Constructed **EgoTSR-Data**, a large-scale dataset comprising 46 million samples organized into three stages: CoT supervision, weakly supervised tagging, and long-horizon sequences.
  - Achieved **92.4% accuracy** on long-horizon logical reasoning tasks, significantly outperforming existing open-source and closed-source state-of-the-art models.

- [**Robust Camera Pose Estimation and 3D Human Reconstruction for Sports Events**](https://g3p-workshop.github.io/assets/pdfs/solution-tim.pdf)
  <br>
  Jing Huang, Hanrong Zhuang, Lin Zhang, **Yuxiang Liu**, Kun Li<sup>†</sup>
  <br>
  *Technical Report for FIFA Skeleton Light Challenge 2025* &nbsp;\[[**Paper**](https://g3p-workshop.github.io/assets/pdfs/solution-tim.pdf) | [**Slides**](https://g3p-workshop.github.io/assets/pdfs/talk-hj.pdf)\]
  - Proposed a method extending the **RCR (Robust Crowd Reconstruction)** framework to video inputs for sports events.
  - Designed a relative camera pose search algorithm with a fast line projector to achieve robustness and efficiency.
  - Refined 3D HVIP to ensure the consistency of human movement and extracted 3D skeletons from SMPL parameters.

{% comment %}
# 🔬 Research Projects & Competitions {#research-projects-and-competitions}

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">arXiv 2026</div>
      <a href="https://arxiv.org/abs/2608.24674">
        <img src='images/turbot2va.png' alt="TurboT2VA: fast joint text-to-video-audio generation with 54.67× generator-only speedup" width="100%">
      </a>
    </div>
  </div>
  <div class='paper-box-text' markdown="1">

  **TurboT2VA: Fast Large-Scale Text-to-Video-Audio Generation via Score-Regularized Consistency Distillation**

  [**Paper**](https://arxiv.org/abs/2608.24674) \| [**Code & Demos**](https://github.com/thu-ml/TurboDiffusion/tree/main/turbot2va) (arXiv 2026)

  - Accelerated a **19B-parameter** joint video-audio model with progressive consistency distillation from **40 steps to 4 steps**, preserving quality, diversity, and synchronization.
  - Achieved **20.1× generator speedup** at 512×768 resolution through four-step distillation.
  - Combined distillation with W8A8 quantization, fused operators, and sparse attention for **54.67× generator-only speedup** at 1024×1792 resolution on one **NVIDIA H20**.
  </div>
</div>

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">ICML 2026</div>
      <img src='images/paper-egotsr/egotsr_thumbnail.png' alt="EgoTSR" width="100%" onerror="this.src='https://dummyimage.com/500x300/e0e0e0/000000.png&text=EgoTSR'">
    </div>
  </div>
  <div class='paper-box-text' markdown="1">

  **EgoTSR: Evolving Ego-Centric Task-Oriented Spatiotemporal Reasoning via Curriculum Learning**
  
  [arXiv 2604.10517](https://arxiv.org/abs/2604.10517) (ICML 2026)
  
  - Proposed a curriculum-based framework that evolves from explicit spatial understanding to internalized task-state assessment and long-horizon planning.
  - Constructed EgoTSR-Data with **46 million samples** across three stages: CoT supervision, weakly supervised tagging, and long-horizon sequences.
  - Achieved **92.4% accuracy** on long-horizon logical reasoning, outperforming existing SOTA models.
  </div>
</div>

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">CVPR Winner</div>
      <img src='images/g3p_champion.png' alt="G3P Challenge" width="100%" onerror="this.src='https://dummyimage.com/500x300/e0e0e0/000000.png&text=CVPR+Winner'">
    </div>
  </div>
  <div class='paper-box-text' markdown="1">

  **Champion of FIFA Innovation Challenge Skeleton Tracking Light**
  
  [**CVPR 2025 Global 3D Human Poses (G3P) Workshop**](https://g3p-workshop.github.io/)
  
  - Achieved **Rank 1** on the leaderboard. Invited to deliver the Winner Talk.
  - Developed a robust method for 3D skeleton tracking in complex unstructured scenarios.
  </div>
</div>
{% endcomment %}

{% comment %}
<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">Project Leader</div>
      <img src='images/image_stitching_project.png' alt="Image Stitching" width="100%" onerror="this.src='https://dummyimage.com/500x300/e0e0e0/000000.png&text=Image+Stitching'">
    </div>
  </div>
  <div class='paper-box-text' markdown="1">

  **Unstructured Large Scene Light Field Image Stitching**
  
  **National Innovation and Entrepreneurship Training Program** (2024.08 - Present)
  
  - Advisor: Prof. [Kun Li](https://cic.tju.edu.cn/faculty/likun/index.html) and Assistant Researcher [Jian Ma](https://majian8.github.io/).
  - Focusing on Trusted Projection and 3D Reconstruction for large-scale scenes.
  - Investigating algorithms for non-structured light field data processing.
  </div>
</div>
{% endcomment %}

{% comment %}
<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">Project</div>
      <img src='images/project-multimodal.png' alt="Multimodal Project" width="100%" onerror="this.src='https://dummyimage.com/500x300/e0e0e0/000000.png&text=Multimodal'">
    </div>
  </div>
  <div class='paper-box-text' markdown="1">

  **Multimodal Data Modeling & Knowledge Discovery**

  **National Innovation and Entrepreneurship Training Program** (2024.04 - 2025.04)

  - **Core Member**. Advisor: Prof. [Yu Wang](https://faculty.tju.edu.cn/wangyu_ai/zh_CN/index.htm).
  - **Status:** Completed (One-year Project).
  - Implemented YOLO-based algorithms for license plate recognition under challenging conditions (high angle, blur, low light).
  - Achieved high accuracy in complex environments.
  </div>
</div>
{% endcomment %}


# 🏅 Honors and Awards {#honors-and-awards}

{% comment %}
**International & National**
- *2026* **Paper Accepted**, ICML 2026.
{% endcomment %}
- *2025.06* **Champion**, FIFA Skeleton Tracking Challenge (CVPR 2025 Workshop).
- *2024–2025 academic year* **National Scholarship** (Ministry of Education of China).
- *2023–2024 academic year* **National Scholarship** (Ministry of Education of China).

{% comment %}
**Provincial & Regional**
- *2025* **First Prize**, Lanqiao Cup National Software Talent Competition (C/C++, Tianjin Area).
- *2024* **First Prize**, Tianjin Arts Performance (Orchestra).
{% endcomment %}

{% comment %}
# 🌟 Leadership & Activities {#leadership-and-activities}
- *2025.09 - Present*: **President**, Student Union, School of Computer Science and Technology, TJU.
- *2024.09 - Present*: **Vice Head**, Peiyang Folk Orchestra.
- *2024.09 - 2025.09*: **League Secretary**, Top-notch Talent Class.
{% endcomment %}

# 📖 Education {#educations}
- *2023.09 - Present*, Undergraduate in Computer Science and Technology, **Tianjin University (TJU)**.
  - **Program**: Top-notch Talent Training Plan 2.0 (Top-notch Talent Class).
{% comment %}
- *2020.09 - 2023.07*, High School, **Shandong Qingdao No. 2 Middle School**.
{% endcomment %}

</div>

<div class="language-panel language-panel--zh" data-language-panel="zh" markdown="1" hidden>

你好，我是 **刘宇翔（Yuxiang Liu）**。欢迎访问我的个人主页！

我是 **天津大学（TJU）智能与计算学部** 计算机科学与技术专业本科生。

我的研究兴趣包括 **三维重建**、**多模态音视频生成** 和 **第一视角时空推理**。

我的工作被 **ICML 2026** 接收，团队曾在 **CVPR 2025 Global 3D Human Poses (G3P) Workshop** 的 Skeleton Tracking Challenge 中获得 **第一名**。此外，我连续两年获得 **国家奖学金**。

**邮箱：** lyx1021@tju.edu.cn

# 🔥 动态 {#news-zh}
- *2026.09*: &nbsp;🚀 发布 [**EgoTSR++**](https://arxiv.org/abs/2609.31751)，一个面向第一视角时空推理与任务进展理解的框架。
- *2026.08*: &nbsp;🚀 发布 [**TurboT2VA**](https://arxiv.org/abs/2608.24674)，一个面向快速联合文本到视频-音频生成的框架，在单张 NVIDIA H20 上实现高分辨率下 **54.67× generator-only 加速**。
- *2026.05*: &nbsp;🎉 论文 [**EgoTSR**](https://arxiv.org/abs/2604.10517) 被 **ICML 2026** 接收：Evolving Ego-Centric Task-Oriented Spatiotemporal Reasoning via Curriculum Learning。
- *2025.12*: &nbsp;⭐ 获得 **2024-2025 学年国家奖学金**。
- *2025.06*: &nbsp;🏆 在 [CVPR 2025 G3P Workshop](https://g3p-workshop.github.io/) Skeleton Tracking Challenge 中获得 **第一名**。
- *2024.12*: &nbsp;⭐ 获得 **2023-2024 学年国家奖学金**。

# 📝 论文发表 {#publications-zh}
（* 共同一作，† 通讯作者）

- [**EgoTSR++: Egocentric Spatiotemporal Reasoning for Task Progress Understanding**](https://arxiv.org/abs/2609.31751)
  <br>
  Xiaoda Yang\*, Can Wang\*, **Yuxiang Liu**, Pengfei Zhou, Jianwen Lou, Shuicheng Yan<sup>†</sup>
  <br>
  *arXiv preprint, 2026* &nbsp;\[[**Paper**](https://arxiv.org/abs/2609.31751)\]
  - 提出一个用于诊断和提升第一视角任务进展理解能力的框架，强调对输入顺序变化保持鲁棒。
  - 构建 **SpatialLogic-Bench**，在原始顺序和交换顺序下评估物理状态对，揭示代表性 VLM 中存在的输入顺序偏差。
  - 结合双向监督、失败感知数据和 progressive CoT-to-Tag curriculum，达到 **92.4% 长时程准确率**，并提升非单调轨迹理解能力。

- [**TurboT2VA: Fast Large-Scale Text-to-Video-Audio Generation via Score-Regularized Consistency Distillation**](https://arxiv.org/abs/2608.24674)
  <br>
  Xiaoda Yang\*, **Yuxiang Liu**\*, Kaiwen Zheng, Yuan Liu, Yibo Lai, Shengpeng Ji, Kai Jiang, Jianfei Chen, Shan Yang, Sen Liang, Xiaobin Hu, Shuicheng Yan, Jintao Zhang<sup>†</sup>, Jun Zhu<sup>†</sup>, Zhou Zhao<sup>†</sup>
  <br>
  *arXiv preprint, 2026* &nbsp;\[[**Paper**](https://arxiv.org/abs/2608.24674) | [**Code & Demos**](https://github.com/thu-ml/TurboDiffusion/tree/main/turbot2va)\]
  - 提出 **TurboT2VA**，一个基于 score-regularized consistency distillation 的框架，用于加速 **19B 参数**联合视频-音频模型，同时保持生成质量、多样性与音画同步。
  - 将 **40 步 teacher 蒸馏为 4 步 student**，结合 progressive discrete consistency warm-up、continuous consistency refinement 与 joint consistency-distribution matching，在 512×768 分辨率下实现 **20.1× generator 加速**。
  - 结合 W8A8 量化、算子融合与 modality-aware sparse attention，在单张 **NVIDIA H20** 上实现 1024×1792 分辨率下 **54.67× generator-only 加速**（318.74s → 5.83s）。

- [**From Perception to Planning: Evolving Ego-Centric Task-Oriented Spatiotemporal Reasoning via Curriculum Learning**](https://arxiv.org/abs/2604.10517)
  <br>
  Xiaoda Yang\*, **Yuxiang Liu**\*, Shenzhou Gao, Can Wang, Jingyang Xue, Lixin Yang, Yao Mu, Tao Jin, Shuicheng Yan, Zhimeng Zhang, Zhou Zhao<sup>†</sup>
  <br>
  *ICML 2026* &nbsp;\[[**Paper**](https://arxiv.org/abs/2604.10517) | [**Code**](https://github.com/Collab-Gen/EgoTSR)\]
  - 提出 **EgoTSR**，一个面向任务导向时空推理的课程学习框架，使模型从显式空间理解逐步演化到长时程规划。
  - 构建 **EgoTSR-Data**，包含 4600 万样本，覆盖 CoT 监督、弱监督标注和长时程序列三个阶段。
  - 在长时程逻辑推理任务上达到 **92.4% 准确率**，显著优于现有开源和闭源先进模型。

- [**Robust Camera Pose Estimation and 3D Human Reconstruction for Sports Events**](https://g3p-workshop.github.io/assets/pdfs/solution-tim.pdf)
  <br>
  Jing Huang, Hanrong Zhuang, Lin Zhang, **Yuxiang Liu**, Kun Li<sup>†</sup>
  <br>
  *Technical Report for FIFA Skeleton Light Challenge 2025* &nbsp;\[[**Paper**](https://g3p-workshop.github.io/assets/pdfs/solution-tim.pdf) | [**Slides**](https://g3p-workshop.github.io/assets/pdfs/talk-hj.pdf)\]
  - 将 **RCR（Robust Crowd Reconstruction）** 框架扩展到体育赛事视频输入。
  - 设计了带快速线投影器的相对相机位姿搜索算法，以提升鲁棒性和效率。
  - 优化 3D HVIP 以保证人体运动一致性，并从 SMPL 参数中提取 3D 骨架。

# 🏅 荣誉奖项 {#honors-and-awards-zh}

- *2025.06* **冠军**，FIFA Skeleton Tracking Challenge（CVPR 2025 Workshop）。
- *2024-2025 学年* **国家奖学金**（中华人民共和国教育部）。
- *2023-2024 学年* **国家奖学金**（中华人民共和国教育部）。

# 📖 教育经历 {#educations-zh}
- *2023.09 - 至今*，**天津大学（TJU）**，计算机科学与技术专业本科生。
  - **项目：** 拔尖学生培养计划 2.0（拔尖班）。

</div>
