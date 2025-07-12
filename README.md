# 🎮 Deep Q-Network (DQN) for Atari Breakout  
**CS6482 – Deep Reinforcement Learning Project**

Train an AI agent to master Atari Breakout using modern reinforcement learning techniques like **Dueling DQN** and **Prioritized Experience Replay (PER)**. This project was developed as part of the coursework for CS6482 – Deep Reinforcement Learning.

---

## 🚀 Project Highlights

- 📈 Achieved an average reward of **21.67** by version **v10**
- 🧠 Implemented **Vanilla DQN**, **Dueling DQN**, and **PER**
- 🖼️ Preprocessed input frames using **OpenCV** and **scikit-image**
- 🧪 Trained over **5,000 episodes** with a CNN-based policy network
- ⚙️ Trained on **NVIDIA A100 GPU** for high-throughput learning

---

## 🛠️ Technologies Used

| Tool/Library     | Purpose                                       |
|------------------|-----------------------------------------------|
| **PyTorch**       | DQN and CNN model implementation              |
| **OpenAI Gym**    | Atari Breakout environment (`ALE/Breakout-v5`)|
| **ALE-Py**        | Atari Learning Environment interface          |
| **OpenCV**        | Frame preprocessing (grayscale, resize)       |
| **Scikit-Image**  | Image transformations                         |
| **NumPy**         | Numerical computations                        |
| **Matplotlib**    | Visualization of training progress            |

---

## 🧠 Skills Demonstrated

- **Reinforcement Learning**: Q-learning, Bellman updates, ε-greedy policy, experience replay  
- **Deep Learning**: Built a 5-layer CNN to process 84×84×4 stacked grayscale frames  
- **Optimization**: Used PER to prioritize valuable experiences and tuned learning rate (0.0002)  
- **Data Engineering**: Frame preprocessing, replay buffer handling, and stacking observations  
- **Evaluation**: Reward curve analysis and Q-value loss tracking  
- **Software Engineering**: Modular and version-controlled codebase (tracked from v1 to v10)  

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
Demonstrates the agent’s learning progression over training episodes:

![Reward Curve](https://github.com/TarunBezawada11/breakout-dqn-agent/blob/main/rewards_curve.png)

### 📉 Loss Curve  
Shows convergence of Q-values during training:

![Loss Curve](https://github.com/TarunBezawada11/breakout-dqn-agent/blob/main/loss_curve.png)

---

## 💻 Compute & Infrastructure

- **GPU**: NVIDIA A100 (80GB HBM2e)
- **Replay Buffer**: ~1M transitions
- **Input Shape**: 84×84×4 (stacked grayscale frames)
- **Model**: Convolutional neural network (with target network updates)

---

## 🔧 Getting Started

```bash
# Clone the repository
git clone https://github.com/TarunBezawada11/breakout-dqn-agent.git
cd breakout-dqn-agent

# Install required dependencies
pip install -r requirements.txt

# Launch the notebook
jupyter notebook CS6482-DQN-Atari.ipynb
