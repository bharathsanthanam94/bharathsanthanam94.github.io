---
title: "Safe robot manipulation using monitoring and recovery strategies"
excerpt: " Trained a reinforcement learning model for a robotic arm to reach door handles in simulation and successfully transferred it to real-world. Developed a self-supervised learning-based anomaly detection model to monitor irregularities and implemented recovery steps.<br/><img src='/images/rl.gif'>"
collection: portfolio
---
### Abstract

### Paper submitted to ICRA 2025 ([Code](https://github.com/bharathsanthanam94/robust-robot-policy-execution))

Learned robot policies have consistently been shown to be quite versatile, but they typically have no built-in mechanism for handling the full complexity of open environments, which makes them prone to execution failures; this implies that simply deploying policies without the ability to recognize and react to failures may lead to unreliable and unsafe robot behaviour. In this paper, we present a framework that couples a learned policy with a method to detect visual anomalies during policy deployment and to perform recovery behaviours when necessary, thereby aiming to prevent failures. Specifically, we first train a policy in simulation and then execute it in the real world to collect data from nominal task executions, based on which we train an anomaly detection model. This model is then integrated into the online policy execution process so that deviations from the nominal execution can be recognized. Detected anomalies trigger a three-level sequential recovery process that consists of (i) pausing the execution temporarily, (ii) performing a local perturbation of the robot’s state before continuing the execution, and (iii) resetting the robot to a safe state by sampling from a learned execution success model. We verify our proposed method on a door handle reaching task with a Kinova Gen3 arm, such that our results show that integrating policy execution with anomaly detection and recovery increases the execution success rate in environments with various anomalies, such as trajectory deviations and adversarial human interventions.


### Key steps

- Train a reinforcement learning model to reach the door in simulation, and transfer to the real world
- Train an anomaly detection model using deep learning techniques that detects any variation from the normal scene as anomalies
- Once anomalies are detected, ensure safety by stopping the robot arm and execute recovery motion

### Concepts

Reinforcement learning, self supervised learning and Gaussian mixture models.

### Tools and Packages

Pytorch, lightning, pybullet, openai gym, stable-baselines3, ROS
