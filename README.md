# Deep Q-Network (DQN) and Prioritized Experience Replay on Acrobot

[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.17-orange.svg)](https://www.tensorflow.org/)
[![Gymnasium](https://img.shields.io/badge/Gymnasium-1.0+-green.svg)](https://gymnasium.farama.org/)

## Overview

This repository implements and compares various Deep Reinforcement Learning algorithms on the **Acrobot-v1** environment from Gymnasium:

- **DQN** (Deep Q-Network)
- **DDQN** (Double Deep Q-Network)
- **DQN with PER** (Prioritized Experience Replay)
- **DDQN with PER**

The implementation includes a custom replay buffer, SumTree data structure for PER, and comprehensive training/validation pipelines.


## Results Summary

| Algorithm | Average Episodic Score (Validation) |
|-----------|-------------------------------------|
| DQN | -187.0 |
| DDQN | -105.8 |
| DQN w/ PER | **-85.2** |
| DDQN w/ PER | -200.0 |

**Best performing:** DQN with Prioritized Experience Replay achieved the highest average episodic score of **-85.2**.

## Training Performance

### Episode Rewards Comparison

The comparison shows that Prioritized Experience Replay significantly improves learning efficiency, with DQN+PER converging faster and achieving better final performance.

## Agent Behavior Videos

| Algorithm | GIF Visualization |
|-----------|-------------------|
| DQN | `gifs/agent_acro.gif` |
| DDQN | `gifs/agent_DDQN_acro.gif` |
| DQN w/ PER | `gifs/agent_DQN_PER_acro.gif` |
| DDQN w/ PER | `gifs/agent_DDQN_PER_acro.gif` |
