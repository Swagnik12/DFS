# DFS
- Python implementation of Depth-First Search (DFS) algorithm for graph traversal.
- Breakdown of the code <br>

- **Initialization :**<br>
 - **graph:** This dictionary represents the graph. Keys are nodes (vertices), and their corresponding values are lists of their adjacent nodes.<br>
 - **start_node:** This variable stores the starting node for the DFS traversal.<br>
 - **visited:** A set is used to keep track of nodes that have already been visited, preventing cycles.<br>
 - **stack:** A list (which acts as a stack using the pop() method) is used to store nodes to be explored. Initially, it contains only the start_node.<br>

 - **DFS Traversal**<br>

- **while stack:** The loop continues as long as there are nodes in the stack.<br>
  - **current_node = stack.pop():** The topmost node from the stack is popped (removed) and assigned to current_node.<br>
- **if current_node not in visited:**<br>
  - **print(current_node, end=""):** If the current node has not been visited before, it is printed.<br>
  - **visited.add(current_node):** The current node is added to the visited set.<br>
- **for neighbor in graph[current_node]:**<br>
  - **if neighbor not in visited:** If a neighbor of the current node has not been visited:<br>
    - **stack.append(neighbor):** The neighbor is pushed (added) onto the stack for exploration later.<br>

  **OUTPUT**: A D C G E F
