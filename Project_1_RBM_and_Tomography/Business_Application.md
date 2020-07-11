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



## Step 2: Explain or provide examples of the types of real-world problems this solution can solve

Applications of optimizing molecular data simulation:
- **Pharma and Materials Science applications**: drug and molecule discovery 
    - Molecular structure analysis by combinatorial optimization
    - Protein design using unconstrained discrete optimization [[1]](https://www.zapatacomputing.com/solutions/)
    - QM/MM method for molecular binding affinity prediction in drug discovery [[1]](https://www.zapatacomputing.com/solutions/)
    - Ab initio transition state analysis for catalytic reaction simulation [[1]](https://www.zapatacomputing.com/solutions/)
    - Ab initio determination of the crystalline structure of organic molecules [[1]](https://www.zapatacomputing.com/solutions/)
    - Molecular screening in drug discovery using continuous latent space [[1]](https://www.zapatacomputing.com/solutions/)
    - ground state simulations, why can't they do it easily and what would it change?
    - Additionally, with more advanced quantum computing hardware, drug development times could be sped up by **20%** using similar molecular simulation optimizations [[Boston Consulting Group]](https://www.bcg.com/en-us/publications/2018/coming-quantum-leap-computing.aspx)
        - We will have a stake in this by expanding research to be compatible with quantum resources, like our D-Wave optimization work


- Other industries (financial, telecom, etc.) have the potential to benefit from the optimization with further work to effectively map their complex data sets into a Hamiltonian. 



## Step 3: Identify at least one potential customer for this solution - ie: a business who has this problem and would consider paying to have this problem solved

- Big Pharma --- what are their R&D costs per drug?
    - Pfizer
    - Roche
    - Merck
    - Where does this fall into the research pipeline??
    

## Step 4: Prepare a 90 second video explaining the value proposition of your innovation to this potential customer in non-technical language

**Script (main points-- drafting)**

- "The development of these new Ising machines and the possibility of mapping the electronic structure problem into
an Ising-type Hamiltonian may grant efficient ways to obtain exact solutions to the Schrödinger equation;
this being one of the most daunting computational problem present in both chemistry and physics."


- COVID comparison!

- exponential reduction in storage, ex) 201 numbers vs 10^30 data points
    - on top of that, we're quadratically decreasing the testing data necessary, to improve computational speeds