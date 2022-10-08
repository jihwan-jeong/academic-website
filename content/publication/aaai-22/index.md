---
title: 'A Distributional Framework for Risk-Sensitive End-to-End Planning in Continuous MDPs'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Noah Patton
  - Jihwan Jeong
  - Mike Gimelfarb
  - Scott Sanner

# Author notes (optional)
author_notes:
  - 'Equal contribution'
  - 'Equal contribution'
  - 'Equal contribution'

date: '2022-06-28T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2017-07-17T00:00:00Z'

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['1']

# Publication name and optional abbreviated publication name.
publication: _Proceedings of the AAAI Conference on Artificial Intelligence, 36(9)_
publication_short: In *AAAI-22*

abstract: Recent advances in efficient planning in deterministic or stochastic high-dimensional domains with continuous action spaces leverage backpropagation through a model of the environment to directly optimize action sequences. However, existing methods typically do not take risk into account when optimizing in stochastic domains, which can be incorporated efficiently in MDPs by optimizing a nonlinear utility function of the return distribution. We bridge this gap by introducing Risk-Aware Planning using PyTorch (RAPTOR), a novel unified framework for risk-sensitive planning through end-to-end optimization of commonly-studied risk-sensitive utility functions such as entropic utility, mean-variance optimization and CVaR. A key technical difficulty of our approach is that direct optimization of general risk-sensitive utility functions by backpropagation is impossible due to the presence of environment stochasticity. The novelty of RAPTOR lies in leveraging reparameterization of the state distribution, leading to a unique distributional perspective of end-to-end planning where the return distribution is utilized for sampling as well as optimizing risk-aware objectives by backpropagation in a unified framework. We evaluate and compare RAPTOR on three highly stochastic MDPs, including nonlinear navigation, HVAC control, and linear reservoir control, demonstrating the ability of RAPTOR to manage risk in complex continuous domains according to different notions of risk-sensitive utility.

# Summary. An optional shortened abstract.
summary: End-to-end planning framework for risk-sensitive planning under stochastic environments by backpropagating through a model of the environment.  The core idea is to use reparameterization of the state distribution, leading to a unique distributional perspective of end-to-end planning where the return distribution is utilized for sampling as well as optimizing risk-aware objectives by backpropagation in a unified framework.

tags:
  - Risk-sensitive planning
  - Reparameterization trick
  - End-to-end planning

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://ssanner.github.io/papers/aaai22_raptor.pdf'
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: 'https://aaai-2022.virtualchair.net/poster_aaai10867'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: RAPTOR
  focal_point: ''
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
  - raptor

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: '' # example
---

<!-- {{% callout note %}}
Click the _Cite_ button above to demo the feature to enable visitors to import publication metadata into their reference management software.
{{% /callout %}}

{{% callout note %}}
Create your slides in Markdown - click the _Slides_ button to check out the example.
{{% /callout %}}

Supplementary notes can be added here, including [code, math, and images](https://wowchemy.com/docs/writing-markdown-latex/). -->
