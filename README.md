# Traffic Signal Optimization using Reinforcement Learning [ Sumo ]

## Project Overview

This project aims to apply various Reinforcement Learning (RL) algorithms to optimize traffic signal timings in urban traffic networks. The main goal is to reduce vehicle waiting times and overall congestion by employing algorithms such as Q-learning, Deep Q-Networks (DQN), SARSA, Proximal Policy Optimization (PPO), and others within a simulated environment created using the **Simulation of Urban MObility (SUMO)** tool.

### Key Algorithms Implemented:
1. **Q-Learning**: A foundational model-free RL algorithm where agents learn the value of actions through a Q-table.
2. **Deep Q-Network (DQN)**: An extension of Q-learning that uses neural networks to approximate the Q-values for large state-action spaces.
3. **SARSA (State-Action-Reward-State-Action)**: An on-policy RL algorithm that updates the Q-values based on the action taken by the agent.
4. **Proximal Policy Optimization (PPO)**: A policy gradient method known for stability in training deep RL models.
5. **Stable Baselines 3 (SB3)**: A collection of reliable RL implementations that provide easy-to-use interfaces for algorithms such as DQN and PPO.
6. **Double SARSA**: A modification of SARSA to reduce overestimation bias and provide more stable Q-value updates.
7. **RESCO (Reinforcement Learning Benchmarks for Traffic Signal Control)**: A specialized benchmark for evaluating RL algorithms in traffic management.

### Simulation Environment:
- **SUMO (Simulation of Urban MObility)**: SUMO is used for creating a realistic simulation of traffic flow in urban areas. The agents (traffic signals) control the timing of lights at intersections based on real-time traffic data such as vehicle queue lengths and waiting times.
- **Traffic Network**: The environment assumes a grid-based urban traffic network, where intersections experience varying congestion levels. Traffic demand, including peak and off-peak hours, is generated using SUMO's vehicle flow tools.
### commands
- python experiments\\ql_single-intersection.py -gui -s 4000
- python experiments\\ql_2way-single-intersection.py -gui -s 4000
- python experiments\\dqn_2way-single-intersection.py -gui -s 4000
- python experiments\\sarsa_2way-single-intersection.py -gui -s 4000
- python experiments\\ql_4x4grid.py -gui -s 4000
- python experiments\\sb3_grid4x4.py -gui -s 4000
- python experiments\\ql_4x4grid_pz.py -gui -s 4000
- python experiments\\sarsa_double.py -gui -s 4000
- python experiments\\sarsa_resco.py -gui -s 4000

