---
title: "An incentive mechanism for joint sensing and communication Vehicular Crowdsensing by Deep Reinforcement Learning"
collection: publications
category: manuscripts
permalink: /publication/2025-04-01-paper-title-number-3
excerpt: 'This paper presents a social-aware incentive mechanism for Vehicular Crowdsensing that integrates Small-World networks with joint sensing and communication optimization. By leveraging a VAE-enhanced PPO algorithm (IM-SJSC), the framework successfully motivates self-interested vehicles to participate, achieving up to a 43.9% reward gain and superior data collection efficiency in realistic urban environments.
'
date: 2025-04-01
publisher: 'Elsevier'
paperurl: 'https://github.com/dreamfly86/dreamfly86.github.io/blob/master/files/An_incentive_mechanism_for_joint_sensing_and_communication_Vehicular_Crowdsensing_by_Deep_Reinforcement_Learning.pdf'
bibtexurl: 'https://github.com/dreamfly86/dreamfly86.github.io/blob/master/files/An_incentive_mechanism_for_joint_sensing_and_communication_Vehicular_Crowdsensing_by_Deep_Reinforcement_Learning.bib'
citation: 'Luo G, Zhan S, Liang C, et al. An incentive mechanism for joint sensing and communication Vehicular Crowdsensing by Deep Reinforcement Learning[J]. Computer Networks, 2025, 260: 111099.'
---

### **Research Background & Motivation**
Vehicular Crowdsensing (VCS) is a vital component of Intelligent Transportation Systems (ITS), yet it faces significant hurdles due to the **self-interested nature of participants** and the high costs associated with energy consumption and privacy risks. Traditional incentive mechanisms often struggle with exploding costs in large-scale scenarios and fail to account for the **realistic social structures** and the **joint optimization of sensing and communication**.

### **Core Contributions & Technical Innovations**
This research proposes a novel social-aware incentive mechanism designed to maximize participant utility under incomplete information:

*   **Small-World (SW) Social Network Integration**: The study introduces a **Newman-Watts (NW) Small-World network** to model the Vehicle Social Network (VSN). This model captures realistic vehicle interactions and provides **non-monetary incentives** through social benefits, sustaining engagement even when monetary rewards are relatively low.
*   **Joint Sensing and Communication Strategy**: Unlike prior works that treat sensing and communication in isolation, this framework enables vehicles to independently determine optimal **sensing time** and **transmission power**. This ensures that data is not only collected but also transmitted to the platform within strict time-slot deadlines.
*   **IM-SJSC Algorithm**: A multi-agent Deep Reinforcement Learning (DRL) approach is developed, combining **Proximal Policy Optimization (PPO)** with a **Variational Autoencoder (VAE)**. The VAE serves as a feature extraction network to distill high-dimensional state information into a structured latent space, enhancing decision-making accuracy and robustness in dynamic environments.

### **Experimental Highlights**
Evaluated using the real-world **T-Drive Beijing taxi dataset**, the proposed **IM-SJSC** algorithm demonstrated significant performance gains:
*   **Utility Improvement**: The average utility outperformed baseline methods (such as Q-learning and DRL-SIM) by **25.00% to 181.82%** under varying vehicle numbers.
*   **Operational Efficiency**: The algorithm achieved the **highest task completion rate** and the **lowest average latency** (as low as 36.8 ms), effectively balancing operational costs with social and monetary rewards.

---


**Analogy for Understanding**:  
Think of this VCS system as a **"Social-Media-Driven Courier Network."** Instead of just paying drivers a flat fee (monetary incentive), the system connects them through a "friend network" (Small-World Network) where they gain "social points" or status by sharing road data. To make sure the system stays efficient, the **IM-SJSC algorithm** acts like a smart personal assistant for each driver, calculating exactly how much time to spend "picking up info" (sensing) versus "driving fast to deliver it" (communication) so they can maximize their total earnings and social standing without burning out.
