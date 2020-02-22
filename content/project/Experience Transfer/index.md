---
title: Experience Transfer 
summary: Framework to teach higher-dim student using experiences of a teacher.

tags:
- Reinforcement Learning
- Deep Learning
date: "2020-01-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).

image:
  caption: Picture from Reinforcement Learning - An Introduction
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
•Aimed to transfer the experience of a teacher agent, receiving higher and lower dimensional observations to train student-agent, receiving only higher dimensional observations.

### Abstract
Learning directly from higher dimensional data like video stream is known to be a difficult problem to tackle in Reinforcement Learning. Learning directly from higher dimensional data can also be very time consuming. Imitation learning can be used in such cases to avoid random policy initializations. However, to use imitation learning, one needs to generate experience from an (expert) agent. A human (expert) agent generating these experience, needs to follow a set of ground rules to stick to the IID-data assumption needed to ensure stability in training. \
One method to avoid the cumbersome process of setting the ground rules, could be to use an (expert) agent, trained on lower dimensional observations. Training on lower dimensional data is known to be computationally efficient and less time consuming<!--[Citation needed] -->. The experience of this trained agent can hence be used to train the higher dimensional agent.
