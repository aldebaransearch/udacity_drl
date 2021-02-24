[//]: # (Image References)

[image1]: https://github.com/aldebaransearch/udacity_drl/blob/main/yellow_bananas_step_800.gif "Trained Agent"

# Project 1: Navigation

### Introduction

In this project, we train a deep reinforcement learning agent to navigate a square world, while collecting yellow bananas and avoiding blue. square world.  

![Trained Agent][image1]

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana.  The video above shows an agent using double Q dueling networks trained for 800 episodes.  

### State and Action Space
The state space has 37 dimensions containing the agent's velocity, along with information about of objects surrounding the agent. The action space contains four discrete actions, corresponding to:
- **`0`** - move forward.
- **`1`** - move backward.
- **`2`** - turn left.
- **`3`** - turn right.

### Solution
The agent is considered successful in the current setting, if it reaches more than 13 points in average over 100 episodes. However, instead of stopping the agent at a score of 13, we let it run for 2000 episodes for different setups and use the score dynamics to compare different approaches to agent architecture. We shall see, that for a simple as well as a more complicated agent design, 800 episodes is enough for the agent to reach an average score of around 15 for 100 episodes.

### Getting Started
**`1`** Build a conda environment using the environment.yml file in this repository by running "conda env create -f environment.yml"

**`2`** Download the Unity environment from the links that matches your operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)
. Place the file in the project folder, and unzip it.

**`3`** Download the notebook Navigator.ipynb and the python file util.py.

### Training
Simply follow the instructions in the first half of the Navigator.ipynb notebook

### Check Solutions
To assess results from training, follow the instructions in the last half of the Navigator.ipynb notebook. 

If you want to examine precalculated solutions, download scores.csv, scores_dd.csv, checkpoint_800.pth and checkpoint_800_dueling_doubleq.pth and use them instead of your own training results.

### Important note for Linux users
Due to what seems to be a bug in the Unity environment running on Linux machines, the notebook kernel has to be restarted between different trainings or different model assessments.


