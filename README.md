# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A: The first step that I used in the naked twins problem was to find the cell value with len(cell) == 2. Once found, I 
try to look for its twin, i.e. the cell containing the same two values. Once found, we use constraint propagation to 
eliminate the two numbers from its peers. 

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: I added the two diagonals values to the unit list. For the solution of the problem, it did not matter how the cells
were ordered. As long as the cell addresses were provided, the solution seemed to be working. 

### Install

This project requires **Python 3**.

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project. 
Please try using the environment we provided in the Anaconda lesson of the Nanodegree.

##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

### Code

* `solutions.py` - You'll fill this in as part of your solution.
* `solution_test.py` - Do not modify this. You can test your solution by running `python solution_test.py`.
* `PySudoku.py` - Do not modify this. This is code for visualizing your solution.
* `visualize.py` - Do not modify this. This is code for visualizing your solution.

### Visualizing 

To visualize your solution, please only assign values to the values_dict using the ```assign_values``` function provided in solution.py

Based on the default value given the program, this is the visualized solution that was obtained. 
!['2.............62....1....7...6..8...3...9...7...6..4...4....8....52.............3'](images/solution.jpg?raw=true)

### Data

The data consists of a text file of diagonal sudokus for you to solve.