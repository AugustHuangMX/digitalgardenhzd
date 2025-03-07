
[[Government Spending]]

[[Labor Income Tax]]

# Fiscal Policy in the Neoclassical growth model 

> Chapter 7 in the book.

- Government expenditure: $G = \gamma Y$.
- Tax revenue: 
	- lump-sum tax $T$. (Which is rare in reality)
	- Labor-income tax $\tau_{w}$
	- Capital-income tax $\tau_{r}$

## Government

$$
G=T + \tau_{r}rK + \underbrace{ \tau_{w} WL }_{ \text{we set} \ \tau_{r} = 0 \ \text{here} }
$$
We are going to change $\tau_{r}$ (holding $\gamma$ constant) to see how $\tau_{r}$ affects the macroeconomy.

## Household

$$
U = \ln C +\beta \ln(L-l) +v(G)
$$

$$
max_{C,l} U = \sum_{t=0}\frac{\ln C+ \beta \ln(L-l_{t})+v(G_{t})}{(1+\rho^t)}
$$

s.t. $\dot{K} = I = wl+rK - \tau_{r} rK - T-C$ 

Do the [[Hamiltonian]] function: 

$$
H = \ln C +\beta \ln(L-l) +v(G) + \lambda [wl + r(1-\tau_{r})K - T -C]
$$

$$
\begin{align}
\frac{\delta H}{\delta C} = \frac{1}{C} - \lambda = 0  \\
\frac{\delta H}{\delta l} = - \frac{\beta}{L - l} + \lambda w=0 \\
\frac{\delta H}{\delta K }  = r(1-\tau_{r})\lambda = \rho \lambda -\dot{\lambda}
\end{align}
$$

Only $\frac{\delta H}{\delta K}$ changes compared with the previous [[Hamiltonian]] function. 

$$
-\frac{\dot{\lambda}}{\lambda} = \underbrace{ (1-\tau_{r})R }_{ \text{after-tax capital } }- \rho
$$

$$
\begin{align}
\frac{\dot{C}}{C} = (1-\tau_{r})r-\rho \\
\end{align}
$$

[[Steady State]]: $\dot{C} = 0 \implies K^s_{LR}: R = \frac{\rho}{1-\tau_{r}}$

When $\tau_{r}$ increases, the long-run capital supply curve shifts upward (i.e., reduction in supply)

When the government taxes capital income move heavily, the household accumulates less capital.

> Then, we look at the firm side.

$$
l^s: w= \frac{\beta C}{L-l}
$$
Nothing new here.

Long-run effects of capital income tax *(Short-run is left as an exercise)*

> 两张图

Comparative Static: $\tau_{r} \uparrow$

- $\tau_{r} \uparrow \implies K_{LR}^s$ shifts upward $\implies K \downarrow, r\uparrow$
- K

We want to show that $l^*$ is independent of $\tau_{r}$

This is a special result due to the assumption of $\delta= 0$

Deriving the steady-state level of labor $l^*$:

$$
\begin{align}
l^d: w= MPL = (1-\alpha)A\left( \frac{K}{l} \right)^\alpha = \frac{(1-\alpha)Y}{l} \\
l^s: w=\frac{\beta C}{L-l} \implies l^s = L -\frac{\beta C}{L-l} \\
l^s = l^d \implies l = L - \frac{\beta C}{(1-\alpha)Y}l  \\
\end{align}
$$

Given $\delta = 0, \frac{C}{Y} = 1-\gamma$

thus,

$$
l^* = \frac{L}{1+ \frac{\beta}{1-\alpha}(1-\gamma)} 
$$

is independent of $\tau_{w}$ due to $\delta = 0$

> Question: How things change when $\delta \neq 0$

So it is independent of $\tau_{R}$

Output market:

$$
Y = A K^\alpha l^{1-\alpha}
$$

shows that $Y$ will decrease 

> Trick: In the short run, it will affect the labor market first, in which the labor market shifts to the left, because the $C$ rises initially due to the lower  (after tax rental price)$(1-\tau_{r})r$, which reduces capital accumulation.

