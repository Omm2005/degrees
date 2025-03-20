# Degrees

A Python implementation of the **Degrees of Separation** problem using **graph search algorithms**. This project explores the shortest connection path between actors using **Breadth-First Search (BFS)** and **A* Search (A-Star Algorithm)**.

---

## 📌 README: How to Use  

### Features  
✅ Finds the shortest connection path between two actors.  
✅ Implements **BFS** for simple shortest path searches.  
✅ Implements **A*** for optimized pathfinding using heuristic estimation.  
✅ Works with large actor-movie datasets.  

### Installation  
1. Clone the repository:  
   ```bash
   git clone https://github.com/Omm2005/degrees.git
   cd degrees
   ```  
2. Install dependencies (if required):  
   ```bash
   pip install -r requirements.txt
   ```  

### Usage  
Run the script and enter the names of two actors to find their degree of separation:  
```bash
python degrees.py
```  

#### Example Output  
```
Enter source actor: Tom Hanks  
Enter target actor: Emma Watson  
Tom Hanks → Saving Mr. Banks → Paul Giamatti  
Paul Giamatti → The Nanny Diaries → Scarlett Johansson  
Scarlett Johansson → The Island → Ewan McGregor  
Ewan McGregor → Beauty and the Beast → Emma Watson  
```
**Degrees of separation: 3**  

---

## 🚀 Contributing  
If you want to contribute:  
1. Fork the repository.  
2. Create a new branch (`feature-branch`).  
3. Commit your changes.  
4. Submit a Pull Request (PR).  

All contributions are welcome, from bug fixes to performance improvements.

---

## 📜 License  
This project is licensed under the **MIT License**.

---

### 🔗 Acknowledgments  
- **CS50 AI**: Inspiration for the project structure.  
- **Graph Theory & Pathfinding Algorithms**: Core concepts used in implementation.  
- **IMDb Dataset**: Source of actor-movie relationships.  