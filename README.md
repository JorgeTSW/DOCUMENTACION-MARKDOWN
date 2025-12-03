  # Tecnológico de Software
  ## Materia: Fundamentos de álgebra
  ## Alumno: Jesus Fernando Castro Hernandez
  ## Actividad \#22 - Matrices doc
  

# Solución de Sistemas de Ecuaciones Lineales

Este documento detalla la resolución paso a paso de los ejercicios.

---

Entendido. Aquí tienes la documentación completa formateada *exclusivamente con texto simple y Markdown*, sin usar códigos matemáticos complejos ni LaTeX, para que no tengas problemas al copiar y pegar.

-----

# 🧮 Fundamentos de Álgebra - Solución de Ejercicios

## Ejercicio 1: Resolver con todos los métodos

**Sistema de Ecuaciones:**

$$
\begin{cases}
x + y + z = 6 \\
2x - y + z = 3 \\
x + 2y - z = 2
\end{cases}
$$

### a) Método de Gauss (Eliminación Gaussiana)

**Objetivo:** Llegar a una matriz escalonada (triangular).

**Paso 1: Matriz Inicial**

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 6 \\
2 & -1 & 1 & 3 \\
1 & 2 & -1 & 2
\end{array}
\right]
$$

**Paso 2: Hacer ceros debajo del primer 1**

Operaciones:
* $F_2 \rightarrow F_2 - 2(F_1)$
* $F_3 \rightarrow F_3 - F_1$

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 6 \\
0 & -3 & -1 & -9 \\
0 & 1 & -2 & -4
\end{array}
\right]
$$

**Paso 3: Acomodar filas**
Intercambiamos $F_2$ con $F_3$ para tener el "1" en la diagonal principal y facilitar el cálculo:

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 6 \\
0 & 1 & -2 & -4 \\
0 & -3 & -1 & -9
\end{array}
\right]
$$

**Paso 4: Eliminar el -3 de abajo**

Operación:
* $F_3 \rightarrow F_3 + 3(F_2)$

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 6 \\
0 & 1 & -2 & -4 \\
0 & 0 & -7 & -21
\end{array}
\right]
$$

**Paso 5: Sustitución hacia atrás**

1.  **Hallar z:**
    $$-7z = -21 \Rightarrow z = \frac{-21}{-7} \Rightarrow \mathbf{z = 3}$$
2.  **Hallar y:**
    $$y - 2(3) = -4 \Rightarrow y - 6 = -4 \Rightarrow \mathbf{y = 2}$$
3.  **Hallar x:**
    $$x + 2 + 3 = 6 \Rightarrow x + 5 = 6 \Rightarrow \mathbf{x = 1}$$

---

### b) Método de Gauss-Jordan

**Objetivo:** Llegar a la matriz identidad (diagonales de 1 y el resto 0).

Continuamos desde donde nos quedamos en Gauss:

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 6 \\
0 & 1 & -2 & -4 \\
0 & 0 & -7 & -21
\end{array}
\right]
$$

**Paso 1: Convertir el -7 en 1**
* Dividir $F_3$ entre -7

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 6 \\
0 & 1 & -2 & -4 \\
0 & 0 & 1 & 3
\end{array}
\right]
$$

**Paso 2: Hacer ceros hacia arriba**
* $F_2 \rightarrow F_2 + 2(F_3)$
* $F_1 \rightarrow F_1 - F_3$

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 0 & 3 \\
0 & 1 & 0 & 2 \\
0 & 0 & 1 & 3
\end{array}
\right]
$$

**Paso 3: Eliminar el último 1 de la Fila 1**
* $F_1 \rightarrow F_1 - F_2$

$$
\left[
\begin{array}{ccc|c}
1 & 0 & 0 & 1 \\
0 & 1 & 0 & 2 \\
0 & 0 & 1 & 3
\end{array}
\right]
$$

**Resultado:** $\mathbf{x = 1, y = 2, z = 3}$

---

### c) Método de Matriz Inversa

**Fórmula:** $X = A^{-1} \cdot B$

**1. Determinante de A:**
Matriz A:
$$
\begin{vmatrix}
1 & 1 & 1 \\
2 & -1 & 1 \\
1 & 2 & -1
\end{vmatrix}
$$

$$Det = 1(1 - 2) - 1(-2 - 1) + 1(4 - (-1))$$
$$Det = 1(-1) - 1(-3) + 1(5)$$
$$Det = -1 + 3 + 5 = \mathbf{7}$$

**2. Matriz Inversa (multiplicada por 1/7):**

$$
A^{-1} = \frac{1}{7}
\begin{bmatrix}
-1 & 3 & 2 \\
3 & -2 & 1 \\
5 & -1 & -3
\end{bmatrix}
$$

**3. Multiplicación (Inversa $\cdot$ Resultados):**

* $x = \frac{1}{7} [(-1)(6) + (3)(3) + (2)(2)] = \frac{1}{7}(-6 + 9 + 4) = \frac{7}{7} = \mathbf{1}$
* $y = \frac{1}{7} [(3)(6) + (-2)(3) + (1)(2)] = \frac{1}{7}(18 - 6 + 2) = \frac{14}{7} = \mathbf{2}$
* $z = \frac{1}{7} [(5)(6) + (-1)(3) + (-3)(2)] = \frac{1}{7}(30 - 3 - 6) = \frac{21}{7} = \mathbf{3}$

---

### d) Regla de Cramer

Se divide el determinante de la variable entre el determinante general (7).

**1. Determinante X** (Cambiar columna X por resultados 6, 3, 2):

$$
\Delta x =
\begin{vmatrix}
6 & 1 & 1 \\
3 & -1 & 1 \\
2 & 2 & -1
\end{vmatrix}
$$

$\Delta x = 6(1 - 2) - 1(-3 - 2) + 1(6 + 2)$
$\Delta x = -6 + 5 + 8 = \mathbf{7}$
$$\mathbf{x = 7 / 7 = 1}$$

**2. Determinante Y** (Cambiar columna Y por resultados 6, 3, 2):

$$
\Delta y =
\begin{vmatrix}
1 & 6 & 1 \\
2 & 3 & 1 \\
1 & 2 & -1
\end{vmatrix}
$$

$\Delta y = 1(-3 - 2) - 6(-2 - 1) + 1(4 - 3)$
$\Delta y = -5 + 18 + 1 = \mathbf{14}$
$$\mathbf{y = 14 / 7 = 2}$$

**3. Determinante Z** (Cambiar columna Z por resultados 6, 3, 2):

$$
\Delta z =
\begin{vmatrix}
1 & 1 & 6 \\
2 & -1 & 3 \\
1 & 2 & 2
\end{vmatrix}
$$

$\Delta z = 1(-2 - 6) - 1(4 - 3) + 6(4 + 1)$
$\Delta z = -8 - 1 + 30 = \mathbf{21}$
$$\mathbf{z = 21 / 7 = 3}$$

---

## Ejercicio 2: Identificar tipo de solución

**a)**
Ecuaciones:
1. $x + y = 3$
2. $2x + 2y = 6$

* **Análisis:** Si divides la segunda ecuación entre 2, te queda exactamente $x + y = 3$. Es la misma línea.
* **Respuesta:** Infinitas soluciones.

**b)**
Ecuaciones:
1. $x + y = 3$
2. $2x + 2y = 7$

* **Análisis:** Si divides la segunda entre 2, queda $x + y = 3.5$. Esto es imposible porque arriba dice que $x + y = 3$. Son líneas paralelas que nunca se tocan.
* **Respuesta:** Ninguna solución.

**c)**
Ecuaciones:
1. $x + y = 3$
2. $x - y = 1$

* **Análisis:** Las pendientes son diferentes. Se cruzan en un punto.
* **Respuesta:** Solución única.

---

## Ejercicio 3: Sistema 4x4

**Sistema:**
1. $x + y + z + w = 10$
2. $2x + y - z + w = 5$
3. $x - y + z - w = 1$
4. $x + y - z + 2w = 8$

**Método rápido (Combinación):**

1.  **Restamos Ec(1) - Ec(4):**
    $$(x+y+z+w) - (x+y-z+2w) = 10 - 8$$
    $$2z - w = 2 \Rightarrow \mathbf{w = 2z - 2}$$

2.  **Restamos Ec(1) - Ec(2):**
    $$(x+y+z+w) - (2x+y-z+w) = 10 - 5$$
    $$-x + 2z = 5 \Rightarrow \mathbf{x = 2z - 5}$$

3.  **Sustituimos x y w en la Ec(3):**
    $$(2z - 5) - y + z - (2z - 2) = 1$$
    $$z - 3 - y = 1 \Rightarrow \mathbf{y = z - 4}$$

4.  **Sustituimos todo en la Ec(1) para hallar z:**
    $$(2z - 5) + (z - 4) + z + (2z - 2) = 10$$
    $$6z - 11 = 10 \Rightarrow 6z = 21 \Rightarrow \mathbf{z = 3.5}$$

5.  **Calculamos los demás:**
    * $w = 2(3.5) - 2 = \mathbf{5}$
    * $x = 2(3.5) - 5 = \mathbf{2}$
    * $y = 3.5 - 4 = \mathbf{-0.5}$

**Resultados:** $x=2, y=-0.5, z=3.5, w=5$

---

## Ejercicio 4: Aplicación práctica (Mix de Productos)

**Datos:**
* P (Premium), S (Standard), U (Utilitario)
* Res: $2P + 1S + 3U = 100$
* Pollo: $3P + 1S + 2U = 120$
* Cerdo: $1P + 2S + 1U = 80$

**Procedimiento:**

1.  **Eliminar S restando (Pollo - Res):**
    $$(3P + S + 2U) - (2P + S + 3U) = 120 - 100$$
    $$P - U = 20 \Rightarrow \mathbf{P = U + 20}$$

2.  **Sustituir P en ecuación de Cerdo:**
    $$(U + 20) + 2S + U = 80$$
    $$2U + 2S = 60 \Rightarrow S + U = 30 \Rightarrow \mathbf{S = 30 - U}$$

3.  **Sustituir P y S en ecuación de Res:**
    $$2(U + 20) + (30 - U) + 3U = 100$$
    $$2U + 40 + 30 - U + 3U = 100$$
    $$4U + 70 = 100 \Rightarrow 4U = 30 \Rightarrow \mathbf{U = 7.5}$$

4.  **Hallar P y S:**
    * $P = 7.5 + 20 = \mathbf{27.5}$
    * $S = 30 - 7.5 = \mathbf{22.5}$

**Respuesta final:**
* Premium: 27.5 unidades
* Standard: 22.5 unidades
* Utilitario: 7.5 unidades
