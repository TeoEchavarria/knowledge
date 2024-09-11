#metodosNumericos
# Metodo : Gauss-Seidel

Parecido al [[metodo Jacobi]] mas al momento de reemplazar en las funciones lo que hacemos es utilizar los anteriores que reemplazamos

Como ejemplo sea $$
\begin{align*}
x_1^{(k+1)} &= 3 + 2x_2^{(k)} + x_3^{(k)} \\
x_2^{(k+1)} &= \frac{9}{2} + x_2^{(k)} + \frac{3}{2} x_3^{(k)} \\
x_3^{(k+1)} &= -\frac{41}{7} + \frac{4}{7} x_2^{(k)} - \frac{8}{7} x_3^{(k)}
\end{align*}
$$
Tomando $x^{(0)} = [1, 1, -1]^T$

$$
x_1^{(k+1)} = 3 + 2x_2^{(k)} + x_3^{(k)}
$$

$$
x_2^{(k+1)} = 3 + \frac{1}{2}\textcolor{red}{(3+2x_2^{(k)} + x_3^{(k)})} + x_3^{(k)}= \frac{9}{2} + x_2^{(k)} + \frac{3}{2} x_3^{(k)}
$$

$$
x_3^{(k+1)} = \frac{17}{7} + \frac{1}{7} \textcolor{red}{(3 + 2x_2^{(k)} + x_3^{(k)})} - \frac{6}{7}  \textcolor{red}{(\frac{9}{2} + x_2^{(k)} + \frac{3}{2} x_3^{(k)})} = -\frac{41}{7} + \frac{4}{7} x_2^{(k)} - \frac{8}{7} x_3^{(k)}
$$

$$
\Rightarrow T_{GS} = \begin{bmatrix}
0 & 2 & 1 \\
0 & 1 & \frac{3}{2} \\
0 & -\frac{4}{7} & -\frac{8}{7}
\end{bmatrix}

y \quad c_{GS} = \begin{bmatrix}
3 \\
\frac{9}{2} \\
-\frac{41}{7}
\end{bmatrix}
$$
