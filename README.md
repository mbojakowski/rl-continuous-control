# rl-continuous-control

## Introduction

This repository contains an implementation of an Agent able to learn to control a double-jointed arm to target a given location.
The environment with which the Agent interacts in the Unity Reacher environment.

The implementation is based on a Deep Reinforcement Learning method (i.e. RL with neural networks).
More precisely, it is based on DDPG, and is partially inspired from a DDPG implementation used for another problem with a continuous action space: https://github.com/udacity/deep-reinforcement-learning/blob/master/ddpg-pendulum/model.py

## Environment

The environment state is a vector of 33 elements.
Actions are vectors of 4 real numbers between -1 and 1.

The problem is considered solved when the agent achieved a minimum average score of 30 over 100 consecutive episodes.

## Getting Started

The entry point is the Jupyter Notebook.
The given implementation was run from a Udacity workspace. Depending on your operation system, you would need to install the corresponding Unity environment and replace below line accordingly:

```
env = UnityEnvironment(file_name='/data/Reacher_One_Linux_NoVis/Reacher_One_Linux_NoVis.x86_64')
```

The [Getting Started](https://github.com/udacity/deep-reinforcement-learning/tree/master/p2_continuous-control#getting-started) section of the official repository contains up-to-date information regarding the installation of the environment for various operating systems.

Otherwise, all code cells need to be executed one after the other.
The first code cell installed all necessary dependencies, defined in the pip *requirements.txt* file.

## Report

A file *Report.pdf* explains the implementation and reports observations about the results.
