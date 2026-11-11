# Matematica discreta

## Amigo invisible

Es bien conocido este problema. Empecemos por recordar que basicamente el amigo
invisible es hacer una permutacion sin puntos fijos.

Al cardinal de todas las permutaciones se le denota: $n!$
Mintras que al cardinal de todas las permutaciones validas para el amigo
invisible, se le denota: $!n$

---

### Fórmulas

1. Fórmula general:

$$
!n = n! \sum_{k=0}^n \frac{(-1)^k}{k!}
$$

2. Aproximación (con redondeo al entero más cercano):

$$
!n \approx \frac{n!}{e}
$$

3. Definición recursiva

$$
!n = (n-1)(!(n-1) + !(n-2))
$$

con condiciones iniciales:

$$
!0 = 1, \quad !1 = 0
$$

### Primeros valores

* $!0 = 1$
* $!1 = 0$
* $!2 = 1$
* $!3 = 2$
* $!4 = 9$
* $!5 = 44$
* $!6 = 265$

### Algoritmo para la obtencion de un permutacion de este tipo

Existen cuatro tipos:

- Equiprobables (suponiendo tener algoritmo de reordenacion)
- No equiprobables pero completos
- No completos equiprobables
- Nada bueno

Evidentemente nos interesan los tres primeros:


