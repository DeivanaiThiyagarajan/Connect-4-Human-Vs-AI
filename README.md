# 🎮 Connect Four – Human vs Computer (AI)

## 📌 Overview
This project implements a **Human vs Computer Connect Four game**, where the AI selects its moves using a **data-driven approach**.

The AI is built using:
- An original dataset that predicts the **winner of a game state**
- A derived dataset that maps each board state to the **best possible next move**

---

## 🧠 Approach
1. The original dataset (`connectfour.data`) contains board states labeled with the predicted winner.
2. This data is processed to generate a new dataset (`Connect_Four_Best_Move.csv`) that stores the **optimal move** for each player in a given state.
3. During gameplay, the AI:
   - Evaluates the current board state
   - Uses the derived dataset to predict the **best next move**
4. A human player competes against this AI in a full Connect Four game.

---

## 📂 Files in This Repository

- **`connectfour.data`**  
  Original dataset used to predict the winner of a Connect Four game for a given board state.

- **`Connect_Four_Best_Move.csv`**  
  Derived dataset containing the best possible move for each player based on predicted game outcomes.

- **`ConnectFourHumanVsComputerGame.py`**  
  Python implementation of the Human vs AI Connect Four game.

- **`Connect_Four_HvsC.ipynb`**  
  Jupyter Notebook used to process the original `.data` file and generate the `.csv` dataset for best move prediction.

---

## 🎯 Key Outcome
This project demonstrates how **game outcome prediction** can be transformed into a **best-move dataset** and used to build a functional AI opponent without exhaustive search.
