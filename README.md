# Slippery Random Maze Reinforcement Learning Project


## Demo

Below is a demonstration of the project in action:

![Slippery Maze Demo](https://github.com/dancher00/Slippery-Random-Maze/blob/main/demo_maze.gif)


This project is a minimal environment designed for experimenting with reinforcement learning algorithms. The environment is a grid-based maze where the agent experiences "slippery" dynamics: intended moves have an 85% chance of success and a 15% chance of moving to a random adjacent unblocked cell.

## Table of Contents
- [Overview](#overview)
- [Demo](#demo)
- [Features](#features)
- [Installation and Usage](#installation-and-usage)
- [License](#license)

## Overview

The Slippery Random Maze project simulates a grid-based maze environment where an agent attempts to navigate from a starting position to a goal while encountering stochastic dynamics. The agent can move up, down, left, right, or stay in place. The movement action succeeds with an 85% probability if the target cell is not blocked; otherwise, the remaining 15% is equally distributed among other available adjacent cells.

## Features

- **Grid-based Maze:** Dynamic maze with random blocked cells.
- **Stochastic Dynamics:** Moves have a chance to deviate from the intended direction.
- **Visual Interface:** Rendered using Pygame.
- **Modular Design:** Components for environment, controller, drawer, and state.
- **Extendable:** Easy to integrate with reinforcement learning algorithms.

## Installation and Usage

**Clone the repository:**

```
git clone https://github.com/dancher00/Slippery-Random-Maze.git
cd Slippery-Random-Maze
```

Use docker
```
docker build --no-cache -t randommaze .

./run.sh q_learning
./run.sh value_iteration
./run.sh policy_iteration
```
## Results

![PI_train](https://github.com/dancher00/Slippery-Random-Maze/blob/main/results/policy-iteration/training.png)

![VI_train](https://github.com/dancher00/Slippery-Random-Maze/blob/main/results/value-iteration/training.png)

![Q_train](https://github.com/dancher00/Slippery-Random-Maze/blob/main/results/q-learning/training.png)


## License
This project is licensed under the MIT License.
