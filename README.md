# 🥋 A3C for Kung Fu

This project implements the **Asynchronous Advantage Actor-Critic (A3C)** reinforcement learning algorithm to train an AI agent to play the classic **Kung Fu** arcade game.  
The agent learns effective fighting strategies by playing multiple parallel instances of the environment, improving stability and training speed.

---

## 🧠 Key Features

- 🎮 **Environment**: Kung Fu arcade game (Atari) with Gymnasium/ALE.  
- 🤖 **A3C Algorithm**: Multi-threaded training with asynchronous agents.  
- 🧠 **Actor-Critic Network**: Combines policy (actor) and value (critic) learning.  
- 📦 **Entropy Regularization**: Encourages exploration and avoids premature convergence.  
- 📊 **Performance Monitoring**: Tracks episode rewards and training progress.  
- 📽️ **Gameplay Recording**: Saves videos of the trained agent in action.  

---

## 📽 Demo Video

Watch the trained agent play **Kung Fu**:  

[![Kung Fu Demo](demo_video.mp4)](demo_video.mp4)

---

## 🛠 Requirements

Install the dependencies:

```bash
pip install gymnasium[atari,accept-rom-license] torch torchvision numpy imageio
```

## ✅ How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/A3C_for_Kung_Fu.git
   cd A3C_for_Kung_Fu
   ```

2. Open and run the Jupyter notebook:
   ```bash
   jupyter notebook A3C_for_Kung_Fu.ipynb
   ```

3. Training will begin, and logs will show the agent’s average scores.

4. After training, a demo video `demo_video.mp4` will be generated..


## 📊 Sample Output

```
  0%|          | 6/3001 [01:59<12:09:52, 14.62s/it] Average agent reward : 620.0
 34%|███▎      | 1007/3001 [04:09<2:01:36,  3.66s/it]Average agent reward : 510.0
 67%|██████▋   | 2012/3001 [06:30<1:11:28,  4.34s/it]Average agent reward : 1120.0
100%|██████████| 3001/3001 [08:55<00:00,  5.60it/s]Average agent reward : 920.0
```

---
## 📂 Project Structure

- `A3C_for_Kung_Fu.ipynb`: Jupyter Notebook with the full training pipeline..
- `demo_video.mp4`:Demo video of the trained agent.
- `checkpoint.pth`: Model weights saved after successful training (if enabled).

---

## 🧠 Network Architecture

- Shared CNN Layers: Extract visual features from game frames.
- Actor Head: Outputs action probabilities.
- Critic Head: Estimates state values.
- Loss Function: Combines policy gradient, value loss, and entropy bonus.

---

## 🎯 Learning Objective

This project showcases how asynchronous reinforcement learning can be applied to challenging environments. By running multiple agents in parallel, A3C accelerates learning and enables an agent to develop complex strategies for mastering Kung Fu gameplay.

---


## 📄 License

This project is open-source and available under the MIT License.  
See the [LICENSE](LICENSE) file for more information.
