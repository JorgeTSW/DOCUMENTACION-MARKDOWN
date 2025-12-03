# Tecnológico de Software  
## Materia: Fundamentos de Álgebra  
## Profesor: Jorge Javier Pedroza Romero
## Alumno: *Cristopher M. Euan Pool*
## Actividad #20
---

## Índice
1. Objetivo general  
2. Matrices originales (36×36)  
3. Matrices traspuestas  
4. Suma de matrices  
5. Resta de matrices  
6. Multiplicación escalar  
7. Composición de matrices  
8. Conclusiones generales

## Objetivo general 

El objetivo de esta actividad fue reforzar las operaciones matriciales fundamentales mediante su aplicación en Excel, representando imágenes como matrices y realizando con ellas transposición, suma, resta, multiplicación escalar y composición. Además, se busca practicar el uso de fórmulas, formato condicional y funciones matriciales en Excel, junto con la correcta documentación del proceso en Markdown dentro de un branch en GitHub, aplicando buenas prácticas de control de versiones y redacción técnica.

---
## Documentación de Matrices Originales (Imágenes 36×36) 

En esta sección documento como hice la construcción de cinco imágenes representadas como matrices de 36×36 en Excel. Cada imagen se creo en excel de manera manual y luego se le dio un formato de colores en este de la primera fue a color y en las siguientes fueron en una escales de balancos y negro 

### 1. Matriz de Imagen Original 1 (36×36) 

#### Captura de la Hoja en Excel

<img width="504" height="467" alt="image" src="https://github.com/user-attachments/assets/b804135c-6a64-4515-80e1-f37be3959846" />


#### Método Utilizado 

Se creó una matriz de 36 filas × 36 columnas, asignando un valor numérico para cada pixel de 1 para negros y 0 para blancos, el rango pasa por todos los decimales hasta llegar a 1.

Para “colorear” la imagen se aplicaron reglas de formato condicional: 

> Excel → Formato condicional → Nueva regla → “Usar una fórmula que determine las celdas para aplicar formato”

Para cada color se definió una fórmula del tipo:

```excel
=A1=1   → aplica color 1 → Negro
=A1=2   → aplica color .5 → gris 
=A1=3   → aplica color 0 → blanco
```
Cada regla incluía un relleno de color distinto.
```excel
$A$1:$AJ$36
```

### 2. Matriz de 2 imagen 2(36×36)

#### Captura de la Hoja en Excel

<img width="609" height="580" alt="image" src="https://github.com/user-attachments/assets/27450e22-0583-4965-85cd-fbc7d7aca97f" />


#### Descripción del proceso

El procedimiento fue el mismo que en Imagen 1:

- matriz de 36×36

- valores numéricos para representar colores

- reglas de formato condicional basadas en fórmulas como:

```excel
=A1=1   → aplica color 1 → Negro
=A1=7   → aplica color .5 → girs  
=A1=8   → aplica color 0 → blanco
```


### 3. Matriz de Imagen 3 (36×36)

#### Captura de la Hoja en Excel

<img width="502" height="500" alt="image" src="https://github.com/user-attachments/assets/21e51e6e-4281-419d-9f9f-fc7aafc7aeb2" />


#### Descripción del proceso

El procedimiento fue el mismo que en Imagen  y 0 utilizando de igual manera los decimales entre esos valores.

### 4. Matriz de 4 (36×36)

#### Captura de la Hoja en Excel

<img width="559" height="337" alt="image" src="https://github.com/user-attachments/assets/a012952f-a794-4588-9a7e-a84f0294b54d" />


#### Descripción del proceso

El procedimiento fue el mismo que en Imagen 2 se utilizo un rando entre blaco y negro 1 siendo negro y 0 blanco


### 5. Matriz de Imagen Original 5 (36×36)

#### Captura de la Hoja en Excel

<img width="379" height="662" alt="image" src="https://github.com/user-attachments/assets/de341184-4906-4580-81d4-54072a9b00b8" />


#### Descripción del proceso

El procedimiento fue el mismo que en Imagen 1 en este se utilizo una de escala del 0 al 2 en rango de 0 para blanco,1 para negro y 2 para rojo


## Documentación de Matrices Traspuestas (Imágenes 65×33)

Tras construir las cinco matrices originales (65×33), se generó para cada una su matriz traspuesta.
La traspuesta de una matriz A consiste en intercambiar filas por columnas, es decir:

> El elemento en fila i, columna j pasa a la posición fila j, columna i.

Esto permite aplicar operaciones matriciales correctamente y visualizar cómo cambia la distribución del pixel art al reorganizar la matriz.

---

### 1. Traspuesta de la Imagen 5

Captura de la Hoja en Excel:

<img width="590" height="298" alt="image" src="https://github.com/user-attachments/assets/a1d6b331-40db-453b-a5a0-0dc8af9ac245" />


#### Método Utilizado:

En Excel, se utilizó la función:

```excel
=TRANSPONER(imagen7!A1:AK36)
```
### Importante:

Antes de escribir la fórmula, es necesario seleccionar un rango del mismo tamaño que la matriz original.
Como la matriz original es de 36 filas × 36 columnas, su traspuesta también será de 65×33.
En Excel moderno no necesitas presionar CTRL + SHIFT + ENTER, la fórmula matricial se confirma automáticamente.

--- 

### 2. Traspuesta de la multiplicacion matricial 2

Captura de la Hoja en Excel:


<img width="628" height="419" alt="image" src="https://github.com/user-attachments/assets/6985e106-1262-4bf4-978a-aa35fa2887e6" />


#### Método Utilizado:

Se aplicó la misma fórmula adaptada al rango de la imagen 2:

```excel
(+= 1*a1:ad30)
```

---

### 3. Suma de dos matrices

Captura de la Hoja en Excel:


<img width="732" height="343" alt="image" src="https://github.com/user-attachments/assets/e9f004b8-29e0-41c4-ab62-6c04502b3e66" />


#### Método Utilizado:

Fórmula usada:


```excel
=a1:ad30+(imagen5)
```

---

### 4. resta de matrices

Captura de la Hoja en Excel:


<img width="740" height="515" alt="image" src="https://github.com/user-attachments/assets/bc765384-55d2-4146-85a6-0e1b6b72bd85" />


#### Método Utilizado:

Fórmula usada:


```excel
=RESTAa1:ad30(imagen3)
```

---

### 5. Resta de matrices

Captura de la Hoja en Excel:


<img width="794" height="549" alt="image" src="https://github.com/user-attachments/assets/0a46e2eb-7380-4ca7-a72c-6915d4b1bbfa" />


#### Método Utilizado:

Fórmula usada:


```excel
=RESTAa1:ad30(imagen2)
```
---


Ambas matrices deben tener exactamente 36×36 valores.
La suma se hace celda por celda, por lo que no es una suma matricial compleja sino aritmética.
El resultado mantiene la estructura del pixel art, pero con colores “mezclados” al aumentar los valores.

### Interpretación del resultado

El resultado de la suma de matrices refleja una combinación directa de los valores numéricos que codifican los colores de ambas imágenes. Cuando un píxel presenta valores altos en las dos matrices, la suma genera un valor mayor, produciendo un color más “intenso” dentro del esquema numérico definido. En los casos en que las figuras no coinciden en posición o forma, la operación crea nuevos patrones y tonalidades, ya que los valores de cada píxel se combinan de manera independiente respecto a la imagen original. De esta forma, es posible observar cómo dos representaciones pixeladas se mezclan matemáticamente para generar una tercera imagen.

--- 

## Operación 2: Resta de Matrices (Imagen A − Imagen B)
La resta de matrices consiste en sustraer los valores de cada elemento de una matriz con los correspondientes elementos de otra matriz del mismo tamaño. Dado que nuestras imágenes están representadas como matrices de 36×36, la operación se realiza celda por celda, comparando cada posición equivalente en ambas matrices.

```excel
(A − B)ᵢⱼ = Aᵢⱼ − Bᵢⱼ
```

En Excel, cada celda del resultado muestra la diferencia numérica entre los valores de color correspondientes en las matrices A y B.

#### En esta ocasión se utilizan las mismas imagenes que en la operación de suma para poder hacer mas practico el ejercicio.


#### Notas importantes

- Ambas matrices deben tener el mismo tamaño (36×36).
- Si el valor de B es mayor que A en alguna celda, el resultado será un número negativo.
- Los valores negativos representan diferencias inversas de intensidad. 
- Esta operación no mezcla colores, sino que marca diferencias punto por punto.

#### Interpretación del resultado

El resultado de la resta matricial permite identificar de forma precisa las diferencias entre las dos imágenes pixeladas. Un valor de 0 indica que ambos pixeles eran idénticos; un valor positivo significa que la Imagen A tenía una mayor intensidad en esa posición; mientras que un valor negativo refleja que la Imagen B poseía un valor superior. Cuando las imágenes difieren en forma o distribución, la operación genera patrones que resaltan contrastes y variaciones visuales. Esta técnica es particularmente útil para detectar cambios estructurales entre matrices y analizar cómo se comportan dos representaciones pixeladas al compararse punto por punto.

--- 


# Conclusiones Generales

La actividad permitió comprender y aplicar de manera integral las operaciones matriciales fundamentales utilizando Excel como herramienta de análisis y visualización. Representar imágenes pixeladas como matrices numéricas facilitó observar de forma clara cómo cada operación transforma la estructura y los valores de una imagen digital. La transposición evidenció el efecto de intercambiar filas por columnas sobre la orientación de las figuras; las operaciones de suma y resta permitieron analizar la interacción entre dos matrices, ya sea combinando sus valores o resaltando diferencias puntuales; la multiplicación escalar mostró cómo un cambio numérico uniforme puede alterar la intensidad de toda la matriz sin modificar su forma; y la composición condicional demostró cómo superponer imágenes mediante reglas lógicas simula efectos de capas y transparencia.

En conjunto, la práctica fortaleció no solo la comprensión de las operaciones matriciales en el contexto del álgebra, sino también el manejo de funciones, referencias y formato condicional en Excel, integrando conceptos matemáticos con herramientas digitales aplicables a situaciones reales.
