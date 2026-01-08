---
title: "A Method and Apparatus for Enhancing the Reliability of Multimodal Large Models Driven by Both Data and Knowledge"
collection: patents
published: 2024-06-14
---

# Beyond Accuracy: This AI Uses 'Spatio-Temporal Collisions' to Build Real-World Trust

## Introduction: The Trust Gap in Modern AI

We increasingly rely on artificial intelligence for high-stakes tasks, from navigating autonomous vehicles through city streets to managing the complex ecosystems of our smart homes. In these scenarios, a simple right or wrong answer isn't enough. While traditional AI models are optimized for accuracy, they often lack a crucial component: the credibility or trustworthiness of their outputs. An AI might be 99% accurate in identifying a stop sign, but that accuracy is meaningless if it fails to understand the context of a busy intersection.

This gap between accuracy and trust is a significant hurdle for the widespread adoption of AI in critical applications. Addressing this challenge, a recently published patent application (**CN 118194012 A**) from researchers at **Xiamen and Jimei Universities** proposes a novel solution. Their **"data-knowledge dual-driven"** method aims to enhance the credibility of multi-modal AI models, ensuring their decisions are not just statistically probable but also logically sound in the real world.

This article will break down the four most impactful ideas from this patent, translating its technical framework into easy-to-understand takeaways that reveal how AI can learn to trust itself.

---

## 1. AI Gets a "Gut Check" with a Knowledge Base

The fundamental problem with many AI systems is that they operate in a vacuum of pure data. A multi-modal model, for instance, might process various inputs—like video from a camera, audio from a microphone, and signals from radar—to produce a single output, which the patent calls a **"fused feature."** This feature represents the AI's best guess based on the data it has seen. However, this conclusion is based solely on patterns in the data, not on real-world context or rules.

The patent's solution is to give the AI a **"gut check."** The method compares the data-driven **"fused feature"** against a pre-set **"knowledge base."** This knowledge base is essentially a digital rulebook for a given scenario, containing established laws, rules, and known patterns. For an autonomous vehicle, this could include traffic regulations, speed limits, and the physical laws of momentum. This approach powerfully frames a classic symbolic AI (the rule-based knowledge base) as a governor for a sub-symbolic AI (the data-driven neural network), providing a critical layer of oversight.

This crucial comparison process is termed a **"spatio-temporal collision."** Think of it as a reality check where the AI's data-based conclusion "collides" with established knowledge. The system measures the degree of overlap between its output and the knowledge base to see if its conclusion makes sense in the real world.

---

## 2. It's Not Just What Is Happening, but When and Where

The concept of a **"spatio-temporal collision"** is more sophisticated than a simple fact-check. It evaluates the AI's conclusion on two distinct but related dimensions, ensuring the output is not only correct but also contextually appropriate.

The two components of this check are:

- **Vector Space Similarity:** This assesses the semantic similarity. It answers the question, **"What is happening?"** For example, does the AI's output vector correspond to a known **'turn left'** command in the knowledge base? This confirms the basic interpretation of the data is correct.
- **Temporal Correlation:** This assesses the contextual appropriateness. It answers the questions, **"Is this the right time and place for this to happen?"** This check verifies if the action aligns with time-sensitive rules, environmental states, or sequential logic defined in the knowledge base.

An autonomous vehicle provides a perfect example. The AI might correctly identify a **'turn left'** maneuver from its sensor data (high vector space similarity). However, the spatio-temporal check would also consult the knowledge base, which includes traffic signal rules. If the traffic light is red, the system flags a low temporal correlation. The action is semantically correct but contextually wrong and dangerous. This dual check prevents the AI from making technically accurate but practically disastrous decisions.

---

## 3. Trust Becomes a Key Input, Not Just an Output

After the spatio-temporal collision, the system generates an **"initial credibility"** score for its data-driven conclusion. A high score means the AI's output aligns well with the established knowledge base. From here, the system initiates a sophisticated two-step process to refine this score:

① **Probability fusion (Bayes):** It performs a **"probability fusion"** using Bayes' formula, combining the raw **"fused feature"** with the **"spatio-temporal collision result."** This generates a new **"fusion result"**—a probabilistic assessment of how likely the feature is, given the reality check.
② **Credibility update:** This fusion result is used to update the initial credibility, producing a final **"target credibility"** score, effectively scaling the initial score by the Bayesian probability.

Here is where the process takes its most innovative turn. Instead of using this credibility score simply as a final confidence metric, the system **feeds it back into the decision-making process**. The final classification network receives two inputs:

- The original **"fused feature"** (what the AI **"sees"**)
- The **"target credibility"** score (how much it **trusts** what it sees)

This is a profound shift. It makes the model's epistemic uncertainty—its own awareness of its confidence—a first-class feature in the decision-making process. The system's final decision is based not only on the raw data but also on its own calculated confidence, which prevents the model from being confidently wrong—a common and dangerous failure mode in traditional classifiers.

---

## 4. The System Learns From Its Own Uncertainty

Perhaps the most powerful aspect of this method is its adaptive credibility framework. The patent describes a self-correcting feedback loop that triggers whenever the system generates a low **"target credibility"** score. An instance of low confidence is not treated as a failure but as a learning opportunity.

When the system flags its own output as having low credibility, it initiates an optimization process by pulling one of two levers. It must determine whether its data interpretation was flawed or its worldview was incomplete:

① **Optimize Pre-processing Strategies:** The system can adjust how it handles data from the very beginning. If the data interpretation was the issue, it might improve data cleaning techniques or refine how it extracts features to produce a more reliable **"fused feature"** in the future.
② **Update the Knowledge Base:** If the data was interpreted correctly but conflicted with the rules, the uncertainty might stem from an outdated or incomplete rulebook. The system can then update the knowledge base to account for new user behaviors or changing environmental rules.

This dynamic feedback loop allows the AI to improve its trustworthiness over time. By actively identifying and learning from moments of uncertainty, the system becomes more robust, reliable, and ultimately, more aligned with the complexities of the real world.

---

## Conclusion: The Future is Credible AI

This **"data-knowledge dual-driven"** approach represents a crucial evolution in AI development. By moving beyond a narrow focus on accuracy, it provides a framework for building systems with quantifiable, verifiable trust. The concepts of spatio-temporal collisions and self-correcting feedback loops create an AI that doesn't just provide answers, but also understands whether those answers are credible in the context of our world.

As we hand over more critical decisions to AI, this patent prompts a vital question for the future of technology and society:

> How will we, as a society, ultimately define and measure our trust in these intelligent systems?


