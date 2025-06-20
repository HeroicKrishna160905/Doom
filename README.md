# 🧠 Doom Reinforcement Learning Experiments

Welcome to the **Doom RL Experiments** repository — an applied reinforcement learning (RL) project built around the ViZDoom environment. This project showcases how classic video games can be used as research-grade platforms for training intelligent agents using deep reinforcement learning, computer vision, and control theory.

🎯 **This project demonstrates the integration of modern RL algorithms with ViZDoom, turning Doom into a testbed for evaluating agent behavior, strategy learning, and visual understanding directly from raw pixel inputs.**

---

## 📌 Key Highlights

- ✅ **Full pipeline:** From raw ViZDoom installation to agent training and evaluation.
- 🧪 **Multiple RL experiments** across different game scenarios: Basic, Defend the Center, Deadly Corridor.
- 📊 **Visualization** of learning curves, reward progression, and agent performance.
- ⚙️ **Custom wrappers** to make ViZDoom compatible with OpenAI Gym.
- 🧠 **Integration with Stable Baselines3** for fast experimentation with state-of-the-art RL algorithms.

---

## 📁 Table of Contents

- [Project Overview](#project-overview)
- [Notebook Descriptions](#notebook-descriptions)
- [Installation & Setup](#installation--setup)
- [Usage Guide](#usage-guide)
- [Directory Structure](#directory-structure)
- [License](#license)
- [Acknowledgments](#acknowledgments)

---

## 🚀 Project Overview

The goal of this project is to explore how RL agents learn in complex visual environments using ViZDoom — a platform built on the classic Doom FPS game. The project includes:

- Environment setup and Gym-compatible wrappers.
- Designing custom action/state spaces.
- Training agents using PPO/DQN/A2C via Stable Baselines3.
- Benchmarking performance on various ViZDoom scenarios.
- Visualizing and logging agent learning and game progress.

**This project is suitable for:**

- Students and researchers exploring visual RL.
- Game AI enthusiasts.
- Developers interested in sim-to-real RL pipelines.

---

## 📓 Notebook Descriptions

| Notebook                 | Description                                                                                              |
|--------------------------|----------------------------------------------------------------------------------------------------------|
| `Doom.ipynb`             | ✅ Initial setup: Installing ViZDoom and creating a Gym wrapper. Demonstrates agent interaction in a basic environment. |
| `Doom1.ipynb`            | 🔍 Extended experiments on alternate maps or training variations.                                         |
| `DoomDefend.ipynb`       | 🛡️ Implements an agent learning the “Defend the Center” scenario — a classic ViZDoom test case.          |
| `Doomdefendcenter.ipynb` | 🧠 Further experiments optimizing reward structures and state representations in "Defend the Center".     |
| `doomdeadlycorrdior.ipynb` | ☠️ Trains agents in the challenging “Deadly Corridor” scenario using complex navigation and survival skills. |

Each notebook is well-commented and modular — ideal for both beginners and researchers to modify or extend.

---

## 🛠️ Installation & Setup

### 📋 Prerequisites

- Python 3.7+
- [Anaconda](https://www.anaconda.com/products/individual) (Recommended)
- Jupyter Notebook or JupyterLab
- GPU (optional but recommended for faster training)

### 📦 Installation Steps

#### 1. Clone the Repository
```bash
git clone https://github.com/HeroicKrishna160905/Doom.git
cd Doom
```

#### 2. Create and Activate Conda Environment (Optional but Recommended)
```bash
conda create -n doom-rl python=3.11
conda activate doom-rl
```

#### 3. Install Dependencies
```bash
pip install gym numpy opencv-python matplotlib stable-baselines3 vizdoom
```

#### 4. Download ViZDoom Scenarios
Some notebooks rely on scenarios from the ViZDoom GitHub repository.

```bash
git clone https://github.com/mwydmuch/ViZDoom
```
Copy relevant `.cfg` files from `ViZDoom/scenarios/` into your working directory.

📘 For advanced configuration, refer to [ViZDoom’s documentation](https://github.com/mwydmuch/ViZDoom).

---

## ▶️ Usage Guide

To run a specific experiment:
```bash
jupyter notebook Doom.ipynb
```

- Change training parameters (steps, learning rate, gamma, etc.) directly in the notebook.
- Evaluate trained agents using rendered gameplay or reward plots.
- Save models and reload them for further fine-tuning.
- 🧪 You can use TensorBoard or matplotlib for visualizing training curves and agent behavior.

---

## 🗂️ Directory Structure

```
doom-rl/
├── Doom.ipynb
├── Doom1.ipynb
├── DoomDefend.ipynb
├── Doomdefendcenter.ipynb
├── doomdeadlycorrdior.ipynb
├── LICENSE
└── .gitignore
```

---

## ⚖️ License

This project is open-sourced under the terms of the MIT License.

---

## 🙌 Acknowledgments

- **ViZDoom:** The Doom-based RL environment.
- **OpenAI Gym:** Standardized interface for RL environments.
- **Stable Baselines3:** Reliable implementations of modern RL algorithms.

---

## 💡 Future Plans

- Integrate curriculum learning across Doom scenarios.
- Benchmark various RL algorithms (e.g., PPO vs DQN vs A2C).
- Extend to 3D navigation and multi-agent reinforcement learning.
- Add logging with TensorBoard or Weights & Biases.

---

📬 **For collaboration, feel free to fork the repository or open an issue/pull request.**  
Built with curiosity and Doomguy’s spirit. 🕹️
