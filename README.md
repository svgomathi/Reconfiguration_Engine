# Reconfiguration_Engine- Overview

# Title: Distributed Multi-Agent Reinforcement Learning Enabled Approach for Optimizing Service Function Chain Reconfiguration in Edge-Cloud Continuum

# Author and Affiliation
**Gomathi Srinivasan Venkata**  
Graduate Institute of Artificial Intelligence, Chang Gung University,Taiwan

**Advisor:** Dr. Hojjat Baghban (Assistant Professor)  
Intelligent Cyber-Physical System Laboratory 

# Abstract
The emergence of the Edge-Cloud Continuum has transformed network service deployment by enhancing scalability,responsiveness, and resource utilization. Within this paradigm,Service Function Chains (SFCs) play a critical role in fulfilling the diverse requirements of latency-sensitive and compute-intensive applications. However, dynamic conditions, such as fluctuating resource availability, variable network service demands, and stringent Quality of Service (QoS) constraints, pose significant challenges to traditional centralized orchestration approaches. This project proposes a Two-Stage Multi-Agent Learning (TS-MAL) framework, a decentralized and intelligent SFC reconfiguration solution based on reinforcement learning. TS-MAL is designed to orchestrate onboarded SFCs efficiently across the Edge-Cloud Continuum. By enabling local orchestration agents to collaboratively reconfigure SFCs, the framework dynamically optimizes virtual function placement, scaling, and migration in response to real-time network conditions and service demand fluctuations. Experimental results demonstrate that TS-MAL achieves approximately 51.47% reduction in end-to-end service latency and 64.03% reduction in energy consumption for onboarded SFCs compared to a baseline single-agent Proximal Policy Optimization (PPO) approach.Furthermore, TS-MAL ensures 100% demands service rate associated to onboarded SFC significantly outperforming the PPO baseline, which achieves an average of 56.93%. These findings underscore the effectiveness of decentralized multi-agent learning in enabling scalable and adaptive service orchestration for next-generation Edge-Cloud infrastructures.

## Key Contributions

The main contributions of this research are summarized as follows:

- **Two-Stage Multi-Agent RL Framework:**  
  A two-stage, multi-agent reinforcement learning framework that integrates edge-aware message passing with decentralized decision-making. This enables intelligent, conflict-aware SFC reconfiguration while allowing each SFC agent to operate independently within a shared network environment.

- **Performance and Evaluation:**  
  Through extensive simulations, we demonstrate significant improvements in system performance, including enhanced energy efficiency, reduced end-to-end service latency, and improved Network Service Success Rate (NSSR) compared to baseline approaches.

# Two-Tier Edge–Cloud Architecture:

<img width="1280" height="720" alt="SystemModel19" src="https://github.com/user-attachments/assets/bbbfc769-4b0d-45f6-b14c-9a64d544c48e" />


- **Summary**

We consider the edge-cloud continuum environment, which is composed of edge and centralized cloud servers. These resources collaboratively host network services, and the onboarded network services receive a set of incoming demands.

# System Model

<img width="1245" height="656" alt="SystemDesign10" src="https://github.com/user-attachments/assets/a3475efc-e584-48a2-8c83-3b366983c707" />

- **High-Level Workflow**
  -  Load network topology (edge + cloud nodes).
  - Generate service demands for each onboarded SFC.
  - Convert topology and SFC state into localized graphs.
  - EaGAT encodes node + edge features.
  - Independent PPO agents infer actions (deploy, scale, migrate, queue).
  - Environment updates latency and energy.
  - Rewards recorded and used for learning.
  - Repeat for multiple episodes.
- **Summary**

  The approach models the network as a graph, where each SFC acts as an independent agent.  
Using an Edge-Augmented Graph Attention Network (EaGAT), each agent receives a localized view of the network and learns optimal actions through a decentralized Independent PPO framework.


# Simulation Environment

A comprehensive simulation environment was set up to evaluate the efficiency of the proposed MAIPPO-EaGAT approach against the baseline algorithm. The simulations were conducted using a Python-based framework.

The experiments were executed in a computational environment configured to support computation-intensive data processing, featuring an AMD Ryzen 7 8700G CPU processor at 4.2 GHz with 8 cores and 16 threads, integrated Radeon 780M graphics, and 128 GB of RAM, with the software stack including PyTorch 2.6.0, PyTorch Geometric 2.6.1, and NetworkX 3.4.2.

<img width="680" height="518" alt="image" src="https://github.com/user-attachments/assets/0b580cba-9fc9-421c-8e82-daf0553e97e6" />

# Evaluation

The Network Service Success Rate (NSSR) reflects the proportion of service demands successfully processed by the system.
The proposed TS-MAL framework consistently achieves 100% NSSR across all SFCs and all demand levels, significantly outperforming the baseline Single-Agent PPO, which struggles under higher demand.

- **NSSR Comparison Between TS-MAL and Baseline PPO**
<img width="1920" height="967" alt="NSSR_pattern" src="https://github.com/user-attachments/assets/813ac157-6aee-4efb-bc18-104eedb5b242" />

*Note: Detailed evaluation metrics such as latency, energy, and convergence behavior are included in the academic manuscript (currently under review). Only the high-level NSSR results are shown here.*

# Repository Status
This repository provides a high-level overview of the research project.
The full source code is kept private until the associated academic paper is published.

