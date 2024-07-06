# Reinforcement Learning Tic-Tac-Toe

A Python-based implementation of Tic-Tac-Toe using Q-learning, featuring both training and testing functionalities.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Directory Structure](#directory-structure)
- [Configuration](#configuration)
- [Contributing](#contributing)

## Introduction
This project demonstrates the use of Reinforcement Learning (RL) to play Tic-Tac-Toe. It employs Q-learning, a model-free RL algorithm, to train agents that can play against each other. Additionally, it allows for testing the trained model by playing against a human player.

## Features
- **Training**: Agents train against each other using Q-learning.
- **Testing**: Test the trained agents by playing against them.
- **Critical Location Detection**: Enhanced rewards for critical moves.
- **Graphical Interface**: Pygame for a visual representation of the game board.

## Installation

### Prerequisites
- Python 3.6+
- Pygame
- Numpy

### Steps
1. **Clone the repository**:
    ```bash
    git clone https://github.com/AayushChoudhary26/TicTacToe-Game-RL
    cd TicTacToe-Game-RL
    ```

2. **Create and activate a virtual environment (optional but recommended)**:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

3. **Install dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

### Training the Model
To train the RL agents, run the `train_model.py` script. You can adjust parameters such as the number of episodes, epsilon (exploration rate), alpha (learning rate), and gamma (discount factor).

```bash
python train_model.py
```

The trained Q-tables will be saved in the `agents` directory.

### Testing the Model
To test the trained RL agents against a human player, run the `test_model.py` script. Follow the on-screen prompts to choose your player and make moves.

```bash
python test_model.py
```

## Directory Structure

```
reinforcement-learning-tictactoe/
│
├── agents/
│   ├── agent1_q_table.pkl         # Q-table for agent 1
│   ├── agent2_q_table.pkl         # Q-table for agent 2
│
├── helper_classes/
│   ├── environment.py             # Tic-Tac-Toe environment class
│   ├── q_learner.py               # Q-learning agent class
│
├── train_model.py                 # Script to train the RL model
├── test_model.py                  # Script to test the RL model
├── requirements.txt               # Python dependencies
└── README.md                      # This README file
```

## Configuration
Modify the parameters in `train_model.py` and `test_model.py` to configure training and testing:
- **Epsilon**: Exploration rate for training.
- **Alpha**: Learning rate.
- **Gamma**: Discount factor.
- **Episodes**: Number of training episodes.

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request for review.

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a pull request
