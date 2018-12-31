# Sudoku Solver

This program solves a Sudoku using different AI approaches like finding the Naked Twins and constraint propagation. 

Naked Twins are the boxes which are peers to each other and have the same 2 values as the possible values. Then the peers of these Naked Twins which have other values too as the possible values can't have values of twin pairs as their possible values. Hence we will eliminate these values from the list of possible values in its peers. To do this we will find the Naked Twins in the puzzle and remove in the its peers possible values. We will use depth first search to all the possible values and use the recursion to find the further Naked twins that are created after removing till we reach the final solution.

We use eliminate,only choice and Naked Twins heuristics to remove the values that are not possible to have in the peers based on the constraints. For the boxes which are on the diagonal of the sudoku we consider the vertical,horizontal and diagonal boxs too as the peers and apply all the three funtions on these boxes to reach the final solution. 


* `Sudoku-Solver.py` takes the Sudoku in the format of a vector where `.` represent the blank space in the sudoku and prints the solved Sudoku

### Visualizing

You can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

Please only assign values to the values_dict using the ```assign_values``` function provided in solution.py
