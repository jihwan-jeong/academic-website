---
title: Conservative Bayesian Model-Based Value Expansion for Offline Policy Optimization (under review)
summary: A model-based offline RL algorithm that is able to trade-off the uncertainty of the learned dynamics model with that of the value function through Bayesian posterior estimation, achieving state-of-the-art performance on a variety of D4RL benchmark tasks. 
tags:
  - Offline RL
date: '2022-10-04T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: PGM description of CBOP
  focal_point: Smart

# links:
#   - icon: book
#     icon_pack: fa
#     name: Paper
#     url: https://arxiv.org/submit/4531177/view
url_code: ''
url_pdf: https://arxiv.org/abs/2210.03802
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""

show_breadcrumb: true

profile: true
---

Offline reinforcement learning (RL) addresses the problem of learning a performant policy from a fixed batch of data collected by following some behavior policy. Model-based approaches are particularly appealing in the offline setting since they can extract more learning signals from the logged dataset by learning a model of the environment. However, the performance of existing model-based approaches falls short of model-free counterparts, due to the compounding of estimation errors in the learned model. Driven by this observation, we argue that it is critical for a model-based method to understand when to trust the model and when to rely on model-free estimates, and how to act conservatively w.r.t. both. To this end, we derive an elegant and simple methodology called conservative Bayesian model-based value expansion for offline policy optimization (CBOP), that trades off model-free and model-based estimates during the policy evaluation step according to their epistemic uncertainties, and facilitates conservatism by taking a lower bound on the Bayesian posterior value estimate. On the standard D4RL continuous control tasks, we find that our method significantly outperforms previous model-based approaches: e.g., MOPO by 116.4%, MOReL by 23.2% and COMBO by 23.7%. Further, CBOP achieves state-of-the-art performance on 11 out of 18 benchmark datasets while doing on par on the remaining datasets.