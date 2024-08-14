---
title: "Safe robot manipulation using monitoring and recovery strategies"
excerpt: " Trained a reinforcement learning model for a robotic arm to reach door handles in simulation and successfully transferred it to real-world applications. Developed a self-supervised learning-based anomaly detection model to monitor irregularities and implemented recovery steps.<br/><img src='/images/example_RL2.jpg'>"
collection: portfolio

Note: We are currently writing a research paper for this work with an idea to publish, more details and the code will be shared soon.
---
#### Abstract

Reinforcement learning models trained for robot manipulation tasks often struggle with reliability when deployed in real-world environments. This challenge arises because these models are trained in simulations and then transferred to the real world. The complexities of real-world scenarios present adaptability issues for the model, leading to suboptimal task performance when deployed on actual robots. To address this limitation, we developed an anomaly detection model designed to identify irregularities during deployment and execute appropriate recovery steps.

#### Key steps:

- Train a reinforcement learning model to reach the door in simulation, and transfer to the real world
- Train an anomaly detection model using deep learning techniques that detects any variation from the normal scene as anomalies
- Once anomalies are detected, ensure safety by stopping the robot arm and execute recovery motion
