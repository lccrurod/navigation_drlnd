# Project Report

## Learning Algorithm
The method choosen for this challenge was Deep Q-Learning, which is based in the used of deep neural networks that map the input of the state of the enviroment to the possible actions. The implementation was the basic, as is in the original paper, and We'll see that It performed decently.
### Arquitecture
The neural network used is made of three fully connected layers:
 * **First Layer.** 37 (state dimensions) input - 64 output
 * **Second Layer.** 64 input - 64 output
 * **Third Layer.** 64 input - 4 (actions) output

### Parameters

- Initial Epsilon: 1
- Final Epsilon: 0.02
- Epsilon decay: 0.98

## Training Results

```
Episode 100	Average Score: 2.83
Episode 200	Average Score: 7.74
Episode 300	Average Score: 10.93
Episode 363	Average Score: 13.04
Environment solved in 263 episodes!	Average Score: 13.04
```
![results graph](https://github.com/lccrurod/navigation_drlnd/blob/main/results.png)

Also there is a video of the trained agent performing the collection task.

[<img src="https://github.com/lccrurod/navigation_drlnd/blob/main/thumbnail_trained_agent.png" width="272" height="151">](https://www.youtube.com/watch?v=KxZVNbaCfk8)

## Improvement Opportunities

The use of the vanilla implementation of the DQN algorithm although effective, It solved the enviroment relatively low number of episodes, leaves a lot of room for experimentation and refinement, some posible steps could be:
- Use dueling networks, as it grants a more robust estimation of Q-values.
- Add Prioritized Experience Replay, this could expand the value extracted from previous episodes and improve the agent.

Also, more of a style preference, could be to explore actions to reduce the jerkiness of the agent, such ass trying to avoid multiple turning in opposite directions.
