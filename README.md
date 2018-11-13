# Banana Navigation Project for DRLND Udacity Nanodegree 
---
This is the first project in the Udacity Deep Reinforcement Learning Nanodegree. It requires students to develop and train a [Deep Q-Network (DQN)](https://deepmind.com/research/dqn/) model to collect yellow bananas in a simulator. 

This project is the first to be solved in the Udacity Deep Reinforcement Learning Nanodegree. It is based in an implementation of a [Deep Q-Network (DQN)](https://deepmind.com/research/dqn/) model.
The environment is modeled in Unity, and the task is to train an agent to collect yellow bananas (getting a reward of +1) and avoid non yellow ones (getting -1 reward) c:

## Project Details
The simulation contains a single agent that navigates a large environment.  At each time step, it has four actions at its disposal:
- `0` - walk forward 
- `1` - walk backward
- `2` - turn left
- `3` - turn right

The state space has `37` dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction.  A reward of `+1` is provided for collecting a yellow banana, and a reward of `-1` is provided for collecting a blue banana. 

The environment is considered solved when the average reward (over the last 100 episodes) is at least +13.

## Getting Started
See the instrucions here to set up your environment [instructions here](https://github.com/udacity/deep-reinforcement-learning#dependencies) 

It also requires [Unity ML-Agents](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Installation.md), [NumPy](http://www.numpy.org/) and [PyTorch](https://pytorch.org/) 


Get the environment matching your OS :

Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)


Use full path file reference for such environment. Note that Banana.app is already included in this repo, so it can be imported with: 
```
env = UnityEnvironment(file_name="Banana.app")
```

## Instructions
Then run the [`navigation_banana.ipynb`](https://github.com/doctorcorral/DRLND-p1-banana/blob/master/navigation_banana.ipynb) notebook using the drlnd kernel to train the DQN agent.

After trainig the model, parameters will be dumpt to `checkpoint.pth` and will be used by the trained agent.

