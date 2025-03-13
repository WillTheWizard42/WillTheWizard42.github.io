---
project_id: Multi-agents
---

#### Context

The goal of this project was to learn about OOP architecture and implementation with Java.

The project contains multiple simulations, each with varying complexity. The most interesting ones are as follow:

##### Game of life

This is a zero player game, determined entirely by its initial state. 

At every step of the simulation, each cell can be dead or alive. Any dead cell with three live neighbors will become alive on the next step. Any live cell with less than two or more than three live neighbors dies at the next step. All other cells remain unchanged from one step to the next.

Depending on the initial state of the simulation, it can die out completely or live on forever. In our model, we wrapped the edges of the simulated grid.

<video width="512" height="512" controls autoplay loop>
  <source src="/assets/videos/exampleConway.webm" type="video/webm">
Your browser does not support the video tag.
</video>

##### Model of segregation

This is a model developped by economist Thomas Schelling, it shows that people having even mild in-group preferences towards their own group can lead to a segregated society.

Each agent desires a certain fraction of their neighborhood (the 8 surrounding cells, ignoring empty ones) to be of the same group as themselves. We call that fraction *B<inf>a</inf>*. At every step of the simulation each agent checks if the current fraction of neighbors that matches their group *B* is more than *B<inf>a</inf>*. If not they will relocate to an empty spot where *B* $\geqslant$ *B<inf>a</inf>*.

Depending on the value chosen for *B<inf>a</inf>* the model can end with a completely segregated grid, or a fairly well balanced one.

<video width="512" height="512" controls autoplay loop>
  <source src="/assets/videos/exampleSchelling.webm" type="video/webm">
Your browser does not support the video tag.
</video>

##### Boids

This is a simulation of the flocking behavior of birds or fish, in our simulation we added predators to chase them.

Prey will try to steer to avoid local flockmates, align with the average heading of local flockmates, and move towards the center of mass of local flockmates.

Predators will try to chase the center of gravity of local flocks, accelerating into a chase when close enough.

<video width="512" height="512" controls autoplay loop>
  <source src="/assets/videos/exampleBoids.webm" type="video/webm">
Your browser does not support the video tag.
</video>

#### Links

- [Source code](https://gitlab.com/adamsw/multi-agents)
- [John Conway's game of life](https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life)
- [Thomas Schelling's model of segregation](https://en.wikipedia.org/wiki/Schelling%27s_model_of_segregation)
- [Craig Reynolds' boids](https://en.wikipedia.org/wiki/Boids)