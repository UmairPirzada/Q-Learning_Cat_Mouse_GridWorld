# Reinforcement Learning (RL), Q-Learning, QLearningAgent, and RLVisualizer

![image](https://github.com/user-attachments/assets/28861970-5105-4eb4-b635-ee92df4850d3)

### 1. Reinforcement Learning (RL):
Reinforcement Learning is a type of machine learning where an agent learns to make decisions by performing certain actions and receiving rewards or penalties in 

return. The goal of the agent is to learn a policy that maximizes cumulative reward over time. In RL, the agent interacts with an environment, observes its state, and

chooses actions that influence the environment's state.

### 2. Q-Learning:
Q-Learning is a popular RL algorithm that aims to learn the optimal policy for an agent. It is a model-free, off-policy algorithm, meaning it does not require a model

of the environment and can learn from actions that are outside the current policy. The algorithm uses a Q-table, where each entry represents the quality (Q-value) of 

a specific action taken from a specific state. The Q-values are updated iteratively based on the rewards received and the maximum expected future rewards.

3. QLearningAgent:
The QLearningAgent class represents an agent that uses the Q-Learning algorithm to learn optimal actions in the environment. Key components of this class include:

###Initialization:
Sets up the environment, Q-table, and parameters like learning rate, discount factor, and exploration rate (epsilon).
###choose_action:
Chooses an action based on the current state using an epsilon-greedy strategy, balancing exploration and exploitation.
update_q_table:
### Updates the Q-values in the Q-table based on the action taken, reward received, and the next state.
### train:
Runs multiple episodes to train the agent, updating the Q-table and tracking metrics like cumulative rewards and movement counts.

plot_training: Visualizes the training process by plotting cumulative rewards and movement counts over episodes.
### 4. RLVisualizer:
The RLVisualizer class is a Tkinter-based GUI application designed to visualize the agent's learning process in a GridWorld environment. Key features include:

# Grid Rendering: 
Displays the grid with the cat (agent), mouse (goal), and obstacles, updating in real-time as the agent moves.

Reward and Movement Count Display: Shows cumulative rewards and the number of movements made by the agent.
# Fullscreen Mode: 
The application starts in fullscreen, but users can exit fullscreen mode using the Escape key.

Image Handling: Utilizes images for visual representation of the agent, goal, and obstacles.

This class provides a visual representation of the agent's learning process, helping users to understand the agent's behavior and performance.

# Q-Learning Cat & Mouse GridWorld
### Overview
This project implements a simple reinforcement learning (RL) environment where a cat (agent) learns to reach a mouse (goal) in a grid world while avoiding obstacles. The learning algorithm used is Q-Learning, a popular RL technique. The project includes a visualizer built using Tkinter to display the agent's learning process and movement.

# Project Structure
GridWorldEnv: A custom environment representing the grid world where the cat (agent) and mouse (goal) are placed. The environment includes obstacles that the agent needs to avoid.

# QLearningAgent: 
A Q-Learning agent that learns to navigate the grid world. It maintains a Q-table to store the quality of actions taken from each state and updates this table based on the rewards received from the environment.

# RLVisualizer: 
A Tkinter-based GUI application that visualizes the agent's movements, the grid world, and key metrics like cumulative rewards and movement counts.

# Key Concepts
# Reinforcement Learning (RL)
RL is a type of machine learning where an agent learns to make decisions by interacting with an environment and receiving feedback in the form of rewards or penalties.

# Q-Learning
Q-Learning is an off-policy RL algorithm that aims to find the optimal action-selection policy. It uses a Q-table to store the expected rewards for taking each action from each state and updates the table based on the agent's experiences.

# QLearningAgent
This class implements the Q-Learning algorithm. Key functions include:

### choose_action:
Selects an action based on the current state using an epsilon-greedy strategy.
### update_q_table:
Updates the Q-table based on the observed reward and the next state.
### train: Runs multiple episodes to train the agent.
### plot_training:
Visualizes the training process with plots of cumulative rewards and movement counts.

 ![image](https://github.com/user-attachments/assets/02ac4dbc-3e60-4387-b53e-f14a3cf70aa1)


![image](https://github.com/user-attachments/assets/4699caf4-b5a7-4f79-9450-b8d4552c2520)


# RLVisualizer
A Tkinter application that visualizes the environment, including the agent, goal, and obstacles. It updates in real-time as the agent moves and displays key metrics.

# How to Run
Clone the Repository:
git clone https://github.com/UmairPirzada/Q-Learning_Cat_Mouse_GridWorld.git
 
# Install Dependencies:
Make sure you have the necessary Python packages installed:

pip install 

gym 

numpy 

pillow 

matplotlib

Run the Training and Visualization:


# Exit Fullscreen Mode:
The visualizer runs in fullscreen mode by default. Press the Escape key to exit fullscreen.

# Dependencies

### Python 3.6+

### Gym

### NumPy

### Pillow

### Matplotlib

### Tkinter (included with standard Python installations)

# Conclusion
The script combines reinforcement learning concepts with practical implementation to create a grid world environment where an agent learns to navigate towards a goal 

while avoiding obstacles. The Q-learning algorithm optimizes the agent's policy, and the Tkinter-based visualization provides an intuitive view of the agent's 

learning process.

# Contributing
Contributions are welcome! Please fork the repository and submit a pull request with your changes.

# Acknowledgements
OpenAI Gym for providing the RL environment framework.
The developers of the libraries used in this project.
# Contact
For questions or suggestions, please open an issue on GitHub or contact the project maintainer.
