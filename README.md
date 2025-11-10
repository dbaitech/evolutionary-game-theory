# Evolutionary Game Theory
Biological populations evolve under pressure from a combination of factors: random genetic mutations, unpredictable environmental disturbance and interactions between each other. Natural selection can be abstracted into the idea of there being strategies 'chosen' by evolutionary agents. These strategies consist of the selection of certain genetic mutations that arise in the population over time and they have the underlying goal of maximizing their own fitness in preserving the proportion of stable phenotypes in the population.

In the paper *Stochastic noncooperative and cooperative evolutionary game strategies of a population of biological networks under natural selection, Biosystems* by Chen et al., this is modelled as both non-cooperative and co-operative evolutionary games. In this repository, I focus on the non-cooperative case.

I also have an implementation of the original replicator equation [in this file](https://github.com/dbaitech/evolutionary-game-theory/blob/main/replicator_equation.ipynb).

I look at modeling the rate of change of different species in a population which will then be used to demonstrate how effective certain strategies are, meaning how effectively they can counter disturbances and maintain a stable population state with minimal evolutionary effort.

## Nonlinear Evolutionary Biological Network
The mathematical model of a Nonlinear Evolutionary Biological Network takes into account the effects of the following on a biological network:
- nonlinear interactions between species
- genetic mutations that have occurred randomly up to a certain time
- random environmental disturbances

and will be used to demonstrate how robust chosen strategies are for how the population state evolves. Strategies of the population are constructed based on choosing genetic mutations that have occurred in the population so far. The effect of these strategies can be viewed by looking at how a population state $\dot{x}(t)$ changes through the following equation:

$$\dot{x}(t) = f(x) + \sum_{i=1}^m u_i(t) + \sum_{k=1}^{N(t)} f_k(t)p(t - t_k) + Bv(t)$$

For more theoretical details on how the code works, see [this description file](https://github.com/dbaitech/evolutionary-game-theory/blob/main/non-cooperative_evo_game_description.ipynb).

As the Jupyter notebook may take a while to open on GitHub, you can open it in Google Colab [![with this link](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/dbaitech/evolutionary-game-theory/blob/main/non-cooperative_evo_game_code.ipynb).
- Here is the file [in this repository](https://github.com/dbaitech/evolutionary-game-theory/blob/main/non-cooperative_evo_game_code.ipynb).

Note: the implementation is under development to fine-tune the initial inputs for more stable results.

# Source Paper
Bor-Sen Chen, Chin-Hsun Yeh,
Stochastic noncooperative and cooperative evolutionary game strategies of a population of biological networks under natural selection,
Biosystems,
Volume 162,
2017,
Pages 90-118,
ISSN 0303-2647,
https://doi.org/10.1016/j.biosystems.2017.08.001.
(https://www.sciencedirect.com/science/article/pii/S0303264717302927)
