# Tecnológico de Software
## Materia: Fundamentos de Álgebra
## Alumno: David Morales Guerrero
## Actividad #20 – Operaciones Matriciales con Excel y GitHub

---

## 🎯 Objetivo
Aplicar operaciones matriciales básicas utilizando hojas de Excel programadas para realizar:

- Matriz numérica derivada de una imagen (pixel-art)
- Suma de matrices
- Resta de matrices
- Multiplicación escalar
- Transposición

Además, integrar el trabajo a un repositorio de GitHub utilizando formato Markdown.

---

## 📂 Archivos incluidos en el proyecto

### ✔ `Punisher`
Imagen en pixel-art reconstruida con colores reales (negro, blanco y rojo).

### ✔ `Punisher_matrix`
Conversión de la imagen a matriz numérica:
- Negro = 1  
- Blanco = 0  
- Rojo = 2  

### ✔ `Punisher_sum`
Suma total de los elementos de la matriz.

### ✔ `Punisher_resta`
Matriz A multiplicada por -1.

### ✔ `Punisher_scalar2`
Matriz A multiplicada por el escalar **2**.

### ✔ `transponer`
Versión transpuesta del pixel-art original.

---

## 🧮 Programación de la hoja de Excel

### **1. Conversión de colores a números**

```excel
=SI(Punisher!A1="#000000",1, SI(Punisher!A1="#FF0000",2,0))
