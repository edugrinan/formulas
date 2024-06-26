## First Neighbors Formula Derivation
### Introduction

Recall that the income variation due to a certain $\Delta \text{NPS}$ in a population $\text{N}$ was:

$$
\frac{\Delta \text{NPS} * \text{N}}{ 2 * 100} * \Delta G_{P-D}
$$

In this expression, the factor

$$
\frac{\Delta \text{NPS} * \text{N}}{ 2 * 100} 
$$

represents the number of detractor-promoter transitions resulting in a $\Delta \text{NPS}$, while $\Delta G_{P-D}$ gives us the income increase associated with one of these transitions. But so far we only considered the **direct effect on the same customer** (hereafter $\Delta G_{0, P-D}$). By including other consequences of a detractor-promoter conversion, we must add to this $\Delta G_{0, P-D}$ other $\Delta G_{i}$. The ones we will present here are caused by the network effect on first, $\Delta G_{FN, P-D}$, and second neighbors, $\Delta G_{SN, P-D}$.

### First Neighbors Contribution

Let $n_P$ be the number of first neighbors (FN) for a **promoter customer**. We will use $X_{P, p}$ , $X_{P, n}$ and $X_{P, d}$ for the fractions of promoters, passives, and detractors among the FN of this very customer. Then the total expenditure by all their FN is:

$$
G_{FN, P} = n_P * (X_{P, p} * G_p + X_{P, n} * G_n + X_{P, d} * G_d)
$$

Where $G_P$, $G_N$, and $G_D$ are the average expenditures of a promoter, passive and detractor. Now we can repeat this expression for the FN of a **detractor customer**:

$$
G_{FN, D} = n_D * (X_{D, p} * G_p + X_{D, n} * G_n + X_{D, d} * G_d)
$$

If we assume that when a customer goes from detractor to promoter, **their entire network instantly shifts from the detractor’s network to the promoter’s network**, then a detractor-promoter transition will result in an income increase of:

$$
\Delta G_{FN, P-D} = G_{FN, P} - G_{FN, D} = n_P * (X_{P, p} * G_p + X_{P, n} * G_n + X_{P, d} * G_d) - n_D * (X_{D, p} * G_p + X_{D, n} * G_n + X_{D, d} * G_d)
$$

This same factor can be defined for the second neighbors (SN), $\Delta G_{SN, P-D}$.

### Complete Formula

Finally, we have the formula:

$$
\frac{\Delta \text{NPS} * \text{N}}{2 * 100} * \left[ \Delta G_{0, P-D} + \Delta G_{FN, P-D} + \Delta G_{SN, P-D} \right]
$$

### Corrections

If we consider that a customer does not have an immediate effect on all their network but only influences a fraction $\alpha$ of it, then the term $\Delta G_{FN, P-D}$ should be multiplied by this factor $\alpha$.
