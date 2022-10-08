---
title: Online Class-Incremental Continual Learning with Adversarial Shapley Value (AAAI-21)
summary: We use 
tags:
- Continual Learning
date: "2021-01-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: ""
  focal_point: Smart

# links:
#   - icon: book
#     icon_pack: fa
#     name: Paper
#     url: https://ssanner.github.io/papers/aaai21_aser.pdf
url_code: ''
url_pdf: 'https://ssanner.github.io/papers/aaai21_aser.pdf'
url_slides: ''
url_video: 'https://slideslive.com/38949257/online-classincremental-continual-learning-with-adversarial-shapley-value?locale=de'
---

In this paper, we specifically focus on the online class-incremental setting where a model needs to learn new classes continually from an online data stream. To this end, we contribute a novel Adversarial Shapley value scoring method that scores memory data samples according to their ability to preserve latent decision boundaries for previously observed classes (to maintain learning stability and avoid forgetting) while interfering with latent decision boundaries of current classes being learned (to encourage plasticity and optimal learning of new class boundaries). Overall, we observe that our proposed ASER method provides competitive or improved performance compared to state-of-the-art replay-based continual learning methods on a variety of datasets.