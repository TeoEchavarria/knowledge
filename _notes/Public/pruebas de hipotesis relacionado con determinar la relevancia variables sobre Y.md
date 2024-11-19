- Planteamos una [[pruebas de hipotesis]] $H_0 : beta_1=0$ y $H_1 : beta_1 != 0$ 

>[!warning] Idea
>Al convertir a $beta_1$ en cero estamos suponiendo que la v.a. que esta acompañando no tiene relevancia sobre $Y$ de esta forma se testea el impacto que tiene la v.a.

>[!note] Herramientas
>Para saber esto podemos usar tanto la prueba $t$ como la del [[anova]], [[sumary]] del modelo ver $P r (>|t|)$ , donde si es menor a $0.05$ el modelo es significativo
>![[sumary.png|350]]

Donde $beta_1$ lo podemos ver como:
$$beta_1 = (sum y_i [x_i - hat(X))/ (sum x_i^2 - hat(X) sum x_i) $$
$$= sum y_i dot m_i$$
- Comprobamos que $beta_1$ sea una combinacion lineal de [[variable aleatoria|v.a.]] [[distribucion normal|normales]], en el caso de que asi sea eso nos dice que se distribuye normal de la forma $$beta_1 tilde N (mu_beta_1, sigma_beta_1^2)$$
Donde : $$mu_beta_1 = E[beta_1] = E[sum y_i dot m_i]$$
Llegando a algo como que $sum m_i = 0$ y $sum m_i x_i = 1$ lo que reemplazando en la [[esperanza]] a calcular nos da que es un estimador insesgado, por lo que $$E[beta_1]=beta_1$$
y $$V a r[beta_1] = sigma^2 sum m_i^
2$$
> Como podemos relacionar la distibucion $N tilde (beta_1,  sigma^2 sum m_i^2)$ con la hipotesis?

Como no conocemos $beta_1$ ni tampoco $sigma^2$ lo que tenemos es que estandarizar, mas con $overline(sigma^2)$ que es una $t_(n-2)$ y como $beta_1 = 0$ 

- Planteamos un [[estadistico de prueba]] bajo $H_0$ : 
- $$overline(beta)/sqrt(overline(sigma)^2 sum m_i^2)$$
- 