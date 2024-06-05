---
title: "Reinforcement learning-based multi-objective control of grid-connected wind farms"
collection: publications
permalink: /publication/2009-10-01-paper-title-number-1
excerpt: 'Reinforcement learning; Wind Farm Control'
date: 2024-2-14
venue: 'IEEE Transactions on Industrial Informatics'
paperurl: 'https://ieeexplore.ieee.org/abstract/document/10436393'
citation: 'Huang Y, Zhao X. Reinforcement Learning-Based Multiobjective Control of Grid-Connected Wind Farms[J]. IEEE Transactions on Industrial Informatics, 2024.'
---
This article aims to design a multiobjective controller with a primary focus on mitigating the wake interference in wind farms to increase their long-term power generation compared with the method without coordination in tackling the wake effect. What is more, this farm-level controller endeavors to keep turbines online in the event of a voltage fault and offer ancillary services to the grid while minimizing the farm power losses. Model-free reinforcement learning (RL) is promising in coping with such challenges since it can train a multiobjective control policy by interacting with the environment. In this article, we first construct a grid-connected wind farm simulator as the environment to collect training samples for model-free RL. Then, we erect three wind farm control objectives: maximizing the power generation of the wind farm by overcoming the wake effect, facilitating the fault-ride-through capability of wind turbines, and enhancing the frequency stability of the grid. Finally, an appropriate reward function is designed to induce RL agents to achieve these objectives. Results show that the proposed method can obviously increase the power generation compared with the method ignoring the wake effect. Furthermore, the method showcases it is capable of controlling turbines to ride through voltage faults of the grid and assisting the grid to return to its nominal frequency.

[Download paper here](https://ieeexplore.ieee.org/abstract/document/10436393)


If you are interested in this paper, please cite it as:
```
@article{huang2024reinforcement,
  title={Reinforcement Learning-Based Multiobjective Control of Grid-Connected Wind Farms},
  author={Huang, Yubo and Zhao, Xiaowei},
  journal={IEEE Transactions on Industrial Informatics},
  year={2024},
  publisher={IEEE}
}
```