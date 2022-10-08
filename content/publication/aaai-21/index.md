---
title: 'Online Class-Incremental Continual Learning with Adversarial Shapley Value'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Dongsub Shim
  - Zheda Mai
  - Jihwan Jeong
  - Scott Sanner
  - Hyunwoo Kim
  - Jongseong Jang

# Author notes (optional)
author_notes:
  - 'Equal contribution'
  - 'Equal contribution'
  - 'Equal contribution'

date: '2021-05-18T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2017-07-17T00:00:00Z'

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['1']

# Publication name and optional abbreviated publication name.
publication: _Proceedings of the AAAI Conference on Artificial Intelligence, 35(11)_
publication_short: In *AAAI-21*

abstract: In this paper, we specifically focus on the online class-incremental setting where a model needs to learn new classes continually from an online data stream. To this end, we contribute a novel Adversarial Shapley value scoring method that scores memory data samples according to their ability to preserve latent decision boundaries for previously observed classes (to maintain learning stability and avoid forgetting) while interfering with latent decision boundaries of current classes being learned (to encourage plasticity and optimal learning of new class boundaries). Overall, we observe that our proposed ASER method provides competitive or improved performance compared to state-of-the-art replay-based continual learning methods on a variety of datasets.

# Summary. An optional shortened abstract.
summary: ''

tags:
  - Continual learning
  - Shapley value
  - Class-incremental learning

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://ssanner.github.io/papers/aaai21_aser.pdf'
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: 'https://slideslive.com/38949257/online-classincremental-continual-learning-with-adversarial-shapley-value?locale=de'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: ''
  focal_point: ''
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
  - aser

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
