---
layout: paper
categories: papers
permalink: papers/llmselfdefense
id: llmselfdefense
title: LLM Self Defense: By Self Examination, LLMs Know They Are Being Tricked
authors:
    - Mansi Phute
    - Alec Helbling
    - Matthew Hull
    - Anthony Peng
    - Sebastian Szyller
    - Cory Cornelius
    - Duen Horng (Polo) Chau
venue: arXiv
venue-shorthand: arXiv
location: https://arxiv.org/abs/2308.07308
year: 2023
url: /papers/llmselfdefense
demo: 
pdf: /papers/19-parametric-viscomm.pdf
code: 
type: preprint
featured: true
selected: true
feature-title: LLM Self Defense
feature-description: LLM's can filter out harmful content produced by themselves!
bibtex: |-
    @misc{phute2023llm,
      title={LLM Self Defense: By Self Examination, LLMs Know They Are Being Tricked}, 
      author={Mansi Phute and Alec Helbling and Matthew Hull and ShengYun Peng and Sebastian Szyller and Cory Cornelius and Duen Horng Chau},
      year={2023},
      eprint={2308.07308},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
    }
---

Large language models (LLMs) are popular for high-quality text generation but can produce harmful content, even when aligned with human values through reinforcement learning. Adversarial prompts can bypass their safety measures. We propose LLM Self Defense, a simple approach to defend against these attacks by having an LLM screen the induced responses. Our method does not require any fine-tuning, input preprocessing, or iterative output generation. Instead, we incorporate the generated content into a pre-defined prompt and employ another instance of an LLM to analyze the text and predict whether it is harmful. We test LLM Self Defense on GPT 3.5 and Llama 2, two of the current most prominent LLMs against various types of attacks, such as forcefully inducing affirmative responses to prompts and prompt engineering attacks. Notably, LLM Self Defense succeeds in reducing the attack success rate to virtually 0 using both GPT 3.5 and Llama 2.
