
The motivation we develop [[Multiple Linear Regression]] is that [[Simple Linear Regression]] only contains one variable that could *explaining* $Y$.

That is, it will face a serious [[Omitted Variable Bias]] (OVB) problem.

## OLS under OVB

The true model:

$$
Y_i = \beta_0 +\beta_1 X_{1i}+\beta_2 X_{2i}+U_I
$$

However, we incorrectly assume:

$$
Y_i = \alpha_0 +\alpha_{1i} X_{1i}+V_i
$$

Where $E[V_i|X_{1i}]=0$



---

From [[Simple Linear Regression in Matrix Notation]], we could also use [[Matrix]] to denote the model.

The initial model is:

$$
y_{i}+ \beta_{1}+\beta_{2}x_{2i}+\beta_{3}x_{3i}+\dots\beta_{k}x_{ki}+\epsilon_{i}
$$

We have $k$ unknowns, and $n$ equations. Only when equations are more than unknowns, we could get the answers.

However, once we change the unknowns to:

$$
\mathbf{X} = \begin{pmatrix}
1 & x_{21} & \dots & x_{k1} \\
\dots  & \dots & \dots & \dots \\
1 & x_{2n} & \dots & x_{kn}
\end{pmatrix}
$$

We could denote the model to a much more simpler form:

$$
\mathbf{y = X \beta + \epsilon}
$$

recall that from [[Simple Linear Regression in Matrix Notation]], the FOC of $S(b))$ is exactly the same, thanks to the matrix:

$$
\mathbf{\frac{\delta S(b)}{\delta b} =} 2\mathbf{X'Xb} - 2\mathbf{X'y = 0}
$$

The difference is that the $\mathbf{X'X}$ is now a $k \times k$ matrix, not $1 \times 1$

We now could derive $e$:

$$
\mathbf{y = Xb +e}
$$
$$
\mathbf{e = y -Xb}
$$
$$
\mathbf{e = y - X (X'X)^{-1}X' y}
$$
$$
\mathbf{e = (I_{k \times k} - X (X'X)^{-1}X' )y}
$$

$$
\mathbf{X'e= X'(I_{n \times n} - X (X'X)^{-1}X' )y}
$$
We called $\mathbf{M = I - X(X'X)^{-1}X'}$ “残差生成矩阵”

$$
\mathbf{X'e= X'I_{k\times k}y-  \underbrace{ X'X (X'X)^{-1} }_{ I_{k} }X'y}  
$$

Thus,

$$
\mathbf{X'e = 0}
$$


Thus we prove that the residual vector $e$ is ==orthogonal== to the matrix of explanatory variables $X$, i.e. $\mathbf{X'e = 0}$.

## OLS part

[[Ordinary Least Squares]]

We could then write $\hat{y}$:

$$
\mathbf{ \hat{y} = Xb = X \underbrace{ (X'X)^{-1} X' y }_{ b }} 
$$
We denote $\mathbf{H}$:
$$
\mathbf{H = X(X'X)^{-1}X'}
$$

$$
\mathbf{y=H y + My = \hat{y}+e}
$$

Try to figure out that $\mathbf{MH = 0}$ ($\mathbf{H}$ and $\mathbf{M}$ are orthogonal).

> Hint: $\mathbf{H = I - M}$

1. identity matrix
2. orthogonal projection matrix

are both [[Idempotency]].


