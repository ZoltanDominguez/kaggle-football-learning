# Google Research Football
## Train agents to master the world's most popular sport

We are creating a machine learning model with reinforcement learning techniques to play in Google Football environment.
There is a kaggle competition at this time, we are submitting our most successful model there too.

This paper by Google Research describes the environment. Also it provides benchmark results for three stateof-the-art reinforcement learning algorithms. Two of them are popular policy gradient methods (PPO, IMPALA) and one is a modern DQN implementation (Ape-X DQN).

1. PPO (Schulman et al., 2017, https://arxiv.org/pdf/1707.06347.pdf)
1. IMPALA (Espeholt et al., 2018, https://arxiv.org/pdf/1802.01561.pdf)
1. Ape-X DQN (Horgan et al., 2018, https://arxiv.org/pdf/1803.00933.pdf)

The paper by Google Researchby Google Research: https://arxiv.org/pdf/1907.11180.pdf



### Environment
The Football Engine is out of the box compatible with OpenAI Gym API, so any approaches used on OpenAI Gym projects will be useful for this special problem too.

The state representation is described in the paper, but here is a clear explanation as well:
https://towardsdatascience.com/google-football-environment-installation-and-training-rl-agent-using-a3c-d058a44f0fad

One representation we are planning to use is Super Mini Map (SMM) representation. It is visualized by many competitors, here is an example:

![Kaggle_SMM](pics/Kaggle_SMM.png)

### Action set
The environment supports 19 actions listed here:
![Action_set](pics/action_set.png)

### Reward function
One very straightforward reward function is the goal score.


### Reinforcement learning
Reinforcement learning articles listed that seems to cover most of the topic:
https://medium.com/@jonathan_hui/rl-deep-reinforcement-learning-series-833319a95530


# Information for testing and training further.
Current best model weights can be loaded from the repo. (you can found it at the res/weights folder)
The gfootbal_colab notebook consists the training and evaluating code as well. The notebook runs in Google Colaboratory on CPU and on GPU as well.

The notebook contains code if you only want to replay the evaluation or if you want to train the model further. The model may also need some optimizations.

# Relevant Papers:
DQN Playing Atari with Deep Reinforcement Learning:
https://arxiv.org/pdf/1312.5602.pdf
Human-level control through deep reinforcement
learning
http://files.davidqiu.com//research/nature14236.pdf
---
Rainbow: Combining Improvements in Deep Reinforcement Learning:
Matteo Hessel, Joseph Modayil, Hado van Hasselt, Tom Schaul, Georg Ostrovski, Will Dabney, Dan Horgan, Bilal Piot, Mohammad Azar, David Silver
https://arxiv.org/abs/1710.02298
---
PRIORITIZED EXPERIENCE REPLAY
Tom Schaul, John Quan, Ioannis Antonoglou and David Silver
Google DeepMind
https://arxiv.org/pdf/1511.05952.pdf

# Information about us needed for Deep Learning Class at BME:
### Team Name 
SoccerPunch
### Team Members:
Dominguez Zoltán (DQN methods)
Koszticza Marcell Lőrinc (IMPALA methods)
Kovács Máté Barnabás (PPO methods)