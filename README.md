# Reconfiguration_Engine- Overview

# Title: Distributed Multi-Agent Reinforcement Learning Enabled Approach for Optimizing Service Function Chain Reconfiguration in Edge-Cloud Continuum

# Author: Gomathi Srinivasan Venkata

# Abstract
The emergence of the Edge-Cloud Continuum has transformed network service deployment by enhancing scalability,
responsiveness, and resource utilization. Within this paradigm,Service Function Chains (SFCs) play a critical role in fulfilling the
diverse requirements of latency-sensitive and compute-intensive
applications. However, dynamic conditions, such as fluctuating
resource availability, variable network service demands, and
stringent Quality of Service (QoS) constraints, pose significant
challenges to traditional centralized orchestration approaches. This
project proposes a Two-Stage Multi-Agent Learning (TS-MAL)
framework, a decentralized and intelligent SFC reconfiguration
solution based on reinforcement learning. TS-MAL is designed to
orchestrate onboarded SFCs efficiently across the Edge-Cloud Con-
tinuum. By enabling local orchestration agents to collaboratively
reconfigure SFCs, the framework dynamically optimizes virtual
function placement, scaling, and migration in response to real-time
network conditions and service demand fluctuations. Experimental
results demonstrate that TS-MAL achieves approximately 51.47%
reduction in end-to-end service latency and 64.03% reduction
in energy consumption for onboarded SFCs compared to a
baseline single-agent Proximal Policy Optimization (PPO) approach.
Furthermore, TS-MAL ensures 100% demands service rate associated to onboarded SFC
significantly outperforming the PPO baseline, which achieves an
average of 56.93%. These findings underscore the effectiveness
of decentralized multi-agent learning in enabling scalable and
adaptive service orchestration for next-generation Edge-Cloud
infrastructures.

## Key Contributions

The main contributions of this research are summarized as follows:

- **Challenge Identification:**  
  We highlight the complexity of orchestrating Service Function Chains (SFCs) across the edge–cloud continuum under fluctuating network conditions, diverse service demands, and limited computational resources.

- **Two-Stage Multi-Agent RL Framework:**  
  We propose a two-stage, multi-agent reinforcement learning framework that integrates edge-aware message passing with decentralized decision-making. This enables intelligent, conflict-aware SFC reconfiguration while allowing each SFC agent to operate independently within a shared network environment.

- **Performance and Evaluation:**  
  Through extensive simulations, we demonstrate significant improvements in system performance, including enhanced energy efficiency, reduced end-to-end service latency, and improved Network Service Success Rate (NSSR) compared to baseline approaches.

