#metodosNumericos
# Metodo : Jacobi

Tenemos 3 ecuaciones y un vector $x^{(0)}$ 

$$\begin{align*}
-x_1 + 2x_2 + x_3 &= -3 \\
-x_1 + 2x_2 - 2x_3 &= 6 \\
x_1 - 6x_2 - 7x_3 &= 17
\end{align*}$$

1. Despejar la variable $x_i$-esima de cada ecuacion y pasandolo a una matriz de la siguiente forma
$$\begin{align*}
x_1^{(k+1)} &= 3 + 2x_2^{(k)} + x_3^{(k)} \\
x_2^{(k+1)} &= 3 + \frac{1}{2} x_1^{(k)} + \frac{1}{3} x_3^{(k)} \\
x_3^{(k+1)} &= 17 - \frac{1}{7} x_1^{(k)} - \frac{6}{7} x_2^{(k)}
\end{align*}
\Rightarrow
T_J = \begin{bmatrix}
0 & 2 & 1 \\
\frac{1}{2} & 0 & \frac{1}{3} \\
-\frac{1}{7} & -\frac{6}{7} & 0
\end{bmatrix}
, \quad
c_J = \begin{bmatrix}
3 \\
3 \\
-\frac{17}{7}
\end{bmatrix} .
$$



2. Apliquemos el ![[corolario convergencia solucion unica sistema lineal]]
Que particularmete a este problema quedaria algo asi $$\|T_J\|_1 = \max\left\{ \frac{1}{2} + 1, \frac{1}{7} + 2, \frac{6}{7} + 1 \right\} = \frac{20}{7} > 1
$$ $$
\|T_J\|_\infty = \max\left\{ 2 + \frac{1}{2}, 1 + \frac{1}{7}, 1 + \frac{6}{7} \right\} = 3 > 1$$
> Y como ambos son mayor a $1$ entonces no podemos confirmar convergencia

3. Saquemosle el determinante a $T_J$ y cambiamos la diagonal por puros $-\lambda$ $$p_{T_J}(\lambda) = \det(T_J - \lambda I) = \begin{vmatrix}
-\lambda & 2 & 1 \\
\frac{1}{2} & -\lambda & \frac{1}{7} \\
\frac{1}{7} & -\frac{6}{7} & -\lambda
\end{vmatrix} 
$$ $$= -\lambda \left( \begin{vmatrix}
-\lambda & \frac{1}{7} \\
-\frac{6}{7} & -\lambda
\end{vmatrix} - 2 \begin{vmatrix}
\frac{1}{2} & \frac{1}{7} \\
\frac{1}{7} & -\lambda
\end{vmatrix} + \begin{vmatrix}
\frac{1}{2} & -\lambda \\
\frac{1}{7} & -\frac{6}{7}
\end{vmatrix} \right)$$ $$ = -\lambda \left( \lambda^2 + \frac{6}{7} - 2 \left( -\frac{\lambda}{2} + \frac{1}{7} \right) + \left( -\frac{3}{7} + \frac{7}{7} \lambda \right) \right) = -\lambda^3 + \frac{2}{7} \lambda^2 - \frac{1}{7}$$

4. Hacer division sinterica con el polinomio resultante
$$p_{T_J}(\lambda) = (\lambda + 0.6998)(-\lambda^2 + 0.6998\lambda - 0.204118) \Rightarrow \Rightarrow \left\{ 
\begin{array}{l}
\lambda_1 \approx -0.6998 \\
\lambda_{2,3} \approx 0.34994 \pm 0.28576i
\end{array}
\right.
$$$$
\rho(T_J) \approx \max\left\{ | -0.6998|, |0.34994 \pm 0.28576i| \right\} \approx \max\left\{0.6998, \sqrt{0.34994^2 + 0.28576^2} \right\} $$$$\approx \max\{0.6998, 0.451793\}$$
Notemos que $0.6998<1$ por lo que podemos decir que converge $\forall x^(0) \in R^3$ 


