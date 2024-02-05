# CCDM2
This repository is for creating a Careful and Competent Driver Model for Merging (CCDM2) scenarios for safety assessment of autonomous vehicles. We combined Monte Carlo Tree Search (MCTS) with Model Predictive Control (MPC) to create a risk-aware, capability-dominant and interpretable driver model. 

## Description
1, The extracted challenging merging scenarios under `\xosc` from the [ExiD](https://levelxdata.com/exid-dataset/) dataset are stored with OpenScenario format, which can be loaded by commonly used simulators, such as esmini. The extracted scenarios with the same format as ExitD are stored under `\scenarios\data`.

2, The map is stored under `\scenarios\maps` with OpenDrive format. We recreated the original map to fix some bugs.

3, The simulation results are under `\output`, where you can find the merging process of different models. If you want to visualize the results, please install [esmini](https://esmini.github.io/) first, then typing
`./bin/replayer --window 60 60 800 400 --file sim.dat`.


### Results Demonstration
|Scenario id | Bare                                                                                                    | CCDM2                                                                                                 |
| ------- | -------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | 
|84_285| <img src="https://github.com/ChengWang2018/CCDM2/blob/main/output/videos/bare/84_285_scenario.gif" width="400" height="88">  | <img src="https://github.com/ChengWang2018/CCDM2/blob/main/output/videos/ccdm2/84_285_scenario.gif" width="400" height="88">  |
|86_770| <img src="https://github.com/ChengWang2018/CCDM2/blob/main/output/videos/bare/86_770_scenario.gif" width="400" height="88">  | <img src="https://github.com/ChengWang2018/CCDM2/blob/main/output/videos/ccdm2/86_770_scenario.gif" width="400" height="88">  |
|86_1640| <img src="https://github.com/ChengWang2018/CCDM2/blob/main/output/videos/bare/86_1640_scenario.gif" width="400" height="88"> | <img src="https://github.com/ChengWang2018/CCDM2/blob/main/output/videos/ccdm2/86_1640_scenario.gif" width="400" height="88"> |
|91_623| <img src="https://github.com/ChengWang2018/CCDM2/blob/main/output/videos/bare/91_623_scenario.gif" width="400" height="88">  | <img src="https://github.com/ChengWang2018/CCDM2/blob/main/output/videos/ccdm2/91_623_scenario.gif" width="400" height="88">  |




