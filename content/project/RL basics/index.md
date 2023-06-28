---
title: Implementation of RL Algorithms
summary: Implementation of basic reinforcement learning algorithms.

tags:
- Reinforcement learning
- Deep learning

date: "2019-06-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
#external_link:

image:
  caption: Q-learning for solving block world
  focal_point: Smart

links:
- icon: github
  icon_pack: fab
  name: GitHub
  url: https://github.com/khush3/rl_algorithms
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""
---

### Abstract
Working on the [autonomous stair-climbing robot](https://khush3.github.io/publication/stair_climbing/) highlighted the limitations of behavior cloning. This realization motivated me to study reinforcement learning. Following are some of the results of my implementation of basic reinforcement learning algorithms form scratch using PyTorch, NumPy, and OpenCV.

### Implementated:
- [x] DQN
- [x] Vanilla Policy Gradient
- [x] PPO
- [ ] DDPG

### Results
#### Value and Policy Iteration
![](https://media.giphy.com/media/L05KQuhnujAW3QyIkG/giphy.gif)

|      Method      | Deterministic Frozen Lake | Stochastic Frozen Lake |
| :--------------: | :-----------------------: | :--------------------: |
| Value Iteration  |             7             |           8            |
| Policy Iteration |             7             |           3            |



#### Q-Learning
![](https://media.giphy.com/media/KyAYvfmKlabE1zC820/giphy.gif)

#### Deep Q-Learning
![](https://media.giphy.com/media/PlsqPhHU7KnB2AdmYa/giphy.gif)
