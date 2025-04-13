# Deep-Q-Network-DQN-Atari-Pong-Agent
# 🕹️ Deep Q-Network (DQN) Atari Pong Agent

This project implements a Deep Q-Network (DQN) agent using **PyTorch** and **OpenAI Gym** to play the classic Atari game **PongNoFrameskip-v4**. The agent learns from raw pixel input using deep reinforcement learning techniques.

---

## 📌 Features

- Convolutional neural network (CNN) based Q-network
- Experience Replay Buffer for stable learning
- Epsilon-greedy exploration strategy
- Frame stacking with Gym wrappers
- Model saving and training reward visualization
- Evaluation using trained agent

---

## 📄 Based on Research

This implementation is inspired by the DeepMind paper:

> **"Playing Atari with Deep Reinforcement Learning"**  
> *Volodymyr Mnih, Koray Kavukcuoglu, David Silver, et al. (2013)*  
> [Read the paper on arXiv](https://arxiv.org/abs/1312.5602)

> 📌 Key techniques from the paper used in this repo:
> - Training a CNN directly from raw Atari frames
> - Using **Q-learning with experience replay**
> - Stacking 4 grayscale frames as input
> - Reward clipping for stable training
> - Frame skipping and action repeats

---

## 🧠 Algorithm Overview

The agent uses a deep convolutional Q-network that:
1. Receives an input of 4 stacked grayscale 84x84 frames
2. Predicts Q-values for all valid actions in a single forward pass
3. Updates Q-values using the Bellman equation and stochastic gradient descent
4. Trains off-policy using experience replay

---


