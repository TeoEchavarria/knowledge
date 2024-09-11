
#geometry
# Matriz Cuadrada

Sea $A$ una matriz cuadrada.

- Diremos que un número $\lambda \in \mathbb{C}$ es un valor propio (o autovalor) de $A$ si existe un [[vector]] no nulo, $v \neq 0$, tal que $Av = \lambda v$. Al vector $v$ se le llama vector propio (o autovector) asociado al valor propio $\lambda$.
- $\lambda$ es un valor propio de $A$ si y sólo si $\lambda$ es un cero del [[polinomio]] característico $p(A) = \det(A - \lambda I)$, esto es, $\lambda$ es raíz de la [[ecuación]] característica $p(A) = 0$.

- El espectro de $A$ es el [[conjunto]] de todos sus valores propios:

  $$
  \sigma(A) := \{ \lambda \in \mathbb{C} : \lambda \text{ es un valor propio de } A \}.
  $$

- El radio espectral de $A$ es el máximo módulo de sus valores propios:

  $$
  \rho(A) := \max_{\lambda \in \sigma(A)} |\lambda|.
  $$
