Permite establecer asociaciones, en este caso lineales, entre las variables de interes.

## Enfoque probabililistico - [[metodo de maxima verosimilitud]]
![[regresion_lineal.pdf#page=4&rect=46,7,438,193|regresion_lineal, p.4]]

$$E(Y|X) = mu_x = beta_0+beta_1 X$$
> Todas las distribuciones tiene la misma forma, comparten la varianza, lo unico que se transporta es la media (que a su vez es la moda y la mediana).

## Enfoque no probabilistico - [[metodo de minimos cuadrados]]

![[regresion_lineal.pdf#page=5&rect=46,8,431,239|regresion_lineal, p.5]]

$$Y_i = beta_0+beta_i X + Epsilon_i$$
Donde $Epsilon_i$ es una variable de error iid con distribucion $N tilde (0,sigma^2)$ 

>[!warning] 
>Como $Y_i$ es una funcion de [[variable aleatoria]] [[distribucion normal|normal]], entonces $Y_i$ tambien es normal

$$Y_i tilde N(E[Y_I], V a r[Y_i])$$
Donde :
$$E[Y_i]= E(beta_0+beta_i X + Epsilon_i)$$
$$= beta_0 + beta_i X$$
$$V a r (Y_i)= V a r(beta_0+beta_i X + Epsilon_i) = sigma^2$$

Para hacer la prediccion de un $Y_(n+1)$ a partir de un $X_(n+1)$ conocido, lo que tenemos que hacer, es estimar $beta_0, beta_1$ y $sigma^2$ 

Via [[metodo de maxima verosimilitud|maxima verosimilitud]]: $$L(beta_0, beta_1, sigma^2 | y_1, ..., y_n, x_1, ..., x_n)$$
$$=f(y_1, ..., y_n|beta_0, beta_1, sigma^2, x_1, ..., x_n)$$

Y recordemos que si ![[independencia entre variables aleatorias]]

Por lo que:

$$=product_(i=1)^n f(y_i|beta_0, beta_1, sigma^2, x_1, ..., x_n)$$
$$Y_i tilde N(beta_0, beta_1 X_i, sigma^2)$$

Llegando a que: $$f(y_i) = 1/(sqrt(2 pi sigma^2)) exp(-1/(2 sigma^2) (y_i-beta_0-beta_1 X_i)^2)$$

Posterior a esto lo que toca es sacar las derivadas parciales para $beta_0, beta_1$ y $sigma^2$ llegando a algo como:
$$$$