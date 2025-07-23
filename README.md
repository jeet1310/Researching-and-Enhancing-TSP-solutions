# 🚚 Traveling Salesman Problem (TSP) Solver – Hybrid Optimization

This project focuses on solving the **Traveling Salesman Problem (TSP)** using a combination of classical and metaheuristic algorithms. It also extends the single-vehicle TSP to a **multi-vehicle** routing problem.

## 📌 Features

- ✅ **Christofides Algorithm** implementation for TSP
- 🔁 **Multi-Vehicle TSP Extension** (4 vehicles) with depot handling
- 🔍 Metaheuristic experiments:
  - Simulated Annealing
  - Ant Colony Optimization
- 📉 Fallback mechanism using **Kruskal’s Algorithm** when custom logic fails
- 📊 Visualization of TSP routes using `matplotlib` and `networkx`


---

## 🧠 Algorithms Used

### 1. Christofides Algorithm
An approximation algorithm for metric TSP that guarantees a solution within 1.5× of the optimal.

### 2. Custom Path Generator (FAILED FOR >12 NODES)
Initially attempted a formula-based route generation. Failed on larger graphs.

### 3. Kruskal’s Algorithm (Fallback)
Used to construct a Minimum Spanning Tree and generate a DFS-based tour when the custom path failed.

### 4. Simulated Annealing
Used for optimization by escaping local minima through probabilistic search.

### 5. Ant Colony Optimization
Inspired by real ants’ foraging behavior, explored for large-node graphs (slow but reliable).

---

## 🚗 Multi-Vehicle Extension

- Nodes divided into **k = 4** groups
- Each vehicle starts and ends at the **depot (node 0)**
- Ensures **no city is visited more than once**

---

## 🧰 Tech Stack

- Python 3.10+
- `networkx`
- `matplotlib`
- `numpy`

---

---

## ⚠️ Known Limitations

- The initial custom algorithm failed when scaled to >12 nodes.
- Metaheuristic parameters (cooling schedule, pheromone decay, etc.) require tuning.

---

## ✨ Future Improvements

- Integrate traffic/weather constraints
- Dynamic route recalculation in real-time
- Deploy as a web-based logistics optimizer

---

## 👤 Author

**Jeet Jain**  
4th Year Computer Engineering  
NMIMS Navi Mumbai

---

## 📄 License

MIT License – feel free to use, modify, and share.



