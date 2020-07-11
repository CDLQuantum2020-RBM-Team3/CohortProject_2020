# Task 2 writeup

## Finding minimum number of hidden units required

Our stopping criterion is that the following needs to be satisfied

$$
C = |E_{RBM} - E_{exact}| \leq 0.0001
$$

$n$ times in a row upon evaluation, where we make evaluations every $I_{eval}$ epochs.

We find that it is important to use a large number of testing samples in order to minimise statistical variation in $C$, and therefore minimise the chance of triggering the stopping criterion too early.

In order to find the minimum number of hidden units $N_h$ required, we run experiments with max epochs $E$ set to 1000 while ramping $N_h$ up between experiments.

The following figure shows the minimum value of $C$ over a 1000 epoch training run for values of $N_h$

We settle on an approximate value $N_h = 10$.

The following figure shows $C$ vs number of epochs during a training run. The stopping criterion is reach at xx epochs.

