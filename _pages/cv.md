---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---


{% include toc %}

Education
======
* M.Phil in Hong Kong University of Science and Technology (Guangzhou), 2027
* B.Eng. in Hong Kong University of Science and Technology (Guangzhou), 2023

Work experience
======

* Spring 2025: Academic Researcher
  * Yu Ling Technology Co.,
  * Duties includes: Nerual Network Framework Design for Embodied AI/VAD


Project experience
======
**End-to-End Customer Support Automation System** | *HKUST(GZ)* | *2024*
* **Project Overview**: Engineered a high-performance automation pipeline integrating Parameter-Efficient Fine-Tuning (PEFT) for intent classification and Large Language Model (LLM) prompt engineering for intelligent response generation.
* **Technical Implementation - Intent Classification**: 
    * Fine-tuned **DistilBERT** using **LoRA (Low-Rank Adaptation)**, training only **0.45%** (296k) of the total 66M parameters to minimize memory footprint and prevent catastrophic forgetting.
    * Implemented **Data Augmentation** via WordNet-based synonym replacement and utilized weighted loss functions to address real-world class imbalance across 11 intent categories.
    * Conducted rigorous statistical evaluation including **Bootstrap resampling** for 95% confidence intervals and **ROC analysis**, achieving a micro-average AUROC of **0.9998**.
* **Technical Implementation - Generation Module**: 
    * Integrated **Qwen2.5:3b** using **few-shot prompting** and category-specific system messages to ensure professional tone and policy compliance.
    * Developed a **Self-Consistency mechanism** that generates multiple candidate responses and utilizes an LLM-based judge to score outputs based on professionalism, clarity, and empathy.
* **Key Results & Performance**:
    * **State-of-the-Art Accuracy**: Achieved **99.63% test accuracy**, significantly outperforming the zero-shot baseline of 24.3%.
    * **Production-Grade Efficiency**: Optimized system for real-time deployment with an inference latency **<50ms per query** and a lightweight LoRA adapter size of just **2.5MB**.
    * **High Data Efficiency**: Attained **99.51% accuracy with only 100 training samples**, demonstrating exceptional sample efficiency through transfer learning.

**M2AD-DinomalyV2: Multi-View Multi-Illumination Unsupervised Anomaly Detection** | *Lead Developer* | *2025*
*  **Project Overview**: Developed an advanced unsupervised anomaly detection (AD) framework, M2AD-DinomalyV2, to address industrial inspection challenges under complex multi-view and varying illumination conditions.
* **Technical Implementation - Model Optimization**: 
    *  Built upon the **Dinomaly** baseline, implementing a structured reconfiguration of training schedules and regularization intensity to enhance model stability.
    *  Performed a two-stage **Optuna-based hyperparameter search** to ensure consistency between constrained optimization and real-world re-training performance.
* **Technical Implementation - Data & Inference Engineering**: 
    *  Integrated a lightweight **ColorJitter** preprocessing pipeline to align light and chromaticity distributions, effectively narrowing the "normal distribution" tail for better separability of anomalies.
    *  Developed a **Test-Time Augmentation (TTA)** strategy using multi-crop averaging to reduce viewpoint variance and smooth cross-view ranking without altering evaluation scripts.
* **Key Results & Impact**:
    *  **Championship Performance**: Secured the **First Prize (National Finals)** in the 2025 Micro-Enterprise Intelligent Computing Competition (MEICC) Smart Manufacturing track.
    *  **State-of-the-Art Metrics**: Achieved a final balanced score of **89.814**, with a Mean AUROC of **94.15** for objects and **85.51** for viewpoints on the M2AD-Synergy dataset.
    * **Robustness**: Demonstrated significant performance gains in challenging categories such as "Bird," "Doll," and "Tube," which are highly sensitive to material reflection and lighting shifts.




Skills
======
* **Technical & Programming Proficiency**
  * Proficient in programming languages including Python and C++
  * Strong foundation in mathematics and statistics for machine learning and data analysis
  * Abundant practice & experience in embedded development
* **AI & Machine Learning Expertise**
  * Strong understanding of Generative AI
    * Expertise in core paradigms (diffusion, transformer, closed-source APIs)
    * Familiarity with key models (diffusion models, video models, VLMs)
    * Proficient in prompt engineering for image and video
  * Hands-on experience in AI research like Embodied AI
* **Research & Soft Skills**
  * Scientific research capability & experience with academic instructors during UG period
  * Creative problem-solving abilities
    * Keen eye for design and aesthetics
  * Excellent communication and documentation skills
  * Fluent English Speaker

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
  