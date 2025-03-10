#Econ/Macro 

Recall some model setting:

- [[Government Spending]]: $G = \gamma Y$
- Tax Revenue: 
	- Lump-sum tax $T$ (We usually ignore it)
	- Labour-income tax $\tau_{w}$
	- **Capital-income tax** $\tau_{r}$ (What we are interested in this chapter)

## Government Side

$$
G = T + \tau_{r} rK + \tau_{w} wl
$$

We are going to change $\tau_{r}$(holding $\gamma$ constant) to see how $\tau_{r}$ affects the macroeconomy.

## Household Side

Recall, for household, we want to maximize their utility:

$$
u = \ln C + \beta \ln(L-l) +v (G)
$$
the maximization problem is:

$$
max_{C,l} U = \sum_{t=0} \frac{\ln C_{t}+ \beta \ln (L-l_{t}) +v(G_{t})}{(1-\rho)^t}
$$
s.t.

$$
\dot{K} = I = wl + rK -\tau_{r}rK - T - C
$$
It is intuitive to use the [[Hamiltonian]] to calculate the best answer, lets do this again:

$$
\begin{align}
\frac{\delta H}{\delta C} & = \frac{1}{C} - \lambda = 0 \implies \lambda = \frac{1}{C} \\
\frac{\delta H}{\delta l} & = -\frac{\beta}{L-l} + \lambda w = 0 \implies \lambda w = \frac{\beta}{L-l}\\
\frac{\delta H}{\delta K} & = \lambda\underbrace{  (1-\tau_{r}r) }_{ \text{after-tax capital rental price} } = \rho\lambda - \dot{\lambda}  \\
\implies - & \frac{\dot{\lambda}}{\lambda} = (1-\tau_{r})r- \rho
\end{align}
$$

