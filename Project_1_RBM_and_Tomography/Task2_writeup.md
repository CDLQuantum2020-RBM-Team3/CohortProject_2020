# Task 2 writeup

## 1. Minimum number of hidden units required

In the first part of Task 2, we work to evaluate the difficulty of the learning problem with the very large dataset `Rydberg_data.txt`

In order to do so, we train an RBM using the entire dataset (20,000 data points), and test to see if the RBM's predicted energy is very close to the exact energy of the molecule, over a range of steps (epochs).

We define "very close to the exact energy" with the following energy difference threshold formula:

    C = |E_{RBM} - E_{exact}| <= 0.0001


???? `n` times in a row upon evaluation, where we make evaluations every `I_{eval}` epochs. ?????

In order to minimise statistical variation in `C` and, therefore, minimize the chance of triggering the stopping criterion too early, we find it's important to use a large number of testing samples. In our test, we use 10,000 testing samples.

To solve for the minimum number of hidden units `N_h` required, we run experiments with max epochs `E` set to 1000 while ramping `N_h` up between experiments. Starting with 1 hidden unit, we test whether `C`, the energy difference threshold, is met.

The following figure shows the minimum value of `C` over a 1000 epoch training run for values of `N_h`: 

[insert plot]

We find that we reach the energy difference threshold with only one hidden unit, `N_h = 1`.

The following figure shows `C` vs number of epochs during a sample training run. 

[insert plot]



## 2. Minimum number of data samples required

In the final part of Task 2, we are interested in reducing the amount of data we need for testing to achieve the desired `C` energy difference threshold. In this case, we solve with double the minimum hidden units found in Part 1 (2*(1 hidden unit) = 2 hidden units).

 

