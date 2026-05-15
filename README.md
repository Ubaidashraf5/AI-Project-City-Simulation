# AI-Project-City-Simulation
AI-based city layout and routing project
# 🏙️ CityMind — AI-Based Urban Intelligence System

> An AI-powered city layout planning and emergency routing simulation built with Python.

---

## 👥 Team Members

| Name | Student ID | Contributions |
|------|-----------|------|
| Ubaid Ashraf | 24I-0841 | Challenge 3: Full Genetic Algorithm for ambulance placement.    Challenge 4: A* routing with real-time re-routing and graceful unreachable-civilian handling. |
| Muhammad Shahzaib Khan | 24I-0741 | Challenge 1: CSP with backtracking and forward checking, Primary Hospital identification.    Challenge 2: Kruskal MST with forced redundancy between Primary Hospital and Primary Depot. |
| Mitul Dial | 24I-0791 | Challenge 5: Full ML pipeline — K-Means, synthetic data generation, Decision Tree, graph integration. Pygame UI: Grid rendering, three overlay modes, event log, status bar. |

---

## 📌 Project Overview

**CityMind** is an intelligent city simulation system that uses multiple AI techniques to plan urban layouts, optimize infrastructure networks, and route emergency vehicles in real time. The project is built on a 15×15 grid city map with various building types, a river system, and flood simulation.

---

## 🧠 AI Challenges Implemented

### Challenge 1 — City Layout (CSP)
- Constraint Satisfaction Problem to place buildings intelligently
- Rules: Hospitals away from Industrial zones, Schools near Residential areas, etc.
- Building types: Residential, Hospital, School, Industrial, PowerPlant, AmbulanceDepot

### Challenge 2 — Network Infrastructure (MST)
- Minimum Spanning Tree using Kruskal's algorithm with Union-Find
- Connects all city nodes with minimum road cost
- BFS-based connectivity checks

### Challenge 3 — Optimization (Genetic Algorithm)
- Genetic Algorithm to optimize city layout fitness
- Fitness function based on proximity of emergency services to population
- Crossover, mutation, and selection operations

### Challenge 4 — Emergency Routing (A* Search)
- A* pathfinding for ambulance routing
- Manhattan distance heuristic
- Avoids blocked/flooded roads in real time

### Challenge 5 — Risk Analysis (Machine Learning)
- K-Means clustering to group city zones by risk level
- Decision Tree classifier to predict flood risk
- Feature extraction based on population density and building type

---

## 🗂️ Project Structure

```
AI-Project-City-Simulation/
│
├── main.py                  # Entry point — launches CityMind
├── city_graph.py            # Core city grid and node/edge structure
├── ui.py                    # Pygame-based visual interface
├── flood_simulation.py      # Flood spreading simulation
│
├── challenge1_layout.py     # CSP-based building placement
├── challenge2_network.py    # MST network construction
├── challenge3_ga.py         # Genetic Algorithm optimization
├── challenge4_routing.py    # A* emergency routing
├── challenge5_ml.py         # ML risk analysis (KMeans + Decision Tree)
│
├── assets/                  # Images, fonts, sounds
│   ├── ambulance.png
│   ├── hospital.png
│   ├── residential.png
│   └── ...
│
├── 24I-0741_24I-0841_24I-0791_Phase1-report.pdf
└── 24I-0741_24I-0841_24I-0791_FinalReport.pdf
```

---

## 🛠️ Technologies Used

- **Python 3.x**
- **Pygame** — Visual UI and simulation
- **NumPy** — Numerical computations
- **scikit-learn** — KMeans clustering, Decision Tree
- **Standard Libraries** — `heapq`, `collections`, `random`, `math`

---

## ▶️ How to Run

### 1. Install Dependencies
```bash
pip install pygame numpy scikit-learn
```

### 2. Run the Project
```bash
python main.py
```

### 3. In the UI
- Click **CSP** — to apply constraint-based city layout
- Click **MST** — to build the road/power network
- Click **GA** — to run genetic algorithm optimization
- Click **Route** — to find ambulance path
- Click **Flood** — to simulate flood spread

---

## 📄 Reports

- 📘 [Phase 1 Report](./24I-0741_24I-0841_24I-0791_Phase1-report.pdf)
- 📗 [Final Report](./24I-0741_24I-0841_24I-0791_FinalReport.pdf)

---

## 🏫 Course Info

**Artificial Intelligence** — $th Semester Project  
FAST National University of Computer and Emerging Sciences (NUCES)
