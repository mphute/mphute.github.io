---
layout: paper
categories: papers
url: /papers/
permalink: papers/llm-attributor
id: llm-attributor

# cover
feature-title: LLM Attributor
feature-description: Interactive Visual Attribution for LLM Generation
image: /images/featured/
featured: true
feature-order: 20240530
coming-soon: false
venue: VIS
year: 2024
award: 
award-link:
code: 

# content
title:
authors:
    - Seongmin Lee
    - Jay Wang
    - Aishwarya Chakravarthy
    - Alec Helbling
    - ShengYun Peng
    - Mansi Phute
    - Duen Horng (Polo) Chau
    -  Minsuk Kahng
pdf: /papers/
figure: /images/papers/
caption: 
selected: false
type: poster
doi: 
bibtex: |-
@article{lee2024llm,
  title={LLM Attributor: Interactive Visual Attribution for LLM Generation},
  author={Lee, Seongmin and Wang, Zijie J and Chakravarthy, Aishwarya and Helbling, Alec and Peng, ShengYun and Phute, Mansi and Chau, Duen Horng and Kahng, Minsuk},
  journal={arXiv preprint arXiv:2404.01361},
  year={2024}
}

---

While large language models (LLMs) have shown remarkable capability to generate convincing text across diverse domains, concerns around its potential risks have highlighted the importance of understanding the rationale behind text generation. We present LLM Attributor, a Python library that provides interactive visualizations for training data attribution of an LLM's text generation. Our library offers a new way to quickly attribute an LLM's text generation to training data points to inspect model behaviors, enhance its trustworthiness, and compare model-generated text with user-provided text. We describe the visual and interactive design of our tool and highlight usage scenarios for LLaMA2 models fine-tuned with two different datasets: online articles about recent disasters and finance-related question-answer pairs. Thanks to LLM Attributor's broad support for computational notebooks, users can easily integrate it into their workflow to interactively visualize attributions of their models. For easier access and extensibility, we open-source LLM Attributor at this https URL LLM-Attribution. The video demo is available at this https URL.