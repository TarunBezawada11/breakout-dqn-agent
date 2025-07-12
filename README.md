# 🎮 Deep Q-Network (DQN) for Atari Breakout  
**CS6482 – Deep Reinforcement Learning Project**

Train an AI agent to master Atari Breakout using advanced reinforcement learning techniques like **Dueling DQN** and **Prioritized Experience Replay (PER)**.

---

## 🚀 Project Highlights

- 📈 Achieved **average reward of 21.67** by version **v10**
- 🧠 Implemented **Vanilla DQN**, **Dueling DQN**, and **PER**
- 🖼️ Preprocessed game frames using **OpenCV** and **scikit-image**
- 🧪 Trained the agent over **5,000 episodes** using Q-learning with a CNN-based policy network
- ⚙️ Training performed on **NVIDIA A100 GPU** for high-throughput learning

---

## 🛠️ Technologies Used

| Tool/Library     | Purpose                                       |
|------------------|-----------------------------------------------|
| **PyTorch**       | Deep Q-Network and CNN implementation         |
| **OpenAI Gym**    | Atari Breakout environment (ALE/Breakout-v5) |
| **ALE-Py**        | Support for Atari Learning Environment        |
| **OpenCV**        | Frame preprocessing (grayscale, resize)      |
| **Scikit-Image**  | Advanced image transformations                |
| **NumPy**         | Numerical computations                        |
| **Matplotlib**    | Reward/loss visualization                     |

---

## 🧠 Skills Demonstrated

- **Reinforcement Learning**  
  Q-learning with Bellman updates, ε-greedy exploration, and experience replay

- **Deep Learning**  
  Designed a 5-layer CNN to process 84×84×4 grayscale stacked frames

- **Optimization**  
  Used Prioritized Experience Replay (PER) and fine-tuned learning rate (0.0002)

- **Data Engineering**  
  Frame preprocessing, stacking, and efficient buffer management

- **Evaluation**  
  Plotted reward curves and Q-loss to track learning progression

- **Software Engineering**  
  Modular, version-controlled codebase (tracked from v1 → v10)

---

## 📊 Results Summary

| Version | Method         | Avg. Reward |
|---------|----------------|-------------|
| v1      | Vanilla DQN    | 1.90        |
| v5      | Dueling DQN    | 12.5 – 15   |
| v10     | DQN + PER      | **21.67**   |

🕒 **Training Time**: ~14.5 hours on NVIDIA A100 GPU

---

## 📉 Visual Insights

### 📈 Reward Curve  
Demonstrates the agent’s learning progress and long-term performance.

### 📉 Loss Curve  
Indicates the convergence behavior of Q-values during training.
https://github.com/TarunBezawada11/breakout-dqn-agent/blob/main/rewards_curve.png
## 💻 Compute & Infrastructure

- **GPU**: NVIDIA A100 (80GB HBM2e)
- **Replay Buffer**: ~1M transitions
- **Input**: 84×84×4 frame stacks
- **Model**: CNN with millions of parameters, using target network updates

---

## 🔧 Getting Started

```bash
# Clone the repository
git clone https://github.com/BlachThunder6302/CS6482-DQN-Breakout.git

# Install dependencies
pip install -r requirements.txt

# Launch the notebook
jupyter notebook CS6482-DQN-Atari.ipynb
