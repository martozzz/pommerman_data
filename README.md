# Overview
Data of [pommerman](https://github.com/YichenGong/Agent47Agent) game. 

In each time step of pommerman, each agent takes an action according to its observations, which essentially generates an *observation - action* pair (or *o-a* pair). Each round of the game gives a winner, and we record the winner's *o-a* pairs from the first step to the last step. Each data file includes 100 rounds.

# data format

## observation
Observations mean what are the situations around the agent in a certain range `w`. E.g., a certain observation when `w = 3` is shown as follows:


|:----:|:----:|:----:|
|    |wall|    |
|bomb|agent|wall|
|wall|    |    |

`w =3` gives 9 cells (and `w =5` gives 25 cells and so on). In each cell, the entity can be a bomb, a rigid wall etc. Please refer to [this page](https://github.com/MultiAgentLearning/playground/tree/master/pommerman#agent-observations) for a detailed description. 

## action
Actions mean what agent do according to its observations. Agents are allowed to move in four directions or lay a bomb. Please refer to [this page](https://github.com/MultiAgentLearning/playground/tree/master/pommerman#agent-observations) for a detailed description. 
