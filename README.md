# 🚦 TrafficMind: Bio-Inspired Signal Optimizer

**Live Demo:** [https://bio-inspired-traffic-pso.vercel.app](https://bio-inspired-traffic-pso.vercel.app)[cite: 1]

## Overview
TrafficMind is a microscopic traffic simulator built to demonstrate the power of **biomimicry** in computer engineering. Inspired by the collective intelligence, social sharing, and foraging behavior of bird flocks, this project utilizes **Particle Swarm Optimization (PSO)** to dynamically adapt traffic signal timings. 

By simulating real-world Navi Mumbai intersections, this project proves how decentralized, swarm-based algorithms can solve complex urban gridlock far more effectively than rigid, fixed-time systems.

## Why This Project Was Built
TrafficMind was developed as an educational simulation to bridge the gap between biological algorithms and urban infrastructure challenges[cite: 2]. Traditional traffic networks often rely on conventional fixed-time plans (e.g., 30s + 30s green splits) that are determined in advance and never change during a run[cite: 2]. While predictable, these rigid systems cannot detect which approach has the longest queue during shifting traffic demands[cite: 2]. This project was created to visually and mathematically demonstrate how adaptive, search-based algorithms can evaluate candidate timing plans in real-time to minimize vehicle wait times[cite: 2]. 

## The Biology Connection (How it Works)
- **The Swarm:** The algorithm generates a "swarm" of particles, where each particle represents a candidate green-light timing plan[cite: 2].
- **Collective Intelligence:** Just as birds communicate the location of food to the flock, particles communicate the best traffic-flow solutions (Global Best) to one another.
- **Natural Selection (Fitness):** Each plan is evaluated based on its ability to reduce vehicle delay and time-averaged queue lengths[cite: 2]. The swarm naturally gravitates toward and refines the most successful traits over multiple iterations.

## Features
- **Microscopic Simulation:** Uses the Intelligent Driver Model (IDM) for braking/acceleration and Poisson distribution for realistic, stochastic vehicle arrivals[cite: 2].
- **Live Performance Metrics:** Compares Fixed-Time vs. PSO-optimized signals side-by-side in real-time.
- **Navi Mumbai Scenarios:** Simulates localized bottlenecks including:
  - *Vashi Plaza* (Heavy North-South)[cite: 2]
  - *Sion-Panvel Expressway* (Heavy East-West)[cite: 2]
  - *Palm Beach Rd* (Balanced)[cite: 2]
  - *Thane-Belapur Rd* (Rush Hour)[cite: 2]
  - *Kharghar Node* (Sudden Surge)[cite: 2]
- **Experiment Lab:** Runs headless simulations over multiple held-out trial seeds to prove true algorithmic generalization and generates average waiting times across scenarios[cite: 2].

## System Analysis: Pros & Cons

### Pros
* **Dynamic Rebalancing:** PSO can seamlessly rebalance green splits when traffic demand shifts, preventing heavy queues on busy approaches from compounding[cite: 2].
* **Targeted Optimization:** The swarm actively searches for timing plans that keep both vehicle delay and queue lengths low within the simulated environment[cite: 2].
* **Rolling-Horizon Adaptability:** The system includes an optional rolling-horizon mode that re-optimizes signals at cycle boundaries using recent arrival data[cite: 2].

### Cons & Limitations
* **Vulnerability to Sudden Surges:** A plan perfectly tuned for one specific demand pattern can perform worse if the traffic demand suddenly changes mid-run[cite: 2].
* **No Global Optimum Guarantee:** Because the PSO algorithm is a search method with limited iterations, it cannot promise it will find the absolute best possible answer[cite: 2].
* **Simulation Simplifications:** The current model evaluates a simplified environment with one lane per approach, straight movements only, and two phases (omitting turning lanes and pedestrian crossings)[cite: 2].
* **Assumption of Perfect Conditions:** The algorithm assumes perfect driver compliance and operates without sensor noise, which does not reflect real-world unpredictability[cite: 2].

## Tech Stack
- **Frontend:** HTML5 Canvas, CSS3, Vanilla JavaScript (Zero external dependencies)[cite: 2]
- **Deployment:** Vercel (Continuous Deployment via GitHub)[cite: 1]

## Acknowledgements
This project was conceptualized, structured, and developed with the assistance of Artificial Intelligence, specifically utilizing Anthropic's Claude and Google's Gemini to accelerate algorithm design, logic structuring, and code refinement.
