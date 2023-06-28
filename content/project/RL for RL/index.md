---
title: RL on Latent Embeddings
summary: Framework to train agent using representation learning.

tags:
- Reinforcement learning
- Deep learning

date: "2020-01-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
#external_link:

image:
  caption: Picture form google.com
  focal_point: Smart

links:
- icon: github
  icon_pack: fab
  name: GitHub
  url: https://github.com/khush3/experience_transfer
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

---
Aimed at training Deep Q-Learning based agents on learned latent embeddings instead of higher dimensional image observations.

### Abstract
Learning directly from higher dimensional data like video stream is known to be a difficult problem to tackle in Reinforcement Learning. Learning directly from higher dimensional data can also be very time consuming. Representation learning can be used in such cases to leverage lower dimensional trained agents. The two-stage agent can be further be fine-tuned to adapt better using end-to-end training. This approach is also more robust to variations in environment due to the fact that agents are trained on learnt representations instead of directly training on the environment observations.