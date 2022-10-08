---
title: "Bayesian Optimization for a Multiple-Component System with Target Values"
authors:
- Jihwan Jeong
- Hayong Shin
# author_notes:
# - "Equal contribution"
# - "Equal contribution"
date: "2021-07-01T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "*Computers & Industrial Engineering*, 157"
publication_short: ""

abstract: Bayesian optimization (BO) that employs the Gaussian process (GP) as a surrogate model has recently gained much attention in optimization of expensive black-box functions. In BO, the number of experiments necessary to optimize a function can be considerably reduced by sequentially selecting next design points that are optimal with respect to some sampling criterion. However, little research has been done to address the optimization of a multiple-component system where each component has a certain target value to meet. In this paper, we aim to find an optimal design parameter in the sense that the response function is close to the target value for every component. To this end, the squared errors from the targets are aggregated to produce an objective function. Instead of modeling this objective using GP as in the standard BO formulation, we place the GP prior over the response function. As a result, the distribution over the objective function follows that of the weighted sum of non-central chi-squared random variables (WSNC) due to the inter-dependency between responses. When components of the system are changed, the standard BO suffers inefficiency; however, our formulation enables us to retain a learned model, resulting in better efficiency. We compare the rates of convergence of different BO methods and other black-box optimization baselines using several test functions. The performance of our model is comparable to the standard BO when there is no change in the system, but the superiority of our method becomes clear when changes in the components occur.

# Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags:
- Bayesian optimization
- Gaussian processes
- Expected improvement
featured: false

# links:
# - name: ""
#   url: ""
url_pdf: http://143.248.80.207/wordpress/wp-content/uploads/2021/04/Bayesian-optimization-for-a-multiple-component-system-with-target-values.pdf
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Illustration of BOMCT'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: '' #example
---

<!-- {{% callout note %}}
Click the *Cite* button above to demo the feature to enable visitors to import publication metadata into their reference management software.
{{% /callout %}}

{{% callout note %}}
Create your slides in Markdown - click the *Slides* button to check out the example.
{{% /callout %}}

Supplementary notes can be added here, including [code, math, and images](https://wowchemy.com/docs/writing-markdown-latex/). -->
