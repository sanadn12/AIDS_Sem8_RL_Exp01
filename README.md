# 🚖 Experiment 1: Q-Learning using Taxi-v3 Environment

**Name:** Sanad Naqvi
**Roll No:** 221A023

---

## 🎯 Aim

To implement the **Q-Learning algorithm** using the Taxi-v3 environment and analyze the learning performance of an agent.

---

## 📌 Problem Statement

The objective is to train an agent to efficiently pick up and drop off passengers at designated locations in a grid-based environment using reinforcement learning.

---

## 📖 Theory

### 🔹 Reinforcement Learning

Reinforcement Learning (RL) is a type of machine learning where an agent learns to make decisions by performing actions and receiving rewards or penalties.

### 🔹 Q-Learning

Q-Learning is a **model-free reinforcement learning algorithm** that learns the value of an action in a particular state.

* It uses a **Q-table** to store values
* The agent selects actions that maximize expected rewards

### 🔹 Taxi-v3 Environment

* Provided by Gymnasium
* Grid world problem
* States: 500
* Actions: 6 possible moves
* Goal: Pick and drop passenger at correct location

---

## 🛠️ Implementation

### 🔹 Libraries Used

* gymnasium
* numpy
* random
* os

### 🔹 Steps

1. Installed and imported required libraries
2. Created Taxi-v3 environment
3. Initialized Q-table with zeros
4. Performed random actions to observe environment behavior
5. Applied Q-Learning update rule:

   ```
   Q(s, a) = Q(s, a) + α [r + max Q(s', a') - Q(s, a)]
   ```
6. Trained the agent for multiple episodes (2000)
7. Recorded rewards and performance

---

## 📊 Results

* Initial random performance:

  * Steps: 1171
  * Reward: -4768

* After training:

  * Rewards improved gradually
  * Agent learned better actions over episodes

*( screenshots & outputs added)*

---

## ✅ Conclusion

* The Q-Learning algorithm was successfully implemented.
* Initially, the agent performed poorly due to random actions.
* With training, the agent improved its performance by learning optimal policies.
* This experiment demonstrates how reinforcement learning can be used for decision-making problems.

---

## 📚 References

* Gymnasium Documentation
* Reinforcement Learning Basics
* Python NumPy Library

---

## 📦 requirements.txt

```
gymnasium
numpy
```
