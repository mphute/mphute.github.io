---
layout: paper
categories: papers
url: /papers/
permalink: papers/semitruths
id: semitruths

# cover
feature-title: "Semi Truths"
feature-description: "A Large-Scale Dataset for Testing Robustness of AI-Generated Image Detectors"
image: /images/featured/
featured: true
feature-order: 20240815
coming-soon: false
venue: NeurIPS
year: 2024
award: 
award-link:
code: 

# content
title: "Semi Truths: A Large-Scale Dataset for Testing Robustness of AI-Generated Image Detectors"
authors:
  - Anisha Pal
  - Julia Kruk
  - Mansi Phute
  - Manognya Bhattaram
  - Diyi Yang
  - Polo Chau
  - Judy Hoffman
pdf: /papers/
figure: /images/papers/
caption: 
selected: false
type: conference
doi: 
bibtex: |-


---
While text-to-image diffusion models have demonstrated impactful applications in art, design, and entertainment, these technologies also facilitate the spread of misinformation. Recent efforts have developed AI-generated image detectors claiming robustness against various augmentations, but their effectiveness remains unclear. Can these systems detect varying degrees of augmentation? Do they exhibit biases towards specific scenes or data distributions? To address these questions, we introduce Semi-Truths, featuring 27,635 real images, 245,360 masks, and 850,226 AI-augmented images featuring varying degrees of targeted and localized edits, created using diverse augmentation methods, diffusion models, and data distributions. Each augmented image includes detailed metadata for standardized, targeted evaluation of detector robustness. Our findings suggest that state-of-the-art detectors are sensitive to different degrees of edits, data distributions, and editing techniques, providing deeper insights into their functionality.