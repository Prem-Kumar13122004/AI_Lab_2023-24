# Ex.No: 2  Implementation of Depth First Search                                                                           
### REGISTER NUMBER : 212222040123
### AIM: 
To write a python program to implement Depth first Search. 
### Algorithm:
1. Start the program
2. Create the graph by using adjacency list representation
3. Define a function dfs and take the set “visited” is empty 
4. Search start with initial node. Check the node is not visited then print the node.
5. For each neighbor node, recursively invoke the dfs search.
6. Call the dfs function by passing arguments visited, graph and starting node.
7. Stop the program.
   ```













   ```
   ```







   ```
### Program:
```
# Using a Python dictionary to act as an adjacency list
graph = {
    '5': ['3', '7'],
    '3': ['2', '4'],
    '7': ['8'],
    '2': [],
    '4': ['8'],
    '8': []
}

visited = set()  # Set to keep track of visited nodes of the graph.

def dfs(visited, graph, node):  # Function for DFS
    if node not in visited:
        print(node)
        visited.add(node)
        for neighbour in graph[node]:
            dfs(visited, graph, neighbour)

# Driver Code
print("Following is the Depth-First Search")
dfs(visited, graph, '5')
```










### Output:
![Ex no 2 DFS](https://github.com/user-attachments/assets/7077a905-6faf-4903-93b2-426486a29b31)



### Result:
Thus the depth first search order was found sucessfully.
