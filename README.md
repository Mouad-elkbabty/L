   
   
   The objective of this project is to provides a solution to every solvable Light-Up (or Akari) grid. The processus is rather simple : We have modelized the game's rules (see lower) in a formula in propositionnal formula, then we have transformed this formula in a DIMACS's file, a file that we can solves thanks to a SAT-Solver. The SAT-SOLVER used was also implemented by ourselves using the DPLL algorithm.
   
   
   
   Rules of the game :
   The grid is composed of 3 types of cells : white, black whitout number and black with. Here are the rules :

The player places light bulbs in white cells such that no two bulbs shine on each other, until the entire grid is lit up.
A bulb sends rays of light horizontally and vertically, illuminating its entire row and column unless its light is blocked by a black cell.
A black cell may have a number on it from 0 to 4, indicating how many bulbs must be placed adjacent to its four sides; for example, a cell with a 4 must have four bulbs around it, one on each side, and a cell with a 0 cannot have a bulb next to any of its sides.
An unnumbered black cell may have any number of light bulbs adjacent to it, or none. Bulbs placed diagonally adjacent to a numbered cell do not contribute to the bulb count.
   
