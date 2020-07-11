![CDL 2020 Cohort Project](../figures/CDL_logo.jpg)
# Quantum Cohort Project Business Application

For each weekly project, your team is asked to complete the below business application exercise.
To complement the technical tasks, please consider the four questions below.
You are free to format your response to these four questions as you wish (with the final question done as a short recorded video), and to include
the content (or links to the content) on your forked repository.

A brief example for each question is included for the 
[Traveling Salesman Problem.](https://en.wikipedia.org/wiki/Travelling_salesman_problem)

## Step 1: Explain the technical problem you solved in this exercise

*early brainstorming bullets-- feel free to delete/change/simplify and expand on*

Overall: Optimization, in application of studying energy of molecules.

- **Task 2**: Optimization problem with exponential speedup: minimized the hidden units and training samples necessary for training the RBM (201 data points vs 10^30 data points)
- **D-Wave**: Solving the optimization problem on D-Wave resources. Expanding our RBM optimization work to new efficient simulation platforms and building relationships and channels for collaboration with a big quantum hardware company (D-Wave). This work allows us a starting point for further exploration with D-Wave resources for further computationally complex chemistry problems we want to solve where D-Wave resources may provide an advantage (ex. larger molecules).  

Example: Finding a global minimum in settings where a classical approach may not be able to find a global minimum.

## Step 2: Explain or provide examples of the types of real-world problems this solution can solve

Optimizing data
- Pharma applications -- searching for ideal molecules 
    - ground state simulations, why cant' they do it easily and what would it change?
---Where does this fall into the research pipeline??
- financial applications -- map financial data to a Hamiltonian 

- ...

Example: A courier has to deliver parcels to several locations and is looking to minimize its travel time. (e.g., “the travelling salesman problem”).

## Step 3: Identify at least one potential customer for this solution - ie: a business who has this problem and would consider paying to have this problem solved

- Big Pharma --- what are their R&D costs per drug?
    - Pfizer
    - Roche
    - Merck
- Big Banks -- what is portfolio optimization R&D? Pitch the speedup of finding optimal portfolios
    - JPM 
    - Goldman Sachs
    - Bank of America
- ...

## Step 4: Prepare a 90 second video explaining the value proposition of your innovation to this potential customer in non-technical language

**Script (main points-- drafting)**

- The development of these new Ising machines and the possibility of mapping the electronic structure problem into
an Ising-type Hamiltonian may grant efficient ways to obtain exact solutions to the Schrödinger equation;
this being one of the most daunting computational problem present in both chemistry and physics.


- COVID comparison!

- exponential reduction in storage, ex) 201 numbers vs 10^30 data points
    - on top of that, we're quadratically decreasing the testing data necessary, to improve computational speeds