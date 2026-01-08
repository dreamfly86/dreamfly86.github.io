---
title: "Beam Prediction Method and Device for Internet of Vehicles Based on Multi-Modal Large Model"
collection: patents
granted: 2025-06-17
---

# How an AI That "Sees" Radio Waves Will Keep Your Future Car Perfectly Connected

We’ve all been there: driving through a city, deep in a call or streaming music, when the connection suddenly drops. It’s a momentary frustration. But for the future of autonomous and connected vehicles, a lost connection isn't a minor annoyance—it's a critical failure that could impact safety and functionality.

The traditional methods for maintaining a wireless connection, which involve constantly scanning for the best signal, are too slow and reactive for the complex, fast-changing environments these vehicles operate in. Millimeter-wave signals, which provide the high speeds future cars will need, are especially sensitive to being blocked by buildings, trees, and other traffic.

A groundbreaking new method, detailed in a recent patent from Xiamen University, offers a solution. It uses a sophisticated AI to predict the best connection by essentially allowing the car to "see" invisible radio waves. Here, we'll deconstruct the four key innovations from this patent that offer a blueprint for the future of vehicle connectivity.

---

## 1. An AI That Fuses Camera Vision with Radio Physics

At its core, the system uses a vehicle's onboard cameras to see the physical world—buildings, other cars, pedestrians, and infrastructure. But here is the brilliant leap: during its training phase, the AI is also fed data from a **"ray tracing model."** This is a physics simulation that calculates exactly how radio signals from a cellular base station bounce, reflect, and scatter off those same buildings and cars.

The key innovation is that the AI learns to connect what it sees with how radio waves behave. It learns that a glass-faced building reflects a signal differently than a concrete wall, and that a large truck will block a signal path entirely. By correlating the visual data with the physics simulation, the AI builds a **"channel feature"** map of the world.

This moves the car's understanding from a simple geometric map (**"there is a truck here"**) to a rich, physics-aware one (**"this truck is a 5G-blocking obstacle, but the glass building to the right is a potential signal reflector"**). This gives the vehicle a predictive, physics-based understanding of its own connectivity, allowing it to intelligently navigate around dead zones and capitalize on non-line-of-sight (NLOS) signals.

---

## 2. A "Brain" That Thinks in Pictures, Data, and Language

The AI powering this system is not a standard image-recognition model. The patent describes it as a **"Multi-modal Large Model,"** an advanced architecture that processes different types of information simultaneously to build a comprehensive understanding.

Broken down into simple terms, its key components include:

- A **Depth Estimation Network** that judges the distance to objects seen by the cameras.
- A **Visual Encoder** that understands what the objects are (e.g., cars, buildings, signs).
- A **Large Language Model (LLM)**, similar to the technology behind ChatGPT, which acts as a sophisticated reasoning engine to process the information.

A crucial component called a **"learnable connector"** bridges the gap between the visual information and the LLM. By feeding the LLM a prompt containing the car's real-time motion data and background physics, the system can reason about the visual scene in the context of radio propagation, outputting precise predictions about where signals will scatter and with what intensity. This advanced structure enables the system to output highly specific data in a way a simpler model could not.

---

## 3. It Predicts the "When," Not Just the "What"

To maintain a high-speed connection, vehicles and base stations use focused radio signals called **beams**. The window of time that a specific beam remains stable is known as its **"beam coherence time."** As the patent points out, existing systems that use a fixed time for this window are inefficient. If a bus pulls in front of the car, the beam can become misaligned, dropping the connection. If the environment is stable, the system might perform wasteful updates when none are needed.

This is where the new system makes another significant advance:

① The multi-modal AI predicts the coordinates and strength of key signal scatter points.
② This data is then used to generate a **"scatter heatmap"**—a visual representation of the best and worst places for signals in the car's immediate vicinity.
③ This heatmap, combined with the car's location data, is fed into a final **"beam prediction model"** that decides:
   - the next best beam to switch to, and  
   - the optimal time length that beam should be used for.

This dynamic adjustment is a game-changer. By proactively managing how long it holds onto a beam based on its predictive understanding of the environment, the connection becomes far more efficient and robust. This proactive resource management is the difference between a network that is merely fast and one that is truly intelligent and resilient—a non-negotiable requirement for Level 4 and 5 autonomy.

---

## 4. The Car Uses Its Own Eyes for a Clearer View

One could imagine an alternative where cameras are placed on the cell towers themselves. However, the patent highlights a key weakness in that approach: a tower's view can easily be blocked by traffic or other obstacles between it and the target vehicle.

The proposed method cleverly avoids this by putting the intelligence where the action is: **on the vehicle.** By using the car's own multi-view cameras (for example, front and rear-facing), the system always has a clear, ground-level perspective of its immediate surroundings.

This makes the system inherently more reliable in the exact scenarios where connectivity is most challenging—dense, dynamic urban environments. The car isn't relying on a distant, potentially obstructed viewpoint; it's using its own eyes to navigate its digital world.

---

## Conclusion: A Glimpse into a Smarter, More Connected Future

The future of reliable, high-speed vehicle connectivity won't be solved by more powerful hardware alone. It will rely on predictive, environment-aware AI that can anticipate changes in the radio environment before they happen. This technology from Xiamen University provides a compelling blueprint for such a system.

This transforms the vehicle from a passive receiver of data into an active participant in its own connectivity, equipped with a digital sixth sense for navigating an invisible landscape of information. As our cars learn to see and predict the radio waves around them, what other invisible forces could they learn to master next?
