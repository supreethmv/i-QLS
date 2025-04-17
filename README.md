# i-QLS
Iterative Quantum Least Squares Algorithm

<!-- [![Paper DOI](https://img.shields.io/badge/DOI-10.1109/QCE60285.2024.00059-orange)](https://doi.org/10.1109/QCE60285.2024.00059)   -->
<!-- [![arXiv](https://img.shields.io/badge/arXiv-2405.14405-green)](https://doi.org/10.48550/arXiv.2405.14405)   -->
[![Conference](https://img.shields.io/badge/Conference-ICCS'25-blue)](https://www.iccs-meeting.org/iccs2025/)  
[![License: Apache License 2.0](https://img.shields.io/badge/License-Apache%20License%20v2.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)  
<!-- [![LinkedIn: SupreethMV](https://img.shields.io/badge/LinkedIn-Supreeth%20Mysore%20Venkatesh-blue)](https://www.linkedin.com/in/supreethmv/)   -->
<!-- [![Website: SupreethMV](https://img.shields.io/badge/Website-www.supreethmv.com-brightgreen)](https://www.supreethmv.com) -->

---

# 🔍 Iterative Quantum-Assisted Least Squares (i-QLS)

This repository contains the official implementation of our paper:

> **"i-QLS: Quantum-supported Algorithm for Least Squares"**  
> 🏛️ Accepted at *25th International Conference on Computational Science (Main Track – Quantum Computing)*

---

## 🌟 Overview

Least squares optimization is at the heart of many machine learning and scientific computing tasks. But solving it with **quantum hardware** has traditionally been limited by the trade-off between **precision** and **hardware constraints**.

This project introduces **i-QLS**, an **iterative quantum-classical hybrid method** that reformulates the least squares objective into a series of **QUBO problems** — solvable by quantum annealers — and **refines the solution across iterations** to achieve higher accuracy with fewer qubits.

---

## ⚙️ How It Works

At a high level:

1. **Discretize** the continuous weight space into binary representations (using `m` bits per weight).
2. **Formulate** the least squares loss as a QUBO (Quadratic Unconstrained Binary Optimization) problem.
3. **Solve** the QUBO using a quantum annealer (e.g., D-Wave Advantage).
4. **Shrink** the search interval based on the best solution found.
5. **Repeat** the process iteratively — each round zooms in on the optimal solution.

This process makes our algorithm an **anytime method**: you can stop after any iteration and still get a meaningful solution.

---

## ✨ Features

- ✅ Scalable to **175+ features** on real quantum hardware  
- ✅ Demonstrated on both **linear** and **non-linear regression** (via splines)  
- 🔁 **Iterative and qubit-efficient**  
- 🧠 Extensible to **non-linear function approximation**  
- 🧪 Includes experiments on real-world D-Wave annealers

---

## 📈 Why It Matters

Traditional quantum approaches to least squares solve a single massive QUBO — requiring many qubits and offering limited flexibility. Our **iterative refinement strategy** breaks the problem into smaller, manageable QUBOs and converges **exponentially** to the true solution.

This makes i-QLS:
- 💡 **Scalable**: Works with today's limited quantum hardware  
- 🔬 **Precise**: Achieves high accuracy through iteration  
- 🔗 **Hybrid**: Bridges quantum optimization with classical preprocessing

---

## 🧪 Experiments & Reproducibility

You’ll find:
- 📊 MSE plots showing convergence across iterations  
- 🧬 Code for reproducing quantum runs on D-Wave (requires D-Wave API token)

---

## 💬 Questions or Feedback?

Open an issue or drop us a message. We welcome collaborations, ideas, and contributions!

---

## **Contact**

**Supreeth Mysore Venkatesh**  

For any inquiries, please reach out to:

- Email: contact@supreethmv.com  
- LinkedIn: [Supreeth Mysore Venkatesh](https://www.linkedin.com/in/supreethmv/)  
- Website: [www.supreethmv.com](https://www.supreethmv.com)


## Contributors

[![Supreeth Mysore Venkatesh](_repo_data/supreethmv.jpg)](https://www.supreethmv.com)