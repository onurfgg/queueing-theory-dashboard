# ⏳ Industrial Engineering Dashboard: M/M/c Queueing Simulator

![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![Chart.js](https://img.shields.io/badge/chart.js-F5788D.svg?style=for-the-badge&logo=chart.js&logoColor=white)
![Operations Research](https://img.shields.io/badge/Operations%20Research-Stochastic%20Processes-success)

A modern, web-based interactive simulation engine designed to visualize and analyze the **M/M/c Queueing Model** in real-time. This dashboard bridges the gap between theoretical Operations Research formulas and practical system behavior by simulating random arrivals (Poisson process) and service times (Exponential distribution) right in the browser.

[🚀 **Click Here for Live Demo**](https://onurfgg.github.io/queueing-theory-dashboard/) *(Buraya kendi canlı linkini eklemeyi unutma)*

## ✨ Key Features

* **Real-Time Stochastic Simulation:** Watch customers arrive and get served dynamically based on probabilistic models, not pre-scripted animations.
* **Live Chart.js Integration:** Tracks and graphs the number of entities in the system ($L$) and in the queue ($L_q$) instantaneously as the simulation runs.
* **Theoretical vs. Empirical:** Automatically calculates steady-state expectations (Probability of zero entities, utilization rate, etc.) and allows you to compare them against the live running simulation.
* **Time-Warp Engine:** Includes a safe, anti-crash speed multiplier that allows you to simulate hours of queueing behavior in mere seconds.
* **Glassmorphism UI:** A highly polished, dark-themed interface inspired by modern analytics tools.

## 🧮 Mathematical Background (M/M/c Model)

The underlying engine relies on the classic Markovian queueing theory:
* **Arrivals:** Follow a Poisson process with rate $\lambda$ (Lambda).
* **Service Times:** Follow an Exponential distribution with rate $\mu$ (Mu).
* **Servers:** $c$ identical servers working in parallel.

The Steady-State formulas calculated natively in the dashboard:

**System Utilization ($\rho$):**
$$\rho = \frac{\lambda}{c \mu}$$

**Probability of Zero Entities ($P_0$):**
$$P_0 = \left[ \sum_{n=0}^{c-1} \frac{(\lambda/\mu)^n}{n!} + \frac{(\lambda/\mu)^c}{c!} \left( \frac{1}{1-\rho} \right) \right]^{-1}$$

**Average Length of Queue ($L_q$):**
$$L_q = \frac{P_0 (\lambda/\mu)^c \rho}{c! (1-\rho)^2}$$

*Note: The system mathematically warns the user and prevents theoretical calculation if $\rho \ge 1$ (unstable system capacity).*

## 🛠️ Installation & Usage

This project is fully client-side. No complex dependencies, server setups, or databases required.

1. Clone the repository:
   ```bash
   git clone [https://github.com/onurfgg/mmc-queueing-simulator.git](https://github.com/onurfgg/mmc-queueing-simulator.git)

Onur Furkan Gök

[Linkedin](https://www.linkedin.com/in/onurfurkan/) 
[GitHub](https://github.com/onurfgg) 

   
