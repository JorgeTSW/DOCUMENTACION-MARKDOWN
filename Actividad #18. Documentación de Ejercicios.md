# Tecnológico de Software
  ## Materia: Fundamentos de álgebra
  ## Alumno: Jesus Fernando Castro Hernandez
  ## Actividad \#18 - Documentación de Ejercicios con Git Branches
  
  ---
  # Ejercicio 1: Determinantes 2x2
  ## Calcula los determinantes

  $$ A =
  \begin{pmatrix}
  4 & 5 \\
  -3 & 2 \\
  \end{pmatrix}
$$

### Determinante de la Matriz A
$$
\begin{aligned}
\det(A) &= (4)(2) - (5)(-3) \\
        &= 8 - (-15) \\
        &= 8 + 15 \\
        &= 23
\end{aligned}
$$



$$ B =
  \begin{pmatrix}
  3 & 5 & 7 \\
  0 & -3 & 1 \\
  0 & 0 & 9 \\
  \end{pmatrix}
$$
### Determinante de la Matriz B
$$
\begin{aligned}
\det(B) &= (3)(-3)(9) \\
        &= -9(9) \\
        &= -81
\end{aligned}
$$


$$ C =
  \begin{pmatrix}
  8 & 7 & 6 \\
  15 & 2 & 3 \\
  2 & 4 & 10 \\
  \end{pmatrix}
$$

### Determinante de la Matriz C
$$
\begin{aligned}
\det(C) &= [(8)(2)(10) + (7)(3)(2) + (6)(15)(4)] - [(2)(2)(6) + (4)(3)(8) + (10)(15)(7)] \\
        &= [160 + 42 + 360] - [24 + 96 + 1050] \\
        &= 562 - 1170 \\
        &= -608
\end{aligned}
$$

### Determinantes de BC
Primero resolvemos la matriz BC

$$
BC =
\begin{pmatrix}
3 & 5 & 7 \\
0 & -3 & 1 \\
0 & 0 & 9
\end{pmatrix}
\begin{pmatrix}
8 & 7 & 6 \\
15 & 2 & 3 \\
2 & 4 & 10
\end{pmatrix}=
\begin{pmatrix}
24+75+14 & 21+10+28 & 18+15+70 \\
0-45+2 & 0-6+4 & 0-9+10 \\
0+0+18 & 0+0+36 & 0+0+90
\end{pmatrix}=
\begin{pmatrix}
113 & 59 & 103 \\
-43 & -2 & 1 \\
18 & 36 & 90
\end{pmatrix}
$$

Ahora ya calculamos los determinantes

$$
\begin{aligned}
\det(BC) &= [(113)(-2)(90) + (59)(1)(18) + (103)(-43)(36)] \\
         &\quad - [(18)(-2)(103) + (36)(1)(113) + (90)(-43)(59)] \\
         &= [-20,340 + 1,062 - 159,444] - [-3,708 + 4,068 - 228,330] \\
         &= [-178,722] - [-227,970] \\
         &= -178,722 + 227,970 \\
         &= 49,248
\end{aligned}
$$














