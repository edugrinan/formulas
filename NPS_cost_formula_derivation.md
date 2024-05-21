## NPS Cost Formula Derivation

Let $P_t$, $N_t$, and $D_t$ be the fractions of promoters, neutrals, and detractors at time $t$ for a population $n_t$. If $G_P$, $G_N$, and $G_D$ are the average expenditures of a member of each group, the total expenditure of the population will be:

$$
G_t = n_t \left( P_t G_p + N_t G_N + D_t G_d \right)
$$

We can define $X_P, X_N$, such that $G_P = X_P + G_D$ and $G_N = X_N + G_D$. Substituting these, we get:

$$
G_t = n_t \left( P_t X_P + N_t X_N + G_D \right)
$$

So the difference in the population total expenditure between $t$ and $t+1$ will be:

$$
\Delta G_{t+1,t} = n_{t+1} \left( P_{t+1} X_{P,t+1} + N_{t+1} X_{N,t+1} + G_{D,t+1} \right) - n_t \left( P_t X_{P,t} + N_t X_{N,t} + G_{D,t} \right)
$$

Now, as long as $n_t$ is different from $n_{t+1}$, it is impossible to isolate a $\Delta G$ that depends solely on $\Delta NPS$, i.e., the variation of $P_t$, $N_t$, and $D_t$.

* Assumption 1: $n_t \approx n_{t+1} \equiv n$.

* Assumption 2: $X_P, X_N, G_D$ do not depend (or depend very weakly) on $t$.

$$
\Delta G_{t+1,t} = n \left( X_P \left( P_{t+1} - P_t \right) + X_N \left( N_{t+1} - N_t \right) \right)
$$

* Assumption 3: If the behavior of neutrals is similar to that of promoters, $X_P \approx X_N \equiv X$.

$$
\Delta G_{t+1,t} = n X \left( P_{t+1} - P_t  + N_{t+1} - N_t \right) = n X \left( D_t - D_{t+1} \right) 
$$
