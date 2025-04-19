# 🐜 Ant Colony Optimization for Pathfinding in a Grid Environment

> A Swarm Intelligence Based Approach for Navigating Obstacle-Filled Grids  
> **Course:** CS351 - Nature Inspired Computing  
> **Department of Computer Science and Engineering**

## 👥 Team Members

- **Kaushik Sahoo** – BTECH/60070/22  
- **Ayush Kumar Kashyap** – BTECH/60075/22  
- **Rishav Kumar Raj** – BTECH/60079/22  

**Supervisor:** Mr. Rayees Ahmed

## 📘 Project Overview

Ant Colony Optimization (ACO) is a nature-inspired metaheuristic that simulates the foraging behavior of real ant colonies to solve complex computational problems. This project utilizes ACO to navigate a 5x5 grid with randomly generated obstacles, identifying the shortest path from a defined start point to a goal.

The implementation demonstrates how decentralized, collective behavior can lead to intelligent problem-solving in dynamic environments.

## 🎯 Objective

To implement the Ant Colony Optimization algorithm for pathfinding in a 2D grid environment with obstacles, and to observe its performance in terms of path quality and computational efficiency.


## 🧪 Problem Specification

- **Grid Dimensions:** 5 x 5  
- **Start Point:** (0, 0)  
- **Goal Point:** (4, 4)  
- **Obstacles:** 20% of grid cells, placed randomly  
- **Goal:** Identify the shortest valid path avoiding obstacles


## ⚙️ Algorithm Parameters

| Parameter          | Value | Description                            |
|-------------------|-------|----------------------------------------|
| Alpha (α)         | 1.0   | Influence of pheromone concentration   |
| Beta (β)          | 2.0   | Influence of heuristic (distance)      |
| Evaporation Rate  | 0.5   | Rate at which pheromones decay         |
| Pheromone Deposit | 100   | Total pheromone laid per path          |
| Number of Ants    | 10    | Number of agents per iteration         |
| Iterations        | 20    | Number of simulation cycles            |


## 🧱 Key Components

### 🧩 Grid Generation
```python
def generate_grid():
    # Creates a 5x5 grid and populates it with random obstacles (20% cells)
```

### 🚶 Ant Movement
```python
def choose_next(current, visited, grid, pheromones):
    # Uses pheromone levels and heuristics to probabilistically choose next cell
```

### 🔁 Pheromone Update
```python
def update_pheromones(paths, pheromones):
    # Increases pheromone along successful paths and evaporates others
```

## 🧾 Visualization

Each iteration displays the grid with:

- `S` — Start  
- `G` — Goal  
- `#` — Obstacle  
- `*` — Ant path  

The best path found is visualized after all iterations complete.

## 📊 Results & Observations

- ACO consistently finds optimal or near-optimal paths.
- Balance between **exploration** (via evaporation) and **exploitation** (via pheromone deposition) is critical.
- Varying the number of ants and iterations affects performance and convergence rate.

## ✅ Advantages

- ✅ Decentralized decision-making  
- ✅ Scalable to larger and more complex grids  
- ✅ Adaptable to dynamic environments  

## ⚠️ Limitations & Future Enhancements

- ⚠️ Susceptible to local optima  
- ⚠️ Performance may vary due to stochastic behavior

**Future Improvements:**
- 🔁 Introduce backtracking to avoid dead-ends
- 🔀 Combine with other algorithms (e.g., Dijkstra, Genetic Algorithms)
- 📈 Tune parameters adaptively based on progress

## 🧠 Conclusion

Ant Colony Optimization is an effective, biologically inspired technique for solving pathfinding problems in constrained environments. This implementation highlights its robustness and adaptability, with potential for enhancement through hybrid models and intelligent parameter tuning.

## 📂 Repository Structure

📁 ACO-Grid-Pathfinding/
├── 📜 README.md
├── 🐍 aco_pathfinding.py
├── 📊 results/
└── 📸 screenshots/

## 📌 References

- Dorigo, M., & Stützle, T. (2004). *Ant Colony Optimization*. MIT Press.  
- Nature-Inspired Computing Course Material – CS351  


## 📝 License

This project is for academic and educational purposes only. Please contact the authors for permission if you intend to use it for commercial purposes.
