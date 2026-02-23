---
title: "HGSTA: Leveraging Hypergraph Computing for Effective Collaborative Perception Feature Fusion"
collection: publications
category: conferences
permalink: /publication/2025-10-19-paper-title-number-6
excerpt: 'This paper introduces HGSTA, a pioneering collaborative perception framework that leverages Hypergraph Computing to fuse multi-agent sensor data. By capturing high-order semantic relationships and utilizing a Deformable Attention Module to correct spatiotemporal misalignments, HGSTA achieves state-of-the-art 3D object detection accuracy and exceptional robustness against GPS errors and network delays in autonomous driving scenarios.'
date: 2025-10-19
publisher: '2025 IEEE 102nd Vehicular Technology Conference (VTC2025-Fall)'
paperurl: 'https://github.com/dreamfly86/dreamfly86.github.io/blob/master/files/HGSTA_Leveraging_Hypergraph_Computing_for_Effective_Collaborative_Perception_Feature_Fusion.pdf'
bibtexurl: 'https://github.com/dreamfly86/dreamfly86.github.io/blob/master/files/HGSTA_Leveraging_Hypergraph_Computing_for_Effective_Collaborative_Perception_Feature_Fusion.bib'
citation: 'Zheng S, Zhan S, Gao Z, et al. HGSTA: Leveraging Hypergraph Computing for Effective Collaborative Perception Feature Fusion[C] 2025 IEEE 102nd Vehicular Technology Conference (VTC2025-Fall). IEEE, 2025: 1-6.'
---
### **Research Background & Motivation**
Collaborative perception allows autonomous systems (like connected vehicles) to share sensor data, significantly improving their ability to navigate complex, occluded, and dynamic environments. However, sharing intermediate semantic features often suffers from **spatiotemporal misalignments** caused by sensor heterogeneity, transmission latency, and localization errors. Furthermore, most existing fusion methods rely on simple pairwise interactions (one-to-one), neglecting the **higher-order dependencies** across multiple agents that are crucial for robust perception in noisy real-world settings.

### **Core Contributions & Technical Innovations**
To overcome these limitations, this paper introduces **HGSTA (HyperGraph Spatial-Temporal Awareness)**, a novel multi-scale feature fusion framework. The core innovations include:

*   **High-Order Hypergraph Modeling**: Unlike traditional graphs that connect two nodes, HGSTA constructs a hypergraph where a single edge can connect multiple nodes. Utilizing Set-Pair Distance (SPD-HC), the framework models complex, group-level spatiotemporal and semantic correlations among multiple agents simultaneously.
*   **Multi-Scale Semantic Fusion**: The framework extracts and aligns features across different scales (low, mid, high), allowing the network to capture both fine-grained details and global contextual dependencies from diverse viewpoints. 
*   **Deformable Attention Module (DAM) Refinement**: To specifically tackle the issue of feature misalignment caused by ego-pose uncertainty or delays, HGSTA employs a Deformable Attention Module. DAM adaptively samples relevant context using learned spatial offsets, dynamically correcting spatial inconsistencies before final detection.

### **Experimental Highlights**
Extensive evaluations were conducted on three major collaborative driving benchmarks: OPV2V, V2XSet, and the real-world V2V4Real dataset. The results demonstrate HGSTA's significant superiority:
*   **State-of-the-Art Accuracy**: HGSTA outperformed leading baselines (like V2X-ViT and CoBEVT), surpassing the previous best by **5.06% and 3.28% in AP@0.7** on the OPV2V and V2XSet datasets, respectively.
*   **Exceptional Robustness**: The framework maintained highly stable detection accuracy even when injected with severe real-world disturbances, including **localization noise (up to 0.5m deviation)** and **communication delays (up to 200ms)**.

​---
### **Analogy for Understanding**
Imagine several witnesses (autonomous vehicles) trying to describe a chaotic intersection to a police officer. 
Traditional methods (Standard Graphs) act like the officer interviewing each witness **one-on-one**, which makes it hard to piece together the global picture, especially if someone’s watch is wrong (time delay) or they are confused about where they were standing (localization error). 
**HGSTA**, on the other hand, puts all witnesses in a **group conference room (the Hypergraph)** where they can instantly find commonalities and correct each other's blind spots. Meanwhile, the **DAM module** acts as a "fact-checker" who automatically adjusts for any witness's bad sense of direction or delayed memory, ensuring the final sketch of the intersection is perfectly accurate.
---
