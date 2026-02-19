# Adaptive Autonomous Cyber Defense via Cost-Aware Deep Reinforcement Learning in Dynamic Network Environments

## Overview

Modern computer networks face continuously evolving cyber threats that traditional rule-based security systems struggle to handle. Static defenses cannot adapt quickly to novel attacks, leading to delayed detection and significant damage.

This project presents an autonomous cyber-defense framework that uses cost-aware deep reinforcement learning (DRL) to detect and mitigate malicious network activity in real time. The system learns adaptive response policies directly from network traffic data, enabling proactive and intelligent intrusion mitigation.

---

## Key Contributions

- Autonomous intrusion response using deep reinforcement learning
- Cost-sensitive reward design balancing security and service availability
- Evaluation on real-world network intrusion datasets (e.g., UNSW-NB15)
- Comparison with classical machine learning-based intrusion detection systems
- End-to-end reproducible research pipeline

---

## Methodology

The problem is formulated as a sequential decision-making task.

### Environment

Network traffic observations are treated as system states.  
At each time step, the agent selects a mitigation action.

### Action Space

- Allow traffic
- Monitor connection
- Rate limit suspicious activity
- Block traffic

### Reward Function

The reward function balances:

- Successful attack mitigation
- False positive penalties
- Service disruption costs
- Missed attack penalties

This cost-aware formulation reflects real-world cybersecurity trade-offs.

---

## Dataset

Experiments are conducted using the **UNSW-NB15** intrusion dataset, which contains realistic network traffic with multiple attack categories.

The dataset is not included in this repository due to size constraints.

Download from:

- Official site: https://research.unsw.edu.au/projects/unsw-nb15-dataset
- Kaggle mirror: https://www.kaggle.com/datasets/mrwellsdavid/unsw-nb15

---
