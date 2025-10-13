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

# About Me
I am currently a first-year Ph.D. student at the [Gaoling School of Artificial Intelligence, Renmin University of China](http://ai.ruc.edu.cn/english/index.htm). I am a member of the [Intelligent Information Retrieval Lab (IIR)](https://ruc-iir-lab.github.io/), supervised by Prof. [Jun Xu](https://scholar.google.com/citations?user=su14mcEAAAAJ) and Assoc. Prof. [Xiao Zhang](https://scholar.google.com/citations?user=5FZ6wbAAAAAJ&hl=en). My research interests include **Large Language Models**, **Reinforcement Learning**, **Information Retrieval**, and **Recommender Systems**. I am always open to collaboration and discussions in these areas. If you are interested, please feel free to reach out!

# Selected Awards
- 🥇 **Gold Medal**, ACM-ICPC Asia Regional Contest, Nanjing, 2024  
- 🥈 **Silver Medal**, China Collegiate Programming Contest (CCPC), Zhengzhou, 2024  
- 🥉 **Bronze Medal**, ACM-ICPC Asia Regional Contest, Hangzhou, 2024  
- 🌍 **Top 0.36% (32 / 8785)** Worldwide, IEEE Xtreme 18 Programming Competition — 2nd in China, 2024  

# Publications

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">Research Project</div><img src='images/project1.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

### [Efficient Activation Optimization for Large-Scale Model Training](#)
**Advisor:** Prof. Yuan Kun, *Peking University* **Duration:** Mar 2025 – May 2025  

- Focused on activation compression algorithms by analyzing the structured sparsity of activation tensors, and developed a dynamic quantization-based mixed-granularity compression scheme.  
- Extended the **COAT quantization framework** to **INT8** and implemented full-process verification on **OLMo**, achieving performance nearly lossless compared to the BF16 baseline.  
- Explored **mixed-granularity activation quantization**, achieving **1.6× acceleration** and **40.8% activation memory reduction** on a single-layer Transformer, and **1.68× end-to-end training speedup** with **35.1% peak memory reduction**.

</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">Research Project</div><img src='images/project2.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

### [Multimodal Large Model Reasoning for Visual Puzzle Understanding](#)
**Institution:** Shanghai Innovation Institute
**Duration:** May 2025  

- Addressed reasoning limitations of large models on **visual grid puzzles** by designing an integrated approach combining **full-parameter fine-tuning**, **Chain-of-Thought (CoT) distillation**, **multi-source data fusion**, and **diversified prompt engineering**.  
- Designed a **CoT distillation pipeline** using *Qwen2.5-VL-72B* to generate reasoning process samples for data augmentation, applying a progressive fusion strategy to boost *Qwen2.5-VL-7B-Instruct*’s cross-task accuracy from **52% to 72%**.  
- Introduced **VGRP-Bench** and designed a **perturbation-based data augmentation** strategy, raising accuracy on high-difficulty tasks (*Aquarium*) from **79% to 92%**.  
- Achieved **4th place (Top 0.7%)** in the *Multimodal Reasoning Puzzle Challenge*.

</div>
</div>

<!-- <div class='paper-box'><div class='paper-box-image'><div><div class="badge">CVPR 2016</div><img src='images/500x300.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Deep Residual Learning for Image Recognition](https://openaccess.thecvf.com/content_cvpr_2016/papers/He_Deep_Residual_Learning_CVPR_2016_paper.pdf)

**Kaiming He**, Xiangyu Zhang, Shaoqing Ren, Jian Sun  

[**Project**](https://scholar.google.com/citations?view_op=view_citation&hl=en&user=DhtAFkwAAAAJ&citation_for_view=DhtAFkwAAAAJ:ALROH1vI_8AC)
<strong><span class='show_paper_citations' data='DhtAFkwAAAAJ:ALROH1vI_8AC'></span></strong>

- This paper presents a residual learning framework to ease the training of networks that are substantially deeper than those used previously.

</div>
</div> -->

# Honors and Scholarships
- 🌟 **National Scholarship** (Dec 2024, Dec 2023)  
- 💡 **CCF Outstanding Undergraduate Program** (Oct 2025)  
- ✨ **First-Class Scholarship**, Xidian University (Dec 2022)  

# Education
- *2026.09 – Present*, **Ph.D. Candidate**, Gaoling School of Artificial Intelligence, Renmin University of China, Beijing, China  
- *2022.09 – 2026.06*, **B.Eng.**, School of Computer Science, Xidian University, Xi’an, China  

# Internships
- *2025.10 – Present*, [Tencent WeChat Group](https://github.com/), China  
  
# Invited Talks

  - Invited to give a talk at the Programming Contest Seminar of Xidian University — [news](https://mp.weixin.qq.com/s/mXxvLBQzaQkp8iAplRgCAw)


# Other
In my spare time, I enjoy participating in Programming Contests and playing chess. I have been playing chess since the age of four and hold the title of **Master of the Chinese Chess Association**. I was the **Youth Champion of Anhui Province** in **2012, 2013, and 2014**.