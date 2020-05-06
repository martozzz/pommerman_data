# Overview
Data of [pommerman](https://github.com/YichenGong/Agent47Agent) game. 

In each time step of pommerman, each agent takes an action according to its observations, which essentially generates an *observation - action* pair (or *o-a* pair). Each round of the game gives a winner, and we record the winner's *o-a* pairs from the first step to the last step. Each data file provided includes 100 rounds of games.

# data format

## observation
Observations mean what are the situations around the agent in a certain range `w`. E.g., a certain observation when `w = 3` is shown as follows:

|    |    |    |
|:----:|:----:|:----:|
|    |wall|    |
|bomb|**agent**|wall|
|wall|    |    |

In the data file provided, `ammo`, `blast_strength` and `can_kick` describe the states of the agent itself, and `Entity_0` -- `Entity_8 ` describe what are around the agent (the order of `Entity_0` -- `Entity_8` are from top-left to bottom-right in the $w \times w$ cells). Please refer to [this page](https://github.com/MultiAgentLearning/playground/tree/master/pommerman#agent-observations) for what the numbers mean.

## action
Actions mean what agent do according to its observations. Agents are allowed to move in four directions or lay a bomb. Please refer to [this page](https://github.com/MultiAgentLearning/playground/tree/master/pommerman#agent-observations) for the mapping between the numbers and actions. 
 
