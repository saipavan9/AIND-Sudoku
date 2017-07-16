# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

To test the solution, run 

```
python solution_test.py
```
To test solution, run 

```  
python solution.py
```


# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A: To find the naked twins,Firstly We tried to find the boxes having the values with length 2, this is an local constraint which helped me to shortlist from 81 boxes.
Secondly, the naked twins are the one which are same and are peers. From the result obtained from first step,I tried to find peers of each result and apply a local contraint i.e, having the same value.
The last step, is to find the common peers for both the naked twins and eliminate the twins values from the other boxes.In this way,Constraint propagation played a major part in solving the naked twins problem.  

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: Constraint propagation made the solution easier to solve the diagonal sudoku problem. We tried to solve the normal sudoku problem using constraint propagation by constraining that the peers of each box should have 1 to 9 and should not repeat itself.
We constrained by a row, coloumn and the unit square.In a similar fashion for a diagonal sudoku problem, we need constrain it by not allowing the repetition in diagonals.We simply try to make the diagonals as also the peers and solve the problem in the old 
fashioned manner i.e normal sudoku problem
