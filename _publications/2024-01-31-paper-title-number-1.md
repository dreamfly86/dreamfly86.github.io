---
title: "ST-HO: Symmetry-Enhanced Energy-Efficient DAG Task Offloading Algorithm in Intelligent Transport System"
collection: publications
category: manuscripts
permalink: /publication/224-01-31-paper-title-number-1
excerpt: 'This paper presents ST-HO, a symmetry-enhanced hybrid algorithm (Simulated Annealing + Tabu Search) for task offloading in IoV. By modeling tasks as Directed Acyclic Graphs (DAGs) and exploiting structural symmetry, the framework achieves a 52.63% faster convergence and significantly reduces system energy consumption while meeting real-time execution constraints in intelligent transportation environments.'
date: 2024-01-31
publisher: 'MDPI'
paperurl: 'https://github.com/dreamfly86/dreamfly86.github.io/blob/master/files/symmetry-16-00164.pdf'
bibtexurl: 'https://github.com/dreamfly86/dreamfly86.github.io/blob/master/files/symmetry-v16-i02_20260105.bib'
citation: 'Gao Z, Luo G, Zhan S, et al. ST-HO: Symmetry-Enhanced Energy-Efficient DAG Task Offloading Algorithm in Intelligent Transport System[J]. Symmetry, 2024, 16(2): 164.'
---

### **Research Background & Motivation**
Modern Intelligent Transport Systems (ITS) face an increasing demand for computational resources due to applications like autonomous driving and traffic monitoring. While Mobile Edge Computing (MEC) allows vehicles to offload burdensome sensing tasks to Road Side Units (RSUs), most existing strategies ignore the **intrinsic dependencies** within tasks. This research addresses the challenge of optimizing energy consumption while respecting the execution order of subtasks, particularly those with complex structures.

### **Core Contributions & Technical Innovations**
The paper introduces an energy-efficient offloading paradigm based on **Mobile Sensing–Communication–Computation (MSCC)** synergy:

*   **DAG-Based Task Modeling**: Unlike coarse-grained models, this work represents vehicle tasks as **Directed Acyclic Graphs (DAGs)**. This captures the temporal dependencies between subtasks, where a subtask can only commence after all preceding prerequisite subtasks are completed.
*   **ST-HO Hybrid Algorithm**: The study proposes a hybrid optimization algorithm combining **Simulated Annealing (SA)** and **Tabu Search (TS)**. This approach leverages SA’s ability to escape local optima and TS’s efficiency in avoiding repetitive searches to minimize total system energy consumption under strict delay constraints.
*   **Symmetry-Enhanced Decision Making**: A key innovation is the integration of **symmetry** into the DAG structure. By identifying symmetric subtasks, the algorithm only calculates offloading strategies for half of the tasks and directly replicates them for the other half. This significantly reduces computational overhead and facilitates rapid decision-making.

### **Experimental Highlights**
Extensive simulations on both small-scale (11 subtasks) and large-scale (30 subtasks) models demonstrate the superiority of the ST-HO algorithm:
*   **Energy Efficiency**: ST-HO reduces energy consumption by at least **5.58%** compared to conventional algorithms, achieving even higher reductions (up to 17.58%) compared to Greedy and SA methods in specific scenarios.
*   **Faster Convergence**: By utilizing the replication strategy for symmetric tasks, the algorithm improves convergence speed by **52.63%**.
*   **Scalability**: The algorithm maintains high optimization performance and a good balance between complexity and energy saving as task sizes and vehicle communication rates vary.

---

### **Analogy for Understanding**
Imagine a **"Smart Assembly Line"** (the DAG task) where certain parts must be bolted before they can be painted. Most systems treat every part as a brand-new problem, wasting time recalculating where to do the work. The **ST-HO algorithm** acts as an expert foreman who combines "trial-and-error" intuition (Simulated Annealing) with a "cheat sheet" of past mistakes to avoid (Tabu Search). Furthermore, by noticing that the left and right sides of the car are **symmetrical**, the foreman simply copies the plan from one side to the other, getting the job done twice as fast with far less effort.
