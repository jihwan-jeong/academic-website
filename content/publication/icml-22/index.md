---
title: 'An Exact Symbolic Reduction of Linear Smart Predict+Optimize to Mixed Integer Linear Programming'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Jihwan Jeong
  - Parth Jaggi
  - Andrew Butler
  - Scott Sanner

# Author notes (optional)
# author_notes:
#   - 'Equal contribution'
#   - 'Equal contribution'

date: '2022-07-27T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2022-07-17T00:00:00Z'

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['1']

# Publication name and optional abbreviated publication name.
publication: In *Proceedings of the 39th International Conference on Machine Learning (ICML-22), Baltimore, USA, 2022*
publication_short: In *ICML-22*

abstract: Predictive models are traditionally optimized independently of their use in downstream decision-based optimization. The **`smart, predict then optimize' (SPO)** framework addresses this shortcoming by optimizing predictive models in order to **_minimize_** the final downstream decision loss.  To date, several local first-order methods and convex approximations have been proposed. These methods have proven to be effective in practice, however, it remains generally unclear as to how close these local solutions are to global optimality. In this paper, we cast the SPO problem as a bi-level program and apply Symbolic Variable Elimination (SVE) to analytically solve the lower optimization.  The resulting program can then be formulated as a mixed-integer linear program (MILP) which is solved to global optimality using standard off-the-shelf solvers. To our knowledge, our framework is the first to provide a globally optimal solution to the linear SPO problem. Experimental results comparing with state-of-the-art local SPO solvers show that the globally optimal solution obtains up to **two orders of magnitude reduction** in decision regret. 

# Summary. An optional shortened abstract.
summary: The Smart Predict+Optimize (SPO) framework tries to solve a decision-making problem expressed as mathematical optimization in which some coefficients have to be _estimated_ by a predictive model.  The challenge is that this problem is non-convex and non-differentiable, even for linear programs with linear predictive models.  Despite that, we provide the first exact optimal solution to the SPO problem by formulating it as a bi-level bi-linear program and reducing it to a mixed-integer linear program (MILP) using a novel symbolic method.

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://ssanner.github.io/papers/icml22_emspo.pdf'
url_code: 'https://github.com/jihwan-jeong/xaddpy'
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: 'https://slideslive.com/38983358'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: (Left) True SPO loss is piece-wise linear (Right) Convex surrogate SPO+ loss
  focal_point: ''
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
  - emspo

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
