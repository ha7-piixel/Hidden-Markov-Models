# 📊 Hidden Markov Model (HMM) Visualizer

**Student Name:** Harikrishnan M 
**Registration Number:** TCR24CS032
**Project:** Baum-Welch Algorithm Implementation & Visualization

---

## 📝 Project Overview
This repository contains a full implementation of the **Baum-Welch Algorithm** (Expectation-Maximization) used to find the unknown parameters of a Hidden Markov Model (HMM). 

The application is built with a Python backend and a **Streamlit** frontend, allowing for real-time training and professional-grade visualization of state transitions.

### ✨ Key Features
* **Core Math:** Implementation of Forward-Backward and Baum-Welch algorithms from scratch.
* **Interactive UI:** Dynamic input for observation sequences and initial probability matrices.
* **High-End Visualization:** Uses D3.js-based rendering for clear, non-overlapping state diagrams.

---

## 🔬 The Mathematics (Baum-Welch)
The algorithm iteratively optimizes the model parameters $\theta = (A, B, \pi)$ to maximize the likelihood $P(O|\theta)$.

### 1. Expectation (E-Step)
We calculate the forward ($\alpha$) and backward ($\beta$) variables:
$$\alpha_t(i) = P(O_1, O_2, \dots, O_t, q_t = S_i | \lambda)$$
$$\beta_t(i) = P(O_{t+1}, O_{t+2}, \dots, O_T | q_t = S_i, \lambda)$$

### 2. Maximization (M-Step)
We update the transition matrix $A$ and emission matrix $B$ using the calculated $\xi_t(i,j)$ and $\gamma_t(i)$ values to converge on the optimal model.

---

## 🛠️ Tech Stack & Requirements
| Library | Description |
| :--- | :--- |
| **Streamlit** | Interactive web interface |
| **NumPy** | Matrix operations and numerical computing |
| **State-Transition-Diagrams** | Advanced D3.js/Graphviz rendering |
| **Flask** | Dependency for visualization assets |

> [!NOTE]
> Make sure you have **Graphviz** installed on your system path for the diagrams to render correctly.

---

## 🚀 How to Run
1. **Clone the repo:**
   ```bash
   git clone [https://github.com/ha7-piixel/Hidden-Markov-Models.git](https://github.com/ha7-piixel/Hidden-Markov-Models.git)
   cd Hidden-Markov-Models
