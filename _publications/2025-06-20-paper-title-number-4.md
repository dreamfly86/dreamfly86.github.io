---
title: "A Review on Federated Learning Architectures for Privacy-Preserving AI: Lightweight and Secure Cloud–Edge–End Collaboration"
collection: publications
category: manuscripts
permalink: /publication/2025-06-20-paper-title-number-4
excerpt: 'This systematic review proposes a cloud–edge–end collaborative framework for Federated Learning, specifically addressing the challenges of resource-constrained and heterogeneous environments. By introducing a 3D trustworthiness framework and analyzing the Privacy–Efficiency–Accuracy trilemma, the work provides foundational insights for building secure, lightweight, and explainable AI systems for 6G and the Internet of Things.'
date: 2025-06-20
publisher: 'MDPI'
paperurl: 'https://github.com/dreamfly86/dreamfly86.github.io/blob/master/files/electronics-14-02512.pdf'
bibtexurl: 'https://github.com/dreamfly86/dreamfly86.github.io/blob/master/files/electronics-v14-i13_20260105.bib'
citation: 'Zhan S, Huang L, Luo G, et al. A Review on Federated Learning Architectures for Privacy-Preserving AI: Lightweight and Secure Cloud–Edge–End Collaboration[J]. Electronics, 2025, 14(13): 2512.'
---

### **Research Background & Motivation**
With the transition of 6G from "connecting everything" to **"connecting intelligence,"** the integration of distributed AI and edge computing has become essential. While centralized cloud computing faces bottlenecks in latency, bandwidth, and privacy, the emergence of **Federated Learning (FL)** offers a promising paradigm for collaborative model training without raw data exchange. however, practical implementation is hindered by massive **heterogeneity of devices and data**, stringent communication constraints, and evolving security threats.

### **Core Contributions & Key Innovations**
This comprehensive systematic review provides a roadmap for the next generation of privacy-preserving AI through a **cloud–edge–end collaborative architecture**:

*   **Three-Dimensional Trustworthiness Framework**: The paper reconstructs the "Trusted AI" concept for FL into three pillars: **Data Trustworthiness** (authenticity), **Process Trustworthiness** (fairness and traceability), and **Outcome Trustworthiness** (transparency and explainability).
*   **Systematic Taxonomy of FL Architectures**: It categorizes state-of-the-art FL paradigms—**Horizontal FL (HFL), Vertical FL (VFL), and Federated Transfer Learning (FTL)**—analyzing their respective mathematical objectives, privacy mechanisms, and cross-domain applications.
*   **Lightweight Optimization Paradigm**: To address resource-constrained environments, the review dissects the **trilemma of Privacy–Efficiency–Accuracy**. It analyzes optimization strategies such as model pruning, quantization, asynchronous updates, and the "entropy increase effect" caused by blockchain-enhanced security.
*   **Cloud–Edge–End Synergy**: The research emphasizes vertical functional decoupling (Cloud for global aggregation, Edge for regional coordination, and End for local micro-training) to balance global analysis with local real-time processing.

### **Future Research Directions**
The paper identifies several frontier topics critical for 6G-enabled systems:
*   **Online and Real-Time FL**: Enabling continuous iteration for streaming data.
*   **Multimodal FL**: Harmonizing multi-source heterogeneous data (e.g., images, voice, sensors) while ensuring crossmodal privacy.
*   **Self-Adaptive Orchestration**: Utilizing reinforcement learning (RL) to dynamically adjust communication intervals and participation rates in highly dynamic environments.

---

### **Analogy for Understanding**
Imagine building a **"Global Smart Library"** where every local branch (End device) has unique, secret books. Instead of sending the secret books to a central headquarters (Cloud), each branch writes its own summary (Model update). A regional supervisor (Edge) gathers these summaries to avoid mail congestion. 
The **3D Trust Framework** ensures that the summaries are true (**Data Trust**), that the supervisor doesn't ignore small branches (**Process/Fairness Trust**), and that the final combined encyclopedia is actually readable and useful for librarians (**Outcome/Explainability Trust**).
