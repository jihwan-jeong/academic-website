---
title: An Exact Symbolic Reduction of Linear Smart Predict+Optimize to Mixed Integer Linear Programming (ICML-22)
summary: The Smart Predict+Optimize (SPO) framework tries to solve a decision-making problem expressed as mathematical optimization in which some coefficients have to be _estimated_ by a predictive model.  The challenge is that this problem is non-convex and non-differentiable, even for linear programs with linear predictive models.  Despite that, we provide the first exact optimal solution to the SPO problem by formulating it as a bi-level bi-linear program and reducing it to a mixed-integer linear program (MILP) using a novel symbolic method.
tags:
  - SPO
date: '2022-07-27T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: (Left) True SPO loss is piece-wise linear (Right) Convex surrogate SPO+ loss
  focal_point: Smart

# links:
#   - icon: book
#     icon_pack: fa
#     name: Paper
#     url: https://ssanner.github.io/papers/icml22_emspo.pdf
url_code: 'https://github.com/jihwan-jeong/xaddpy'
url_pdf: 'https://ssanner.github.io/papers/icml22_emspo.pdf'
url_slides: ''
url_video: https://slideslive.com/38983358

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: '' #example
---

Predictive models are traditionally optimized independently of their use in downstream decision-based optimization. The **`smart, predict then optimize' (SPO)** framework addresses this shortcoming by optimizing predictive models in order to **_minimize_** the final downstream decision loss.  To date, several local first-order methods and convex approximations have been proposed. These methods have proven to be effective in practice, however, it remains generally unclear as to how close these local solutions are to global optimality. In this paper, we cast the SPO problem as a bi-level program and apply Symbolic Variable Elimination (SVE) to analytically solve the lower optimization.  The resulting program can then be formulated as a mixed-integer linear program (MILP) which is solved to global optimality using standard off-the-shelf solvers. To our knowledge, our framework is the first to provide a globally optimal solution to the linear SPO problem. Experimental results comparing with state-of-the-art local SPO solvers show that the globally optimal solution obtains up to **two orders of magnitude reduction** in decision regret. 