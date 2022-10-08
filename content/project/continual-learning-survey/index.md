---
title: Online Continual Learning in Image Classification&#58; An Empirical Survey
summary: 
tags:
- Continual Learning
date: "2021-10-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Types of Continual Learning Problems
  alt_text: ''
  focal_point: Smart

url_code: ''
url_pdf: https://arxiv.org/pdf/2101.10423.pdf
url_slides: ''
url_video: ''

slides: ""

profile: true

show_breadcrumb: true

# commentable: true
---

Online continual learning for image classification studies the problem of learning to classify images from an online stream of data and tasks, where tasks may include new classes (class incremental) or data nonstationarity (domain incremental). One of the key challenges of continual learning is to avoid catastrophic forgetting (CF), i.e., forgetting old tasks in the presence of more recent tasks. Over the past few years, a large range of methods and tricks have been introduced to address the continual learning problem, but many have not been fairly and systematically compared under a variety of realistic and practical settings. To better understand the relative advantages of various approaches and the settings where they work best, this survey aims to (1) compare state-of-the-art methods such as Maximally Interfered Retrieval (MIR), iCARL, and GDumb (a very strong baseline) and determine which works best at different memory and data settings as well as better understand the key source of CF; (2) determine if the best online class incremental methods are also competitive in the domain incremental setting; and (3) evaluate the performance of 7 simple but effective tricks such as the “review” trick and the nearest class mean (NCM) classifier to assess their relative impact. Regarding (1), we observe that iCaRL remains competitive when the memory buffer is small; GDumb outperforms many recently proposed methods in medium-size datasets and MIR performs the best in larger-scale datasets. For (2), we note that GDumb performs quite poorly while MIR — already competitive for (1) — is also strongly competitive in this very different (but important) continual learning setting. Overall, this allows us to conclude that MIR is overall a strong and versatile online continual learning method across a wide variety of settings. Finally for (3), we find that all tricks are beneficial, and when augmented with the “review” trick and NCM classifier, MIR produces performance levels that bring online continual learning much closer to its ultimate goal of matching offline training. Our codes are available at https://github.com/RaptorMai/online-continual-learning.