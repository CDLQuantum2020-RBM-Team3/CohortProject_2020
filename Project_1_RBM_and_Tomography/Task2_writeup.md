# Task 2 writeup

## 1. Minimum number of hidden units required

In the first part of Task 2, we work to evaluate the difficulty of the learning problem with the very large dataset `Rydberg_data.txt`

In order to do so, we train an RBM using the entire dataset (20,000 data points), and test to see if the RBM's predicted energy is very close to the exact energy of the molecule, over a range of steps (epochs).

We define "very close to the exact energy" with the following energy difference threshold formula:

    C = |E_{RBM} - E_{exact}| <= 0.0001


???? `n` times in a row upon evaluation, where we make evaluations every `I_{eval}` epochs. ?????

In order to minimise statistical variation in `C` and, therefore, minimize the chance of triggering the stopping criterion too early, we find it's important to use a large number of testing samples. In our test, we use 10,000 testing samples.

To solve for the minimum number of hidden units `n_hin` required, we run experiments with max epochs `E` set to 1000 while ramping `N_h` up between experiments. Starting with 1 hidden unit, we test whether `C`, the energy difference threshold, is met.

The following figure shows the minimum value of `C` over a 1000 epoch training run for values of `n_hin`: 

[insert plot, C vs # hidden units]

![C vs Hidden Units](/Task2_writeup_plots/"Sweep_over_hidden_units.png") ???save the plots and add???

We find that we reach the least energy difference with only one hidden unit, `n_hin = 1`. In fact, as shown in the plot below with ??*averaged*?? min energy differences as a function of the number of hidden units, we find that the energy differences increase as we increase hidden units. 

Note: Since we intentionally used a large number of testing samples and introduced patience functions to minimize statistical variation in our energy difference calculations, we never actually hit the energy difference threshold, though we approach it with the lower hidden units.


Below is an example of a statistically optimized plot given `n_hin = 1` and `stopping_patience = 2`, displayed with `C` as a function of the  number of epochs during a sample training run. 

[insert plot, C vs # epochs]


We can solve for the "size" of the entity the RBM spits out is the equivalent storage of `100 + n_hin + n_hin*100 = 100 + 1 + 1*100  = 201` numbers. In comparison to `2^100 = 1.27*10^30`, it's clear that the RBM's output is much smaller in size and, thus, extremely useful for computation. 



## 2. Minimum number of data samples required

In the final part of Task 2, we are interested in reducing the amount of data we need for testing to achieve the desired `C` energy difference threshold. In this case, we solve with double the minimum `n_hin` hidden units found in Part 1 (double min N_h = 2 hidden units).

We start with 500 testing data points, `n_testing_samples`, and move up in increments of 100 to solve for the minimum testing samples necessary to reach `C`, the energy difference threshold.
 
 [insert plot]
 
We find that the minimum `n_testing_samples` necessary to reach `C` is 500 testing samples, a significant reduction in data from the original 20,000 data points. 


