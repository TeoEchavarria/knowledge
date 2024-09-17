> [!PDF|red] [[Clase 20.pdf#page=10&selection=5,0,123,1&color=red|Clase 20, p.1]]
> > Suponga que se tiene un experimento multinomial, es decir una serie de ensayos ($n$ ensayos) identicos e independientes y $k$ posibles categorias o clases. Sea $p_i$ la probabilidad de clasificar un sujeto u objeto en la categoria $i$ y sea $N_i$ el numero de sujetos u objetos que caen en la categoria $i$ de los n ensayos. Se tiene que $N_1 + · · · + N_k = n$. Cada $N_i$ sera una v.a. binomial con parametros $n$ y $p_i$ con $i = 1, 2 · · · , k$. El numero esperado de ensayos en la categoria $i$ sera $$E [N_i] = n \cdot p_i ; i = 1, 2, · · · , k$$ 
> 

![[Clase 20.pdf#page=10&rect=7,63,355,123&color=red|Clase 20, p.1]]

### Para variables discretas

![[Clase 20.pdf#page=16&rect=7,15,355,220&color=red|Clase 20, p.2]]

> Para todos los $p_i$ 

# Ejemplo 

![[Clase 20.pdf#page=33&rect=10,144,355,224|Clase 20, p.4]]

> [!PDF|red] [[Clase 20.pdf#page=33&selection=79,11,130,1&color=red|Clase 20, p.4]]
> > Asi las cosas, las hipotesis a plantear son: $$H_0 : p_i = 1/6 , i = 1, 2, · · · , 6 text("vs") H_a : exist j text("tal que") p j 6 = 1/6 $$

![[Clase 20.pdf#page=44&rect=6,167,355,231&color=red|Clase 20, p.5]]
Por lo que nuestra [[region de rechazo]] seria:
$$R.C. = {X_c | X_c > chiq_(0.05)(5)}$$
Como $X_c=4.82$ y $chiq_(0.05)(5)=11.07$ entonces $X_c$ no pertenece a la region de rechazo por lo que no se rechaza $H_0$

![[Clase 20.pdf#page=44&rect=54,40,267,76&color=red|Clase 20, p.5|400]]

### Pruebas para variables continuas
> [!PDF|note] [[Clase 20.pdf#page=96&selection=61,3,64,16&color=note|Clase 20, p.12]]
> > [[prueba de hipotesis Kolmogorov-Smirnov]], [[prueba de hipotesis  Shapiro-Wilks]], [[prueba de hipotesis Cramer Von Misses]], [[prueba de hipotesis Jarque Bera]],[[prueba de hipotesis de Asimetria y Kurtosis de Mardia]]

