# Special-Topics-2

# Community Detection in Multi-Attributed Networks

## Hybrid Multiobjective Evolutionary Algorithm (HMOEA-CD)

---

## 📌 Overview

This project presents a **Hybrid Multiobjective Evolutionary Algorithm for Community Detection (HMOEA-CD)** in multi-attributed networks. The goal is to identify meaningful communities by optimizing multiple objectives such as structural quality and community compactness.

Traditional community detection methods focus only on network topology. This project improves upon them by using **multiobjective optimization and evolutionary algorithms** to achieve better clustering performance.

---

## 🎯 Objectives

* Detect communities in complex networks
* Maximize **modularity (Q)**
* Minimize **number of communities**
* Improve clustering accuracy using evolutionary optimization

---

## ⚙️ Methodology

The proposed approach uses a **Multiobjective Evolutionary Algorithm (MOEA)** with the following steps:

1. Initialize population (chromosomes representing communities)
2. Evaluate fitness using:

   * Modularity
   * Community size
3. Apply genetic operations:

   * Selection
   * Crossover
   * Mutation
4. Perform local refinement
5. Select best solutions using Pareto optimization
6. Output final community structure

---

## 🧠 Key Concepts

* Community Detection
* Multiobjective Optimization
* Genetic Algorithms
* Modularity Maximization
* Pareto Optimality

---

## 📊 Datasets Used

| Dataset       | Type       | Description                               |
| ------------- | ---------- | ----------------------------------------- |
| LFR Benchmark | Synthetic  | Standard benchmark for testing algorithms |
| WebKB         | Real-world | Webpage classification network            |
| Mafia Network | Social     | Small social interaction network          |

---

## 📈 Evaluation Metrics

The performance of the algorithm is evaluated using:

* **Modularity (Q)** – Measures community structure quality
* **Normalized Mutual Information (NMI)** – Measures similarity with ground truth
* **F1 Score** – Accuracy of community assignments
* **Computational Efficiency** – Runtime and convergence

---

## 📊 Results Summary

| Method       | Modularity | NMI      | F1 Score |
| ------------ | ---------- | -------- | -------- |
| K-Means      | 0.42       | 0.51     | 0.55     |
| Spectral     | 0.48       | 0.58     | 0.61     |
| Louvain      | 0.55       | 0.65     | 0.70     |
| **HMOEA-CD** | **0.69**   | **0.78** | **0.82** |

👉 The proposed method outperforms traditional approaches in all metrics.

---

## 📉 Convergence Behavior

The algorithm shows rapid improvement in early generations and stabilizes later, indicating efficient optimization.

---

## 📂 Project Structure

```
├── data/               # Datasets (LFR, WebKB, Mafia)
├── src/                # Implementation code
├── results/            # Output results and graphs
├── figures/            # Visualization images
├── paper/              # Research paper
└── README.md           # Project documentation
```

---

## 🚀 How to Run

1. Install required libraries:

   ```bash
   pip install networkx numpy matplotlib
   ```

2. Run the main script:

   ```bash
   python main.py
   ```

3. View results:

   * Community visualization
   * Performance metrics
   * Convergence graphs

---

## 🔮 Future Work

* Incorporate node attribute similarity explicitly
* Detect overlapping communities
* Extend to dynamic networks
* Improve scalability for large datasets
* Integrate deep learning (GNNs)

---

## 📚 References

* Multiobjective Evolutionary Algorithms for Community Detection
* IEEE Transactions on Cybernetics papers
* Modularity optimization methods

---

## 👨‍💻 Authors

* Chetan Jain
* Ojash Choudhary

---

## ⭐ Conclusion

The proposed **HMOEA-CD** provides an effective and scalable solution for community detection in complex networks by leveraging multiobjective optimization and evolutionary strategies.

---
