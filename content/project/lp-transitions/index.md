---
title: Symbolic Dynamic Programming for Continuous State MDPs with Linear Program Transitions (IJCAI-21)
summary: Recent advances in symbolic dynamic programming (SDP) have significantly broadened the class of MDPs for which exact closed-form value functions can be derived. However, no existing solution methods can solve complex discrete and continuous state MDPs where a linear program determines state transitions --- transitions that are often required in problems with underlying constrained flow dynamics arising in problems ranging from traffic signal control to telecommunications bandwidth planning. In this paper, we present a novel SDP solution method for MDPs with LP transitions and continuous piecewise linear dynamics by introducing a novel, fully symbolic **argmax** operator.
tags:
- Planning
date: "2021-07-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: ''
  focal_point: Smart

url_code: ''
url_pdf: 'https://www.ijcai.org/proceedings/2021/0562.pdf'
url_slides: 'https://ijcai-21.org/videos-slides/?video=768'
url_video: 'https://ijcai-21.org/videos-slides/?video=768'

slides: ""

show_breadcrumb: true

profile: true
---

Recent advances in symbolic dynamic programming (SDP) have significantly broadened the class of MDPs for which exact closed-form value functions can be derived. However, no existing solution methods can solve complex discrete and continuous state MDPs where a linear program determines state transitions --- transitions that are often required in problems with underlying constrained flow dynamics arising in problems ranging from traffic signal control to telecommunications bandwidth planning. In this paper, we present a novel SDP solution method for MDPs with LP transitions and continuous piecewise linear dynamics by introducing a novel, fully symbolic **argmax** operator. On three diverse domains, we show the first automated exact closed-form SDP solution to these challenging problems and the significant advantages of our SDP approach over discretized approximations.