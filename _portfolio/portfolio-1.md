---
title: "Safe robot manipulation using monitoring and recovery strategies"
excerpt: " Trained a reinforcement learning model for a robotic arm to reach door handles in simulation and successfully transferred it to real-world. Developed a self-supervised learning-based anomaly detection model to monitor irregularities and implemented recovery steps.<br/><img src='/images/rl.gif'>"
collection: portfolio
---
### Abstract

### Paper submitted to ICRA 2025 ([Code](https://github.com/bharathsanthanam94/robust-robot-policy-execution))

Reinforcement learning models trained for robot manipulation tasks often struggle with reliability when deployed in real-world environments. This challenge arises because these models are trained in simulations and then transferred to the real world. The complexities of real-world scenarios present adaptability issues for the model, leading to suboptimal task performance when deployed on actual robots. To address this limitation, we developed an anomaly detection model designed to identify irregularities during deployment and execute appropriate recovery steps.


### Key steps

- Train a reinforcement learning model to reach the door in simulation, and transfer to the real world
- Train an anomaly detection model using deep learning techniques that detects any variation from the normal scene as anomalies
- Once anomalies are detected, ensure safety by stopping the robot arm and execute recovery motion

### Concepts

Reinforcement learning, self supervised learning and Gaussian mixture models.

### Tools and Packages

Pytorch, lightning, pybullet, openai gym, stable-baselines3, ROS
