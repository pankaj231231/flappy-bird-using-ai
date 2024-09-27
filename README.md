# FlapAI-Bird

This AI program implements several AI agents for playing Flappy Bird. The program applies reinforcement learning algorithms, including SARSA, Q-Learning, and Function Approximation, and Deep Q Networks. After training for 10,000 iterations, the agents regularly achieves high scores of 1400+, with the highest in-game score of 2069. 


## Installation

The project requires the following frameworks:

- Pygame: https://www.pygame.org



- OpenCV: https://opencv.org

## Train an Agent

The program implements the following agents.

- Baseline Agent.

```bash
python main.py --algo Baseline --probFlap 0.5
```

- SARSA Agent.

```bash
python main.py --algo SARSA --probFlap 0.1 --rounding 10 --lr 0.8
```

- Q-Learning Agent.

```bash
python main.py --algo QLearning --probFlap 0.1 --rounding 10 --lr 0.8 --order backward
```

- Function Approximation Agent with Linear Regression.

```bash
python main.py --algo FuncApproxLR --probFlap 0.1 --lr 0.1
```

- Function Approximation Agent with a Feed Forward Neural Network.

```bash
python main.py --algo FuncApproxDNN --probFlap 0.1 --lr 0.1
```

- Function Approximation Agent with Convolutional Neural Network.

```bash
python main.py --algo FuncApproxCNN --probFlap 0.1 --lr 0.1
```

