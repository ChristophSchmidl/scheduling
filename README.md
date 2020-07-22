# The scheduling problem

## Books

- [ ] Scheduling: Theory, Algorithms, and Systems (2016) by **Michael L. Pinedo** (recommended)
- [ ] Essentials of Metaheuristics (Second Edition) by **Sean Luke** (recommended)
- [ ] Metaheuristics: From Design to Implementation by **El-Ghazali Talbi** (recommended!)
- [ ] Flow Shop Scheduling: Theoretical Results, Algorithms, and Applications by **Hamilton Emmons and George Vairaktarakis**
- [ ] Maschinenbelegungsplanung in der Variantenfertigung: Job-Shop-Scheduling mit Fälligkeitsterminen und Flow-Shop-Scheduling mit begrenzten Zwischenlägern by **Iria Lechleiter**
- [ ] Computational Intelligence in Flow Shop and Job Shop Scheduling by **Uday K. Chakraborty**
- [ ] Genetic and Hybrid Algorithm Approaches to Flow Shop Scheduling by **Jose Rodrigues**
- [ ] Job Shop Scheduling with Consideration of Due Dates: Potentials of Local Search Based Solution Techniques by **Jens Kuhpfahl**

## Youtube

- [x] [The scheduling problem playlist](https://www.youtube.com/playlist?list=PLN4kTzLXGGgU2-WLwxfuRwfnENwSusLCb) by **Luis R. Izquierdo**
	- [x] The scheduling problem (1/7). Introduction
	- [x] The scheduling problem (2/7). Types of scheduling problems
	- [x] The scheduling problem (3/7). Assumptions and notation
	- [x] The scheduling problem (4/7). Performance measures and objectives
	- [x] The scheduling problem (5/7). Different approaches to deal with scheduling problems
	- [x] The scheduling problem (6/7). Different priority rules applied to a job shop problem
	- [x] The scheduling problem (7/7). Computation of makespan in a permutation flow shop

**Types of scheduling problems**

* **Permutation Flow Shop**: In the permutation flow shop, (i) all jobs have the same processing order through the machines, and (ii) each machine processes the jobs in the same order. E.g., a Conveyor. n! possible solutions.
* **Flow shop**: In a flow shop problem, there are m machines that should process n jobs. All jobs have the same processing order through the machines. The order of the jobs in each machine can be different. There is not common transport nor any type of hard link. (n1)^m possible solutions.
* **Job Shop**: Each job has its own routing. (n!)^m possible solutions.
* **Open shop**: Unlike the job-shop problem, the order in which the processing steps happen can vary freely.
* **Dynamic**: Jobs arriving dynamically.

**Solution strategies**

* **Exact methods**
	* Optimal solution, but only for simple cases (Johnson's rule, Hodgon's Algorithm)
* **Heuristic methods and priority rules**
	* Easy to apply but often not very good solutions
* **Metaheuristic methods (stochastic optimization)**
	* Iterative local search
	* Simulated annealing
	* Genetic algorithms
	* Tabu Search
	* ...

**Performance measures and objective**

* **C_max** = makespan
* **F_max** = minimizing the maximum flow time of jobs
* **F_med** = minimizing the average flow time of jobs

Due date related objectives:

* **T_max** = minimizing the maximum tardiness
* **E_max** = minimizing the maximum earliness
* **L_max** = minimizing the maximum absolute lateness
* **T_med** = minimizing the average tardiness
* **E_med** = minimizing the mean earliness
* **L_med** = minimizing the mean absolute lateness
* **number of tardy jobs**

Performance measures with priority:

* **F_{wt}** = minimizing the weighted sum of flow times of the jobs. The larger the weight of the job, the more important it is.
* **T_{wt}** = minimizing the weighted sum of the tardiness
* **L_{wt}** = minimizing the weighted sum of the absolute lateness
* **E_{wt}** = minimizing the weighted sum of the earliness
* **ET_{wt}** = minimizing the weighted sum of the tardiness and earliness times

**Priority rules**	

* **Total Slack**
	* Slack = due date - actual date - processing time of remaining operations
* **Critical Ratio**
	* Critical ratio = (due date - actual date)/(processing time of remaining op.)
* **Shortest Processing Time (SPT)**
* **Longest Processing Time (LPT)**
* **FIFO (First In First Out)**
* **LIFO (Last In First Out)**
* **Earliest Due Date (EDD)**
* **Jobs with longer remaining process time**
* **Higher value**
* **Work In Queue (WINQ)**
* **Random**


- [x] [Introduction to Metaheuristics](https://www.youtube.com/playlist?list=PLN4kTzLXGGgWNf4CDyoZZOsjOCftW5ej6) by **Luis R. Izquierdo**
	- [x] Introduction to Metaheuristics (1/9)
	- [x] Introduction to Metaheuristics (2/9). Combinatorial Optimization problems
	- [x] Introduction to Metaheuristics (3/9). Exact methods, approximate methods and metaheuristics
	- [x] Introduction to Metaheuristics (4/9). Classification criteria for metaheuristics
	- [x] Introduction to Metaheuristics (5/9). Exploration and Exploitation. When to use metaheuristics
	- [x] Introduction to Metaheuristics (6/9). Random search
	- [x] Introduction to Metaheuristics (7/9). Local search
	- [x] Introduction to Metaheuristics (8/9). Local search applied to the Travelling Salesman Problem
	- [x] Introduction to Metaheuristics (9/9). Summary of Introduction to Metaheuristics


* **Relaxation** = Solve a simpler/easier problem than the original problem in hope that you get some insights on the original problem and to solve it at the end
* **Metaheuristic** = General purpose heuristic or a high-level problem-independent algorithmic framework , Meta-(beyond, at a higher level), -heuristic(to find, to search, to discover)

**Taxonomies**

Many classification criteria may be used for metaheuristics. The most common are:

* Nature inspired vs non-nature inspired
* Memory usage vs memoryless methods
* Deterministic vs stochastic
* Iterative vs greedy
* Population-based vs single-solution based search


## Websites

- [ ] CPU scheduling: https://www.geeksforgeeks.org/preemptive-and-non-preemptive-scheduling/
	* Algorithms based on preemptive scheduling are: Round Robin (RR),Shortest Remaining Time First (SRTF), Priority (preemptive version), etc.
	* Algorithms based on non-preemptive scheduling are: Shortest Job First (SJF basically non preemptive) and Priority (non preemptive version), etc.

## Papers

- [x] Waqas, U., Geilen, M., Kandelaars, J., Somers, L., Basten, T., Stuijk, S., ... & Corporaal, H. (2015, March). A re-entrant flowshop heuristic for online scheduling of the paper path in a large scale printer. In 2015 Design, Automation & Test in Europe Conference & Exhibition (DATE) (pp. 573-578). IEEE.
- [x] Pinxten, J. V., Waqas, U., Geilen, M., Basten, T., & Somers, L. (2017). Online scheduling of 2-re-entrant flexible manufacturing systems. ACM Transactions on Embedded Computing Systems (TECS), 16(5s), 1-20.	