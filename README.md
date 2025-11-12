# Tecnológico de Software
## Materia: Fundamentos de álgebra
## Profesor: Jorge Javier Pedrozo Romero
## Alumno: Giovana Ruby Díaz Anduze
## Actividad \#16 - Matrices doc
## Fecha: 11 de noviembre de 2025

---
### EJEMPLO DE LA ACTIVIDAD: Identificación de matrices

Matriz identidad, porque la diagonal está compuestos por solo unos y los elementos fuera de la diagonal son ceros.

$$ A =
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
$$

MUESTRA

Calcula la suma de A y B

$$ A =
\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
\end{pmatrix}
$$

$$ B =
\begin{pmatrix}
9 & 10 & 11 \\
12 & 13 & 14 \\
\end{pmatrix}
$$

$$ A + B =
\begin{pmatrix}
1 + 9 & 2 + 10 & 3 + 11 \\
4 + 12 & 5 + 13 & 6 + 14 \\
\end{pmatrix}
$$

$$ A + B =
\begin{pmatrix}
10 & 12 & 14 \\
16 & 18 & 20 \\
\end{pmatrix}
$$

---
# TÍTULO: MATRICES
---

---
# OBJETIVO DE LA DOCUMENTACIÓN:
El objetivo principal de esta actividad es que como alumnos implementemos los conocimientos de los temas vistos, matrices, de la asisgnatura en la plataforma Github.
---

---
Ejercicio 1: Clasificar matrices
---
El objetivo de este ejercicio es con base en las matrices que nos proporcionan identificar qué clase de matriz es.
---
$$ A =
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
$$

Tipo de matriz:
- Identidad porque todos los elementos de la diagonal son 1.

$$ B =
\begin{pmatrix}
3 & 0 & 0 \\
0 & -2 & 0 \\
0 & 0 & 5 \\
\end{pmatrix}
$$

Tipo de matriz:
- Diagonal porque todos los elementos fuera de la diagonal son ceros.

$$ C =
\begin{pmatrix}
2 & 1 & 4 \\
1 & 3 & 5 \\
4 & 5 & 6 \\
\end{pmatrix}
$$

Tipo de matriz:
- Simétrica porque los elementos tanto arriba como abajo de la diagonal son iguales.

$$ D =
\begin{pmatrix}
1 & 2 & 3 \\
0 & 4 & 5 \\
0 & 0 & 6 \\
\end{pmatrix}
$$

Tipo de matriz:
- Triángulas superior porque todos los elementos debajo de la diagonal son cero.

---
Ejercicio 2: operaciones básicas
---
El objetivo de este ejercicio es realizar operaciones básicas de matrices.
---

$$ A =
\begin{pmatrix}
2 & -1 \\
3 & 4 \\
\end{pmatrix}
$$

$$ B =
\begin{pmatrix}
5 & 2 \\
-1 & 3 \\
\end{pmatrix}
$$

- Calcula:

A) A + B 

$$ A + B =
\begin{pmatrix}
2+5 & -1+2 \\
3-1 & 4+3 \\
\end{pmatrix}
$$

$$ A + B =
\begin{pmatrix}
7 & 1 \\
2 & 7 \\
\end{pmatrix}
$$

B) 2A - B

$$ 2A =
\begin{pmatrix}
4 & -2 \\
6 & 8 \\
\end{pmatrix}
$$

$$ 2A - B =
\begin{pmatrix}
4-5 & -2-2 \\
6-(-1) & 8-3 \\
\end{pmatrix}
$$

$$ 2A - B =
\begin{pmatrix}
-1 & -4 \\
7 & 5 \\
\end{pmatrix}
$$

C) AB

$$ AB =
\begin{pmatrix}
((2x5) + (-1x-1)) & ((2x2) + (-1x3)) \\
((3x5) + (4x-1)) & ((3x2) + (4x3)) \\
\end{pmatrix}
$$

$$ AB =
\begin{pmatrix}
11 & 1 \\
11 & 18 \\
\end{pmatrix}
$$

D) BA

$$ AB =
\begin{pmatrix}
((5x2) + (2x3)) & ((5x-1) + (2x4)) \\
((-1x2) + (3x3)) & ((-1x-1) + (3x4)) \\
\end{pmatrix}
$$


$$ BA =
\begin{pmatrix}
16 & 3 \\
7 & 13 \\
\end{pmatrix}
$$

E) A^T

$$ A =
\begin{pmatrix}
2 & -1 \\
3 & 4 \\
\end{pmatrix}
$$

$$ A^T =
\begin{pmatrix}
2 & 3 \\
-1 & 4 \\
\end{pmatrix}
$$

---
Ejercicio 3: Multiplicación de cadena
---
El objetivo de este ejercicio es demostrar que ambas operaciones que nos proporcionan son iguales.
---

$$ A =
\begin{pmatrix}
1 & 2 \\
3 & 4 \\
\end{pmatrix}
$$

$$ B =
\begin{pmatrix}
2 & 0 \\
1 & 3 \\
\end{pmatrix}
$$

$$ C =
\begin{pmatrix}
1 & 1 \\
0 & 2 \\
\end{pmatrix}
$$

- Demuestra que: (AB)C = A(BC)
---
# (AB)C
- AB:

$$ AB =
\begin{pmatrix}
((1x2) + (2x1)) & ((1x0) + (2x3)) \\
((3x2) + (4x1)) & ((3x0) + (4x3)) \\
\end{pmatrix}
$$

$$ AB =
\begin{pmatrix}
4 & 6 \\
10 & 12 \\
\end{pmatrix}
$$

- (AB)C:

$$ (AB)C =
\begin{pmatrix}
((4x1) + (6x0)) & ((4x1) + (6x2)) \\
((10x1) + (12x0)) & ((10x1) + (12x2)) \\
\end{pmatrix}
$$

$$ (AB)C =
\begin{pmatrix}
4 & 16 \\
10 & 34 \\
\end{pmatrix}
$$

# A(BC)
- BC:

$$ BC =
\begin{pmatrix}
((2x1) + (0x0)) & ((2x1) + (0x2)) \\
((1x1) + (3x0)) & ((1x1) + (3x2)) \\
\end{pmatrix}
$$

$$ (BC) =
\begin{pmatrix}
2 & 2 \\
1 & 7 \\
\end{pmatrix}
$$

- A(BC):

$$ A(BC) =
\begin{pmatrix}
((1x2) + (2x1)) & ((1x2) + (2x7)) \\
((3x2) + (4x1)) & ((3x2) + (4x7)) \\
\end{pmatrix}
$$

$$ A(BC) =
\begin{pmatrix}
4 & 16 \\
10 & 34 \\
\end{pmatrix}
$$

RESPUESTA: SÍ DAN LO MISMO
