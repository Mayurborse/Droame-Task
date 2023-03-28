# Drone



1. Problem Definition:
The problem we are trying to solve is to find the optimal paths for multiple drones to visit a set of locations,
while minimizing the total time taken to complete the task.
2. Approach:
To solve this problem, I have taken a brute force approach that involves generating all possible paths for the
drones and then selecting the path that takes the least amount of time.
3. Libraries or Frameworks Used:
I have not used any external libraries or frameworks to construct this algorithm. The code is written in
Python, which is a popular programming language for data analysis and scientific computing. However, we
can visualize the path of drones with the help of matplotlib.
4. Explanation of the Code:
• The code defines a class called "Drone" that represents a single drone, with attributes such as its speed,
starting location, and time limit.
• Then I have defined a function called "distance" that calculates the Euclidean distance between two points
in a two-dimensional space.
• The "get_paths_helper" function is the core of the algorithm. It takes three arguments: "drones", "path", and
"paths". "drones" is a list of drone objects, "path" is a list that represents the current path being generated, and
"paths" is a list of all the paths generated so far. The function uses recursion to generate all possible paths for
the drones. For each drone, the function checks if it can reach the next location within its time limit, and if so,
it adds the location to the path and recursively calls itself with the updated path. Once all drones have visited
all locations, the function adds the path to the list of paths.
• Finally, I have defined a function called "get_paths" that calls "get_paths_helper" for each drone and returns
the list of all possible paths.
• Then I have created a list of drone objects and call the "get_paths" function to generate all possible paths. 
We then print out the paths generated for each drone.
