---
title: A Distributional Framework for Risk-Sensitive End-to-End Planning in Continuous MDPs (AAAI-22)
summary: End-to-end planning framework for risk-sensitive planning under stochastic environments by backpropagating through a model of the environment.  The core idea is to use reparameterization of the state distribution, leading to a unique distributional perspective of end-to-end planning where the return distribution is utilized for sampling as well as optimizing risk-aware objectives by backpropagation in a unified framework.
tags:
- Planning
date: "2022-01-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: RAPTOR
  alt_text: RAPTOR agents learn to avoid the dangerous zone in the middle
  focal_point: Smart

url_code: ''
url_pdf: https://ssanner.github.io/papers/aaai22_raptor.pdf
url_slides: ''
url_video: 'https://aaai-2022.virtualchair.net/poster_aaai10867'

slides: ""

profile: true

show_breadcrumb: true

# commentable: true
---

Recent advances in efficient planning in deterministic or stochastic high-dimensional domains with continuous action spaces leverage backpropagation through a model of the environment to directly optimize action sequences. However, existing methods typically do not take risk into account when optimizing in stochastic domains, which can be incorporated efficiently in MDPs by optimizing a nonlinear utility function of the return distribution. We bridge this gap by introducing Risk-Aware Planning using PyTorch (RAPTOR), a novel unified framework for risk-sensitive planning through end-to-end optimization of commonly-studied risk-sensitive utility functions such as entropic utility, mean-variance optimization and CVaR. A key technical difficulty of our approach is that direct optimization of general risk-sensitive utility functions by backpropagation is impossible due to the presence of environment stochasticity. The novelty of RAPTOR lies in leveraging reparameterization of the state distribution, leading to a unique distributional perspective of end-to-end planning where the return distribution is utilized for sampling as well as optimizing risk-aware objectives by backpropagation in a unified framework. We evaluate and compare RAPTOR on three highly stochastic MDPs, including nonlinear navigation, HVAC control, and linear reservoir control, demonstrating the ability of RAPTOR to manage risk in complex continuous domains according to different notions of risk-sensitive utility.