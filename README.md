# 🚦 TrafficMind: Bio-Inspired Signal Optimizer

**Live Demo:** [Insert your Vercel URL here]

## Overview
TrafficMind is a microscopic traffic simulator built to demonstrate the power of **biomimicry** in computer engineering. Inspired by the collective intelligence, social sharing, and foraging behavior of bird flocks, this project utilizes **Particle Swarm Optimization (PSO)** to dynamically adapt traffic signal timings. 

By simulating real-world Navi Mumbai intersections, this project proves how decentralized, swarm-based algorithms can solve complex urban gridlock far more effectively than rigid, fixed-time systems.

## The Biology Connection (How it Works)
* **The Swarm:** The algorithm generates a "swarm" of particles, where each particle represents a candidate green-light timing plan.
* **Collective Intelligence:** Just as birds communicate the location of food to the flock, particles communicate the best traffic-flow solutions (Global Best) to one another.
* **Natural Selection (Fitness):** Each plan is evaluated based on its ability to reduce vehicle delay and queue lengths. The swarm naturally gravitates toward and refines the most successful traits over multiple iterations.

## Features
* **Microscopic Simulation:** Uses the Intelligent Driver Model (IDM) for braking/acceleration and Poisson distribution for realistic, stochastic vehicle arrivals.
* **Live Performance Metrics:** Compares Fixed-Time vs. PSO-optimized signals side-by-side in real-time.
* **Navi Mumbai Scenarios:** Simulates localized bottlenecks including Vashi Plaza (Heavy N-S) and Sion-Panvel Expressway (Heavy E-W).
* **Experiment Lab:** Runs headless simulations over multiple held-out trial seeds to prove true algorithmic generalization.

## Tech Stack
* **Frontend:** HTML5 Canvas, CSS3, Vanilla JavaScript (Zero external dependencies)
* **Deployment:** Vercel
