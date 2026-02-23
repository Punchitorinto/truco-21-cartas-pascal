# truco-21-cartas-pascal
# 🃏 Magic 21 Card Trick - Pascal Implementation

Este repositorio contiene una implementación robusta del clásico truco de magia de las 21 cartas, desarrollado en **Pascal** utilizando el entorno **Lazarus**.

## 🚀 Descripción del Proyecto
El programa simula el proceso donde un usuario elige una carta mentalmente y, mediante tres rondas de preguntas sobre la ubicación de la misma, el software logra identificarla con precisión absoluta.

## 🧠 Lógica y Algoritmo
El núcleo del proyecto se basa en un **Algoritmo de Convergencia Matemática**:
- **Estructura:** Se utiliza un arreglo unidimensional de 21 elementos para representar el mazo.
- **Transposición:** En cada ronda, el mazo se reparte en una matriz de 7x3 (3 columnas).
- **Convergencia:** Al colocar sistemáticamente la columna elegida por el usuario entre las otras dos (técnica de "sándwich"), la carta objetivo se desplaza hacia el centro del arreglo.
- **Resultado:** Tras exactamente 3 iteraciones válidas, la carta elegida colapsa invariablemente en la **posición 11**.

## 🛠️ Características Técnicas (Code Highlights)
- **Validación de Entradas (Sanitización):** El programa maneja entradas vacías, caracteres no deseados y números fuera del rango [1..3] sin romper la lógica del mazo.
- **Gestión de Estados:** El contador de rondas solo progresa ante ingresos de datos válidos.
- **Manipulación de Arreglos:** Implementación de un sistema de reparto "tipo póker" (distribución round-robin) para sincronizar lo que el usuario ve visualmente con la estructura de datos interna.
- **Arquitectura Lineal (Sin Procedimientos/Funciones):** El diseño se mantuvo deliberadamente en un bloque principal para demostrar el dominio absoluto sobre el flujo de control, la anidación de ciclos y la gestión de variables globales sin abstracciones externas.
  
## 💻 Cómo ejecutarlo
1. Descarga el archivo `.pas`.
2. Ábrelo con **Lazarus IDE** o cualquier compilador de Pascal (como Free Pascal).
3. Compila y ejecuta (`F9`).

---
Desarrollado con fines educativos para demostrar lógica algorítmica y control de flujo. 😎

