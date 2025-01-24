# Deep Q-Learning for Cart-Pole Game

This repository contains the implementation of a Deep Q-Learning (DQN) agent trained to play the Cart-Pole game using OpenAI Gym. The project demonstrates how reinforcement learning can be used to train an agent to balance a pole on a cart.

## Table of Contents
- [Introduction](#introduction)
- [Repository Structure](#repository-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Extending the Project](#extending-the-project)
- [References](#references)

## Introduction

The Cart-Pole problem is a classic reinforcement learning task where the goal is to balance a pole on a cart by moving the cart left or right. This project uses a Deep Q-Network (DQN) to train an agent to solve this problem. The DQN is a neural network that approximates the Q-value function, which is used to determine the best action to take in a given state.

## Repository Structure
```
Deep-Q-Learning-Cart-Pole/
├── README.md
├── notebooks/
│ ├── Q-learning-cart.ipynb
│ └── utils/
│ ├── memory.py
│ ├── q_network.py
│ └── visualization.py
├── assets/
│ ├── atari-network.png
│ ├── cart-pole.jpg
│ ├── deep-q-learning.png
│ ├── dqn-atari.pdf
│ └── q-network.png
├── checkpoints/
│ └── cartpole.ckpt
├── requirements.txt
└── nature14236.pdf
```


- **`notebooks/`**: Contains the Jupyter notebook for training and testing the DQN agent.
  - `Q-learning-cart.ipynb`: Main notebook for training and testing the agent.
  - `utils/`: Utility scripts for memory replay, Q-network, and visualization.
- **`assets/`**: Contains images and PDFs used in the project.
- **`checkpoints/`**: Saved model checkpoints.
- **`requirements.txt`**: List of Python dependencies.
- **`nature14236.pdf`**: Original DQN paper for reference.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Deep-Q-Learning-Cart-Pole.git
   cd Deep-Q-Learning-Cart-Pole
   ```
2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3. Install OpenAI Gym:
    ```bash
    pip install gym
    ```

## Usage
1. Open the Jupyter notebook:
```bash
jupyter notebook notebooks/Q-learning-cart.ipynb
```
2. Follow the steps in the notebook to:
- Train the DQN agent.
- Visualize the training progress.
- Test the trained agent.

3. To save and load model checkpoints:
- Checkpoints are saved in the checkpoints/ directory.
- Use the saver object in the notebook to save and restore the model.

Results
The trained agent achieves a high reward by balancing the pole for the maximum number of steps. The training progress is visualized using a rolling average of the rewards over episodes.

## References
- Playing Atari with Deep Reinforcement Learning

- OpenAI Gym Documentation
