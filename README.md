# The scheduling problem

## Books

- [ ] Scheduling: Theory, Algorithms, and Systems (2016) by **Michael L. Pinedo**
- [ ] Flow Shop Scheduling: Theoretical Results, Algorithms, and Applications by **Hamilton Emmons and George Vairaktarakis**
- [ ] Maschinenbelegungsplanung in der Variantenfertigung: Job-Shop-Scheduling mit Fälligkeitsterminen und Flow-Shop-Scheduling mit begrenzten Zwischenlägern by **Iria Lechleiter**
- [ ] Computational Intelligence in Flow Shop and Job Shop Scheduling by **Uday K. Chakraborty**
- [ ] Genetic and Hybrid Algorithm Approaches to Flow Shop Scheduling by **Jose Rodrigues**
- [ ] Job Shop Scheduling with Consideration of Due Dates: Potentials of Local Search Based Solution Techniques by **Jens Kuhpfahl**

## Youtube

- [ ] [The scheduling problem playlist](https://www.youtube.com/playlist?list=PLN4kTzLXGGgU2-WLwxfuRwfnENwSusLCb) by **Luis R. Izquierdo**
	- [x] The scheduling problem (1/7). Introduction
	- [x] The scheduling problem (2/7). Types of scheduling problems
	- [ ] The scheduling problem (3/7). Assumptions and notation
	- [ ] The scheduling problem (4/7). Performance measures and objectives
	- [ ] The scheduling problem (5/7). Different approaches to deal with scheduling problems
	- [ ] The scheduling problem (6/7). Different priority rules applied to a job shop problem
	- [ ] The scheduling problem (7/7). Computation of makespan in a permutation flow shop

**Types of scheduling problems**

* **Permutation Flow Shop**: In the permutation flow shop, (i) all jobs have the same processing order through the machines, and (ii) each machine processes the jobs in the same order. E.g., a Conveyor. n! possible solutions.
* **Flow shop**: In a flow shop problem, there are m machines that should process n jobs. All jobs have the same processing order through the machines. The order of the jobs in each machine can be different. There is not common transport nor any type of hard link. (n1)^m possible solutions.
* **Job Shop**: Each job has its own routing. (n!)^m possible solutions.
* **Open shop**: Unlike the job-shop problem, the order in which the processing steps happen can vary freely.
* **Dynamic**: Jobs arriving dynamically.

## Websites

- [ ] CPU scheduling: https://www.geeksforgeeks.org/preemptive-and-non-preemptive-scheduling/
	* Algorithms based on preemptive scheduling are: Round Robin (RR),Shortest Remaining Time First (SRTF), Priority (preemptive version), etc.
	* Algorithms based on non-preemptive scheduling are: Shortest Job First (SJF basically non preemptive) and Priority (non preemptive version), etc.

## Papers

- [x] Waqas, U., Geilen, M., Kandelaars, J., Somers, L., Basten, T., Stuijk, S., ... & Corporaal, H. (2015, March). A re-entrant flowshop heuristic for online scheduling of the paper path in a large scale printer. In 2015 Design, Automation & Test in Europe Conference & Exhibition (DATE) (pp. 573-578). IEEE.
- [ ] Pinxten, J. V., Waqas, U., Geilen, M., Basten, T., & Somers, L. (2017). Online scheduling of 2-re-entrant flexible manufacturing systems. ACM Transactions on Embedded Computing Systems (TECS), 16(5s), 1-20.	