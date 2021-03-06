# CS202 Programming Assignment 2

## Question:

Implement a SAT solver. Given a formula in the DIMACS representation, your implementation should return:
1) a model if the formula is satisfiable
2) report that the formula is unsatisfiable
You are free to use any language and algorithm (Semantic Tableau, Analytic Tableau, DPLL or a combination).


## SAT Solver:

We have implemented Sat Solving by using backtracking algorithm, recursive function.

This recursive function recursivly checks for satisfiability after assigning a truth value to literals till it assigns to all literals. Also, backtracks if found unsat and continue with literal's negation till we check for every case. Function gives ```1``` in case of sat and ```0``` in case of unsat with stored model in ```result``` vector defined globaly.

#### How to run:

-> Compile the cpp file "sat_solver.cpp" using g++ compiler using the command "g++ sat_solver.cpp".
-> Invoke the executable file "sat_solver" to run the program by typing "./sat_solver".
-> At first, it asks for the input cnf file path then for the output txt file path to get result .
->The solution can be found in the file "output.txt" after the code has been executed.
This output file may contain ```SAT``` and the model in case of satisfiability and ```UNSAT``` in case of unsatisfiability.
