# navigation_drlnd

This repository corresponds to the first project in Udacity's Deep Reinforcement Learning Nanodegree. The goal is to train and agent to navigate and collect/avoid bananas in a square space.

## The enviroment:

![env screenshot](https://github.com/lccrurod/navigation_drlnd/blob/main/screen%20intro%20enviroment.png)

It is based in a large square where the agent receives +1 reward for collecting a yellow banana and -1 for every blue one. Therefore the goal is to collect yellow bananas while avoiding blue bananas.

The enviroment state is given by the agents velocity, and the ray-based perception of the objects based on the agent's forward direction. The state has a total of 37 dimensions. Based on that information the agent must be able to determine which is the best action to excute, It can:

- `0` - move forward.
- `1` - move backwards.
- `2` - turn left.
- `3` - turn right.

When is the enviroment considered solved? - It is expected that the agent achieves an average of 13+ in 100 consecutive episodes in order to solve the enviroment.

## Getting Started:

This project is jumpstarted by the [Value-based-methods](https://github.com/udacity/Value-based-methods/blob/main/README.md) repository where in the `/python` folder are the necesary files for unity enviroments, and, Separately in the `Banana_Windows_x86_64` is located the specific enviroment for the project. The additional prerrequisites are specified in the `requirements.txt` file.

The files `model.py` and `dqn_agent.py` are based on the available content for the course for defining a Deep Q-Network and an trainable agent based on the network respectively.

The process of training the agent in done in the `AgentTraining.ipynb` notebook.
