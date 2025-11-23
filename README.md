# Price-Elasticity-Model-for-Cryptocurrencies

* This repository includes the simulation done for the paper: Optimal mining in proof-of-work blockchain protocols. The full version of the paper can be find in here: https://www.sciencedirect.com/science/article/pii/S1544612322007863

**Files:**

- **main_simulation.ipynb:** This is the main simulation of the paper, in which we used a simple Q-learning algorithm to model a number of miners who participate in the mining activity. Agents are naive in the way that they have no information in the beginning but by playing the game for a sufficient number of times, their strategies converge to the equilibrium. 

- **neural_network_simulation:** Simulating the same game but now we used RLlib framework (https://docs.ray.io/en/latest/rllib/index.html). This is an advanced framework enabling the use of many agents with values drawn from continuous distributions. The main motivation to use this framework is to have a more accurate model and also indicate that the errors observed in the previous version (q-learning) were due to the restrictions of the q-learning model.

- **parametrization.ipynb:** It is a script created to address one of the reviewer comments regarding the stability of the results for a range of the parameters.
