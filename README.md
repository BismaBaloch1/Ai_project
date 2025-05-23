# ♟️ HexAI - AI Strategy for the Game of Hex

**HexAI** is a strategic AI-based implementation of the classic board game Hex, allowing gameplay between human players and artificial intelligence agents. The AI supports multiple strategies including Minimax with Alpha-Beta Pruning, Monte Carlo Tree Search (MCTS), and Reinforcement Learning. This project was developed as part of an academic exploration into advanced AI decision-making for deterministic, zero-sum board games.

---

## 👩‍💻 Built By

- **Bisma**  
- **Sadia**

**Course:** Artificial Intelligence  
**Instructor:** Alishba Subhani  
**Submission Date:** October 3, 2025

---

## 🎮 Features

✅ Play against human or AI opponents  
🤖 Choose between Minimax, Alpha-Beta, or MCTS AI  
♟️ Configurable board size  
🧠 AI difficulty scaling via heuristics and self-learning  
🚀 Optimized decision-making using transposition tables  
📊 Built-in tools for running performance experiments  

---

## 📦 Installation

Clone the repository and install dependencies using:

pip install -r requirements.txt

## How to Play

Run the main game loop:

python hexai.py

### 🎮 Optional Flags

| Option         | Action                        | Choices                      | Default |
|----------------|-------------------------------|-------------------------------|---------|
| `-p1`          | Player 1 (Blue) type          | `{human, alphabeta, mcts}`   | `human` |
| `-p2`          | Player 2 (Red) type           | `{human, alphabeta, mcts}`   | `mcts`  |
| `-s`, `--size` | Set board size                | `int`                         | `4`     |
| `-t`, `--use_tt` | Use transposition table     | `bool`                        | `False` |
| `-b`, `--begin`| Which player starts (1 or 2)  | `1 = Blue`, `2 = Red`         | `1`     |

## Experiments
Run experiments to compare different AI strategies and heuristics:

1. Alpha-Beta with/without Heuristics

python hexexperiments.py comp -o base -m

2. Iterative Deepening + Transposition Table

python hexexperiments.py comp -o idtt -m

3. MCTS Optimization

python hexexperiments.py mcts
⚠️ Note: This can take 15–20 minutes depending on CPU power.

4. MCTS vs Alpha-Beta

python hexexperiments.py comp -o mcts -m

## AI Techniques Used

Minimax Algorithm – Standard decision-making for 2-player adversarial games

Alpha-Beta Pruning – Efficiently reduces the search space in Minimax

Monte Carlo Tree Search (MCTS) – Uses simulation-based strategies for move evaluation

Reinforcement Learning (optional) – Allows AI to improve over time via self-play

Heuristics – Influence maps, shortest path (Dijkstra), and positional scoring



## Technologies Used

Language: Python

Libraries: NumPy, Pygame, Scikit-learn, TensorFlow/PyTorch (for RL)
