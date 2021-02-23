[//]: # (Image References)

[image1]: https://github.com/aldebaransearch/udacity_drl/blob/main/yellow_bananas_step_800.gif "Trained Agent"

# Project 1: Navigation

### Introduction

In this project, we train a deep reinforcement learning agent to navigate a square world, while collecting yellow bananas adn avoiding blue. square world.  

![Trained Agent][image1]

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana.  The video above shows an agent using double Q dueling networks agent trained for 800 episodes.  

### Stae and Action Space
The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction.  Given this information, the agent has to learn how to best select actions.  Four discrete actions are available, corresponding to:
- **`0`** - move forward.
- **`1`** - move backward.
- **`2`** - turn left.
- **`3`** - turn right.
