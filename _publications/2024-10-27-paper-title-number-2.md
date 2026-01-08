---
title: "QoS-Aware Tripartite Evolutionary Game Strategy: A Task-Driven Performance Optimization Based on ISCC for IoV"
collection: publications
category: conferences
except: 'This paper introduces an innovative Tripartite Evolutionary Game framework to optimize the integration of sensing, communication, and computation (ISCC) in vehicle networks. By utilizing a task-driven three-layer architecture and a unified QoS utility function, the proposed strategy achieves optimal resource scheduling and a 43.9% reward gain in mature collaborative environments.'
permalink: /publication/2024-10-24-paper-title-number-2
date: 2024-10-24
publisher: '2024 IEEE 100th Vehicular Technology Conference (VTC2024-Fall)'
paperurl: 'https://academicpages.github.io/files/paper3.pdf'
citation: 'Zhan S, Luo G, Gao Z, et al. QoS-Aware Tripartite Evolutionary Game Strategy: A Task-Driven Performance Optimization Based on ISCC for IoV[C] 2024 IEEE 100th Vehicular Technology Conference (VTC2024-Fall). IEEE, 2024: 1-6.'
---

### **Research Background & Motivation**
The advancement of Intelligent Transportation Systems (ITS) and 6G requires a shift from isolated resource management to the **Integration of Sensing, Communication, and Computation (ISCC)**. Traditional strategies that separate these resources often lead to uneven scheduling and fail to meet the diverse Quality of Service (QoS) requirements of complex scenarios like high-level autonomous driving. There is a critical need for a **unified performance metric** and a framework that can manage the natural competition and cooperation among these heterogeneous resources.

### **Core Contributions & Technical Innovations**
This paper proposes a task-driven resource management framework based on evolutionary game theory:

*   **Tripartite Evolutionary Game Model**: The research models the interactions between **Communication, Sensing, and Computation** entities as a tripartite game. This approach analyzes the dynamic evolution of resource allocation, acknowledging that vehicles in an IoV environment exhibit game-like behaviors when scheduling multidomain resources.
*   **Three-Layered System Architecture**: The framework is structured into three distinct layers:
    *   **Decision Space Layer**: Where participants (vehicles, RSUs, cloud) compete and collaborate to maximize utility.
    *   **Task-Driven Layer**: Which defines specific resource requirements and manages resource transfer based on game outcomes.
    *   **Resource Layer**: Which integrates multidomain resources into a unified pool for dynamic allocation.
*   **Unified QoS Utility Function**: The study develops a joint utility function that incorporates multi-node competition, dependency, and cooperation. This function provides a **unified representation of performance metrics** for ISCC, allowing for a comprehensive evaluation of the integrated system.

### **Experimental Highlights & Evolutionary Stages**
The research identifies three stages of technological evolution for ISCC: **Coexistence** (initial), **Mutual Aid** (development), and **Integrated Benefit** (maturity). Simulation results demonstrate:
*   **Convergence to Optimality**: Regardless of initial strategies, the system successfully converges to the **"Strong Coupling"** state (the Mature Stage), where all entities collaborate to achieve a win-win outcome.
*   **Resource Balance**: The study proves that lower resource imbalance ($G$) directly leads to higher joint utility for all participants.
*   **Efficiency**: Task-driven analysis effectively guides resource allocation, ensuring precise alignment with specific application demands.

---

**Analogy for Understanding**:  
Imagine a **"Smart Kitchen"** (the IoV system) where three specialized chefs—the **Communication Chef** (orders/logistics), the **Sensing Chef** (ingredient inspection), and the **Computation Chef** (recipe execution)—must share a limited set of tools and space. Initially, they work separately (Coexistence), often getting in each other's way. However, through the **Evolutionary Game Strategy**, they learn to coordinate their actions based on the specific "Dish" (Task) being ordered. Eventually, they reach a state of **"Strong Coupling"** where they synchronize perfectly, ensuring the meal is served with the highest quality (QoS) while wasting the least amount of energy and time.
