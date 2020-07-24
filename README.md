# Introduction-to-Robot-Programming
This is a C++ and ROS based course. All the assignments are done in C++.

# Project 1

Problem statement is in the Project 1 folder

# Project 2

## Structure of Robot Navigation in a Maze

Problem statement is in the Project 2 folder

### How to execute

##### NOTE: This has been tested on codelite platform only! Also, c++11 has been used for development.

##### Few sub-notes:
* `Assignment` folder is the workspace folder. It contains `.workspace` file which can be loaded into your codelite environment. 
* Doxygen documentation can be viewed by cloning the repo and navigating to `documentation/docs/html` and open `index.html` in your local browser.
* Every input being asked contains two values: First being row number, second being column number.
* The grid is designed such that (0, 0) is top-left corner of the map. row and column indices increase downwards (row) and towards right (column).
* Code is designed to accept both ( ) i.e. freespace and (.) i.e. dot as input from map. However, obstacle has to be (#).

#### Execution Note!
##### Input file is by default taken from `Assignment` directory i.e. it has been coded with relative path.
##### If the existing code does not work (i.e. input file error!), please change the following and run the code.
* line #160 in `main.cpp` where `std::string path` has been defined. Change the value to path in your system before executing the code. (Please specify absolute path!)

##### Sample execution:
Few observations:
* \# corresponds to obstacle
* \+ corresponds to partial (when goal is not reached), else path to goal (G) from start (S) node.
![sample_output](https://user-images.githubusercontent.com/47953521/88437872-6e458780-cdd5-11ea-9b29-03081232c117.png)


# Project 3

## Create a structure of two mobile robots in a maze to pickup the objects

Problem statement is in the Project 3 folder

## Explanation

In this project, we were given two mobile robots in a maze to pickup the objects. We had to write the structure of the project using OOP Inheritance and Polymorphism.

The first one belonged to the Landbasedwheeled type and the second one was LandbasedTracked type. Both classes derived from Landbasedrobot class. The Landbasedrobot had many data members ike speed, width, length, height which were private and many member functions like goup, go down, turn right, turn left to write codes for the different directions the robot moves. Similarly, Landbasedwheeled had attributes like wheel number to record the number of wheels mounted on the robot.

So in the program, we created Landbasedrobot as an abstract class so that the functions in it can be written virtual and be overridden in the derived classes. After that, the Landbasedwheeled and Landbasedtracked classes derived from the base class. Attributes of the base class and the derived class were declared protected and all the member functions were declared public. Then the constructors and the destructors for the base class were written. We used a UML diagram to depict this structure.

### How to execute

PLease follow the following steps to run the program file.

Steps:

1) Open the RWA3-Group10.workspace in your codelite environment.
2) Open the main.cpp file under the src folder inside the workspace.
3) RUn the main.cpp file and the output will be shown in the output terminal.

## Final Project

# Robot navigation in a Maze to the center of the Maze

Problem statement is in the Final Project folder

## Explanation

In this project, we were provided a turtlebot and the aim was to find the optimal path for this bot from the start point to the goal point that was in the middle of the maze. This project was done in C++ using data structures and we implemented Breadth First search and Depth First Search algorithms using recursion and backtracking to find the optimal path. Then we documented the code.

BFS is a traversing algorithm where you should start traversing from a starting node which is selected and traverse the graph layerwise thus exploring the neighbor nodes connected to the source. It uses a queue data structure.
1. Move horizontally and visit all the nodes of the current layer by putting them in the queue.
2. Move to the next layer.
3. Repeat the process until queue is empty.

DFS is a recursive algorithm that uses backtracking. It uses a stack to store the addresses of the nodes. The idea is that it visits all the nodes on the current path till all the unvisited nodes have been traversed before selecting the next path. Let me explain this to you in steps.
1. Pick a starting node and put all the adj nodes into a stack. Move vertically.
2. Pop a node from the stack to select the next node to visit and push all its adj nodes into the stack.
3. Repeat this process until stack is empty but ensure that the nodes that are visited are marked.

The final outcome was that BFS worked better than DFS in this case as the maze was convoluted.  Sometimes, DFS would get stuck in the local minima and displayed that no solution exists.

### How to execute

PLease follow the following steps to run the program file.

Steps:

1) Open the RWA3-Group10.workspace in your codelite environment.
2) Open the main.cpp file under the src folder inside the workspace.
3) RUn the main.cpp file and the output will be shown in the output terminal.


### Output Video

![bfs](https://user-images.githubusercontent.com/47953521/88436528-7819bb80-cdd2-11ea-953b-db2ac982337d.gif)

Breadth First Search Traversal
