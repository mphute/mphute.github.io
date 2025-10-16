---
layout: paper
categories: papers
url: /papers/
permalink: papers/visor-pp
id: visor-pp

# cover
feature-title: VISOR++
feature-description: Transferrable Visual Input based Steering for Output Redirection in Large Vision Language Models
image: /images/featured/
featured: false
feature-order: 20250901
coming-soon: false
venue: arXiV
year: 2025
award: 
award-link:
code: 

# content
title: VISOR++ - Transferrable Visual Input based Steering for Output Redirection in Large Vision Language Models
authors:
  - Ravi Balakrishnan
  - Mansi Phute
pdf: /papers/
figure: /images/papers/
caption: 
selected: false
type: conference
doi:    
bibtex: |-


---
Vision Language Models (VLMs) are increasingly being used in a broad range of applications. 
While existing approaches for behavioral control or output redirection are easily detectable and often ineffective, activation-based steering vectors require invasive runtime access to model internals incompatible with API-based services and closed source deployments. 
We introduce VISOR (Visual Input based Steering for Output Redirection), a novel method that achieves sophisticated behavioral control through optimized visual inputs alone. It enables practical deployment across all VLM serving modalities while remaining imperceptible compared to explicit textual instructions. 
A single 150KB steering image matches, and often outperforms, steering vector performance. 
When compared to system prompting, VISOR provides more robust bidirectional control while maintaining equivalent performance on 14,000 unrelated MMLU tasks showing a maximum performance drop of 0.1\% across different models and datasets. 
Beyond eliminating runtime overhead and model access requirements, VISOR exposes a critical security vulnerability: adversaries can achieve sophisticated behavioral manipulation through visual channels alone, bypassing text-based defenses. 
Our work fundamentally re-imagines multimodal model control and highlights the urgent need for defenses against visual steering attacks.