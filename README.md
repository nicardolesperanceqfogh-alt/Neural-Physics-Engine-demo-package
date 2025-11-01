# Neural-Physics-Engine-demo-package
Neurophysical core — private. This repository contains a public showcase: a brief description of capabilities, an example (raw) dataset, and a demo video of the neurophysical core in action.

# What the system does

1) The system learns cause-and-effect relationships between agents and objects in the environment on the fly. When a scene is launched, it:

2) Receives observation strings (the state of the scene at time t),

3) Forms predictions of local steps/reactions in regression, which takes place as a sequence of small transformations,

4) When interacting (contact), it learns to predict the consequences of interaction and adjusts its future steps,

5) In interactive mode, it accepts an external goal and adapts the agent's behaviour in real time.




https://github.com/user-attachments/assets/adca4b92-ca3b-4fe1-b3bf-aca49b828799

# Important clarification

This is not Reinforcement Learning (RL) and does not involve learning through rewards or feedback from the environment. The system does not use policies, agents, or Q-functions. What it does is implement a full-fledged simulation of the environment, which the system has learned to reproduce based solely on observational data — a dataset with records of the position and orientation of all objects over time. In other words, instead of learning to act as in classical RL, the system: analyses real observations of the scene (recorded coordinates, angles, collisions), builds internal cause-and-effect patterns (what leads to what), and is then able to independently reproduce the behaviour of the environment: movement, interactions, reactions of objects and goals. This is closer to modelling physical causal relationships than to optimising agent behaviour. In essence, the core is a neurophysical engine that reconstructs the dynamics of the world from observations.

Unlike visually-driven world generation systems such as HunyuanWorld, this engine focuses on causal world dynamics — learning object interactions directly from observation, not from predefined physics equations.

# What should be included in this repository

1) README.md — high-level description (this file).

2) example_dataset.json — example dataset.

3) 2025-10-31 21-59-48.mp4 — short render recording: goal setting → agent movement → contact with object → object reaction.

Contact mail: caskinv2507@gmail.com
