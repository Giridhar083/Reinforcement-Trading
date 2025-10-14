# Reinforcement Trading
This project implements a Deep Q-Network (DQN), a reinforcement learning algorithm, to train an agent for automated stock trading. The agent learns to make decisions—buy, sell, or hold—based on historical stock price data with the goal of maximizing its portfolio value over time.

### 📊 Project Overview
The core of this project is a custom trading environment built to simulate stock market interactions. A reinforcement learning agent, specifically a DQNAgent, is trained within this environment. The agent's objective is to develop a profitable trading strategy by learning from the consequences of its actions.

### How It Works
Environment: A TradingEnv class simulates the stock trading environment. It manages the agent's portfolio, tracks the stock price, and calculates the reward for each action taken.

Agent: A DQNAgent is created using a deep neural network (built with TensorFlow/Keras). This agent is responsible for deciding the optimal action at each step.

Training: The agent is trained over a specified number of episodes. In each episode, it interacts with the trading environment, and its neural network is updated through a process of experience replay to learn a Q-function, which estimates the value of taking a certain action in a given state.

Evaluation: After training, the agent's performance is evaluated on a separate test dataset to see how well it can trade on unseen data. The portfolio value over time is plotted to visualize the agent's profitability.

### 🛠️ Technologies & Libraries Used
This project is built using Python and relies on the following libraries:

TensorFlow & Keras: For building and training the deep neural network that powers the DQN agent.

NumPy: For numerical operations and data manipulation.

Pandas: For handling and processing the time-series stock data.

Matplotlib: For plotting the agent's performance and visualizing the portfolio value.

tqdm: For displaying progress bars during the training loop.
