# 📖 Reinforcement Learning Dictionary

**Difficulty:** ⭐ Beginner  
**Estimated Reading Time:** 10–15 minutes  
**Prerequisites:** None  
**Last Updated:** July 2026

---

# 📚 Introduction

This dictionary contains the most important Reinforcement Learning (RL) terms introduced throughout this module.

Use it as a quick reference while studying, working on projects, or preparing for interviews.

The terms are arranged in **alphabetical order** for easy lookup.

---

# A

## Action

A decision made by the **agent** based on the current state of the environment.

**Example:**

A robot chooses to move forward.

---

## Actor

The part of an **Actor-Critic** algorithm responsible for selecting actions.

**Example:**

In PPO, the actor decides which action to perform next.

---

## Actor-Critic

A family of Reinforcement Learning algorithms that combines:

- An **Actor**, which selects actions.
- A **Critic**, which evaluates those actions.

**Examples:**

- PPO
- A2C
- A3C

---

# C

## Continuous Control

A Reinforcement Learning problem where actions can take continuous values rather than a small set of fixed choices.

**Example:**

Controlling the steering angle of a self-driving car.

---

## Critic

The component of an Actor-Critic algorithm that evaluates the quality of actions and helps improve the policy.

---

## Cumulative Reward

The total reward an agent receives over time.

The objective of Reinforcement Learning is usually to maximize cumulative reward rather than immediate reward.

---

# D

## Deep Q-Network (DQN)

A Reinforcement Learning algorithm that combines **Q-Learning** with a **Neural Network** to estimate Q-values in large or complex environments.

---

# E

## Environment

Everything outside the agent.

The environment:

- Responds to actions.
- Provides rewards.
- Determines the next state.

**Example:**

A warehouse where a delivery robot operates.

---

## Episode

One complete learning session.

It begins with an initial state and ends when the task is completed or another stopping condition is reached.

---

## Exploration

Trying new actions to discover better strategies.

Exploration helps the agent gather new information about the environment.

---

## Exploitation

Choosing actions that the agent already believes will produce high rewards.

Exploitation uses existing knowledge to maximize performance.

---

# L

## Long-Term Reward

The total future reward expected from a sequence of actions.

Reinforcement Learning focuses on maximizing long-term rewards instead of only immediate rewards.

---

# M

## Model-Based Learning

A Reinforcement Learning approach where the agent uses or learns a model of the environment to predict future outcomes and plan actions.

---

## Model-Free Learning

A Reinforcement Learning approach where the agent learns directly through interaction with the environment without building a model.

---

# N

## Negative Reinforcement

Encouraging desirable behavior by **removing an unpleasant condition** after the correct action.

> **Note:** Negative Reinforcement is different from punishment.

---

# P

## Penalty

A negative reward given when the agent performs an undesirable action.

**Example:**

A robot receives a penalty for colliding with a wall.

---

## Policy

The strategy that tells the agent which action to choose in each state.

A policy improves over time as the agent gains experience.

---

## Policy Gradient

A family of Reinforcement Learning algorithms that directly learns and improves the policy instead of estimating action values.

---

## Positive Reinforcement

Encouraging desirable behavior by **adding a positive reward** after a successful action.

---

## PPO (Proximal Policy Optimization)

A popular Actor-Critic Reinforcement Learning algorithm known for stable and efficient policy updates.

It is widely used in robotics, autonomous systems, and industrial automation.

---

# Q

## Q-Learning

A Value-Based Reinforcement Learning algorithm that learns the expected future reward (Q-value) for each state-action pair.

---

## Q-Value

The estimated future reward for taking a specific action in a given state.

Higher Q-values indicate better expected long-term outcomes.

---

# R

## Reinforcement Learning (RL)

A type of Machine Learning in which an agent learns through interaction with an environment by receiving rewards or penalties.

The objective is to maximize long-term cumulative rewards.

---

## Reward

Feedback received from the environment after performing an action.

Rewards may be:

- Positive
- Negative (penalties)
- Zero

---

## Reward Function

A rule that defines how rewards and penalties are assigned to the agent's actions.

A well-designed reward function is essential for effective learning.

---

# S

## SARSA

A Value-Based Reinforcement Learning algorithm whose name stands for:

**State → Action → Reward → State → Action**

It updates its learning using the action that the agent actually takes next.

---

## Sequential Decision-Making

Making a series of decisions where each action influences future states and rewards.

This is one of the main types of problems Reinforcement Learning is designed to solve.

---

## Simulation

A virtual environment used to train and test Reinforcement Learning agents safely before real-world deployment.

---

## State

The current situation of the environment observed by the agent before taking an action.

**Example:**

A robot detects:

- Battery level
- Current location
- Nearby obstacles

Together, these observations form the current state.

---

# T

## Trial and Error

A learning process in which an agent improves by repeatedly trying actions, observing the results, and adjusting its behavior.

---

# V

## Value Function

A function that estimates how beneficial a state or state-action pair is based on expected future rewards.

---

## Value-Based Learning

A category of Reinforcement Learning algorithms that learns the value of actions before selecting the best one.

**Examples:**

- Q-Learning
- SARSA
- DQN

---

# W

## Workflow

The repeated Reinforcement Learning process:

```text
Observe State

↓

Choose Action

↓

Perform Action

↓

Receive Reward

↓

Learn

↓

Repeat
```

---

# 📋 Quick Reference Table

| Term | Short Definition |
|------|------------------|
| Action | Decision made by the agent |
| Actor | Selects actions |
| Actor-Critic | Combines an actor and a critic |
| Critic | Evaluates actions |
| Cumulative Reward | Total reward over time |
| DQN | Deep Learning version of Q-Learning |
| Environment | World where the agent operates |
| Episode | One complete learning session |
| Exploration | Trying new actions |
| Exploitation | Using known good actions |
| Model-Based Learning | Uses a model of the environment |
| Model-Free Learning | Learns from experience |
| Negative Reinforcement | Removes an unpleasant condition |
| Penalty | Negative reward |
| Policy | Decision-making strategy |
| Policy Gradient | Learns the policy directly |
| Positive Reinforcement | Adds a reward |
| PPO | Modern Actor-Critic algorithm |
| Q-Learning | Learns Q-values |
| Q-Value | Estimated future reward |
| Reinforcement Learning | Learning through interaction |
| Reward | Feedback after an action |
| Reward Function | Defines rewards and penalties |
| SARSA | Learns using the next action actually taken |
| Sequential Decision-Making | Decisions that affect future outcomes |
| Simulation | Virtual training environment |
| State | Current situation |
| Trial and Error | Learning through repeated attempts |
| Value Function | Estimates future usefulness |
| Value-Based Learning | Learns action values |
| Workflow | RL learning cycle |

---

# 🧠 Memory Tips

Remember the core Reinforcement Learning cycle:

```text
State

↓

Action

↓

Reward

↓

Learning

↓

Repeat
```

Remember the three main algorithm categories:

```text
Value-Based

↓

Policy-Based

↓

Actor-Critic
```

Remember the most common algorithms:

```text
Q-Learning

↓

SARSA

↓

DQN

↓

Policy Gradient

↓

PPO
```

---

# 🎯 Final Note

Congratulations! 🎉

You have completed the **Reinforcement Learning** module.

You now understand:

- The fundamentals of Reinforcement Learning
- How agents learn from rewards and penalties
- Key RL components
- Types of Reinforcement Learning
- Popular algorithms
- Real-world applications
- Advantages and limitations
- Interview preparation
- Quick revision and terminology

You are now ready to move on to the next major topic:

> **06 – Deep Learning**