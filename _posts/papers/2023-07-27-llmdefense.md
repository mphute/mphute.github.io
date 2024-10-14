---
layout: paper
categories: papers
permalink: papers/llm-self-defense
url: /papers/llm-self-defense
id: llm-self-defense

# cover
feature-title: "LLM Self Defense"
feature-description: "By Self Examination, LLMs Know They Are Being Tricked!"
image: /images/featured/23_llm-self-defense.png
featured: true
feature-order: 20230815
coming-soon: false
venue: ICLR Tiny Paper
year: 2024
award: Deployed at ADP
award-link:
code: https://github.com/poloclub/llm-self-defense

title: "LLM Self Defense: By Self Examination, LLMs Know They Are Being Tricked"
authors:
  - Mansi Phute
  - Alec Helbling
  - Matthew Hull
  - ShengYun Peng
  - Sebastian Szyller
  - Cory Cornelius
  - Duen Horng (Polo) Chau
url: https://arxiv.org/abs/2308.07308
pdf: /papers/23-llmselfdefense.pdf
figure: /images/papers/23_llm-self-defense.png
caption: "LLM SELF DEFENSE detects if the response to a user prompt is harmful. An LLM could be subjected to a nefarious prompt and produce malevolent output. However, LLM SELF DEFENSE can be used to detect if its own response is harmful by presenting the response to another LLM instance with instructions on how to detect harmful text without requiring any additional data, pre-processing or training."
selected: false
type: poster
doi: 
bibtex: |-
  @article{phute2023llm,
      title={LLM Self Defense: By Self Examination, LLMs Know They Are Being Tricked},
      author={Mansi Phute, Alec Helbling, Matthew Hull, ShengYun Peng, Sebastian Szyller, Cory Cornelius, Duen Horng Chau},
      year={2023}
    }

---

Large language models (LLMs) are popular for high-quality text generation but can produce harmful content, even when aligned with human values through reinforcement learning. Adversarial prompts can bypass their safety measures. We propose "LLM Self Defense", a simple approach to defend against these attacks by having an LLM screen the induced responses. Our method does not require any fine-tuning, input preprocessing, or iterative output generation. Instead, we incorporate the generated content into a pre-defined prompt and employ another instance of an LLM to analyze the text and predict whether it is harmful. We test LLM Self Defense on GPT 3.5 and Llama 2, two of the current most prominent LLMs against various types of attacks, such as forcefully inducing affirmative responses to prompts and prompt engineering attacks. Notably, LLM Self Defense succeeds in reducing the attack success rate to virtually 0 using both GPT 3.5 and Llama 2.