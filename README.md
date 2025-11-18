# Tecnológico de Software
## Materia: Fundamentos de álgebra
## Alumno: Humberto Ramirez Gruintal
## Actividad \#18 - Determinantes

---

# Cálculo de determinantes

# EJERCICIO 1  
## Determinante de una matriz 2×2

Para una matriz:

$$
A =
\begin{pmatrix}
4 & 5 \\
-3 & 2 \\
\end{pmatrix}
$$

Usamos la fórmula:

$$
\det(A) = ad - bc
$$

Sustituyendo:

$$
\det(A) = (4)(2) - (5)(-3)
$$

$$
= 8 + 15 = 23
$$

$$
\boxed{23}
$$

---

# EJERCICIO 2  
## Determinante de la matriz B

Dada la matriz:

$$
B =
\begin{pmatrix}
3 & 5 & 7 \\
0 & -3 & 1 \\
0 & 0 & -9 \\
\end{pmatrix}
$$

Como es una **matriz triangular**, su determinante es el producto de sus elementos diagonales:

$$
\det(B) = (3)(-3)(-9)
$$

$$
= -9 \cdot (-9) = 81
$$

$$
\boxed{81}
$$

---

# EJERCICIO 3  
## Determinante de la matriz C

La matriz es:

$$
C =
\begin{pmatrix}
8 & 7 & 6 \\
15 & 2 & 3 \\
2 & 4 & 10 \\
\end{pmatrix}
$$

Usamos la **regla de Sarrus**.

### Diagonales positivas

$$
(8)(2)(10) + (7)(3)(2) + (6)(15)(4)
$$

$$
= 160 + 42 + 360 = 562
$$

### Diagonales negativas

$$
(6)(2)(2) + (8)(3)(4) + (7)(15)(10)
$$

$$
= 24 + 96 + 1050 = 1170
$$

### Determinante

$$
\det(C) = 562 - 1170 = -608
$$

$$
\boxed{-608}
$$

---

# EJERCICIO 4  
## Determinante del producto BC

Usamos la propiedad:

$$
\det(BC) = \det(B)\cdot\det(C)
$$

Con los valores:

$$
\det(B) = 81, \qquad \det(C) = -608
$$

Entonces:

$$
\det(BC) = (81)(-608)
$$

$$
= -49248
$$

$$
\boxed{-49248}
$$






