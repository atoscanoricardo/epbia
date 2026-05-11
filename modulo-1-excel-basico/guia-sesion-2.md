# Guía de Sesión 2: El Cerebro de Excel (Funciones Avanzadas)

En esta sesión pasaremos de "escribir datos" a "hacer que los datos hablen". Aprenderemos a manipular texto, gestionar fechas con precisión y usar lógica condicional para la toma de decisiones.

---

## 1. Manipulación de Texto (Data Cleaning)
A menudo los datos vienen "sucios" de otros sistemas. Estas funciones son tu kit de limpieza:
*   **`IZQUIERDA / DERECHA / EXTRAE`**: Extraen partes específicas de un código (ej. los primeros 3 dígitos de un ID).
*   **`UNIRCADENAS`**: La evolución del viejo `CONCATENAR`. Permite unir textos con un separador (ej. una coma) e ignorar celdas vacías.
*   **`HALLAR`**: Encuentra la posición de un carácter (como un espacio o un @) para saber dónde cortar un texto.

## 2. El Tiempo es Oro (Funciones de Fecha)
Excel cuenta los días desde el 1 de enero de 1900. Entender esto es clave para cálculos financieros.
*   **`SIFECHA(inicio, fin, "Y")`**: La función "oculta" de Excel para calcular años cumplidos (edad o antigüedad).
*   **`DIA.LAB`**: Calcula una fecha futura saltándose fines de semana y festivos (ideal para gestión de proyectos).

## 3. Lógica y Estadística Condicional
Aquí es donde Excel empieza a "pensar" por ti:
*   **`SUMAR.SI.CONJUNTO`**: Suma valores solo si cumplen varias condiciones (ej. "Ventas de Café" + "En Bogotá" + "Mes de Mayo").
*   **`CONTAR.SI.CONJUNTO`**: Cuenta cuántas veces ocurre algo bajo múltiples criterios.
*   **`PROMEDIO.SI.CONJUNTO`**: Obtiene el promedio bajo criterios específicos.

---

## ⚡ El Concepto: "Anidación"
La verdadera potencia aparece cuando pones una función dentro de otra. 
*   *Ejemplo:* `=IZQUIERDA(A1, HALLAR(" ", A1)-1)` -> Esta fórmula extrae automáticamente el primer nombre de una celda, sin importar qué tan largo sea, buscando el primer espacio.

---
> **Próximo Paso:** Ve al ejercicio `dashboard-rrhh.md` para aplicar estas funciones en un caso real de gestión de talento humano.
