
## Full Explanation  

### Graph Representation  
The dataset is structured as a **graph**, where:  
- **Nodes** represent actors.  
- **Edges** represent movies that connect actors.  

The program builds this graph from a dataset containing actors and their corresponding movies, then uses **graph search algorithms** to determine the shortest path between two given actors.

### Algorithms Used  

#### 1️⃣ Breadth-First Search (BFS)  
BFS is an **uninformed search algorithm** that explores the shortest path level by level, making it ideal for finding **unweighted shortest paths** in a graph.  

- **Time Complexity**: \(O(V + E)\), where \(V\) is the number of vertices (actors) and \(E\) is the number of edges (movies).  
- **Advantages**: Always finds the shortest path in an unweighted graph.  
- **Disadvantages**: Can be slow for large graphs with many nodes.  

#### 2️⃣ A* Search Algorithm (A-Star)  
A* is an **informed search algorithm** that uses a **heuristic function** to prioritize which nodes to explore first.  

It follows this cost function:  
\[
f(n) = g(n) + h(n)
\]  
where:  
- \(g(n)\) = the actual cost from the start node to the current node.  
- \(h(n)\) = the estimated cost from the current node to the goal (heuristic).  

For this problem, the **heuristic function** can be estimated using the number of remaining connections based on movie links.  

- **Time Complexity**: \(O(E)\) in the worst case, but significantly faster with a good heuristic.  
- **Advantages**: More efficient than BFS when searching large graphs.  
- **Disadvantages**: Requires a well-designed heuristic to avoid unnecessary computations.  

---

### Dataset Structure  
The dataset consists of actors and movies, formatted as:  
```csv
actor_id, actor_name
movie_id, movie_title
movie_id, actor_id
```
This structure allows quick lookups and efficient graph construction.

---

### Performance Comparison  

| Algorithm  | Time Complexity | Space Complexity | Use Case |
|------------|---------------|----------------|-----------|
| **BFS**   | \(O(V + E)\) | \(O(V)\) | Guaranteed shortest path, but slow for large datasets |
| **A***   | \(O(E)\) (worst case) | \(O(V)\) | Faster than BFS with a good heuristic |

A* generally performs better in scenarios where we can estimate the distance to the goal.
