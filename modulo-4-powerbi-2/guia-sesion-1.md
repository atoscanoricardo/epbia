# Guía de Sesión 1: DAX Avanzado - El Poder de CALCULATE

¡Bienvenido al nivel experto! En esta sesión conocerás la función más importante de Power BI: **CALCULATE**. Si DAX fuera un equipo de superhéroes, CALCULATE sería el líder.

---

## 1. La Función CALCULATE
CALCULATE permite modificar el contexto de filtro de un cálculo. Es decir, puedes pedirle a Power BI que sume las ventas, pero ignorando ciertos filtros o forzando otros.
*   **Sintaxis**: `CALCULATE([Medida], Filtro1, Filtro2...)`
*   **Ejemplo**: `Ventas Norte = CALCULATE([Ventas Totales], Geografía[Sede] = "Norte")`

## 2. Las Funciones ALL y FILTER
Para que CALCULATE sea aún más potente, solemos acompañarla de estas dos:
*   **ALL**: "Limpia" o ignora los filtros. Es vital para calcular porcentajes de participación (ej. "Mis ventas" dividido "Ventas de todos").
*   **FILTER**: Permite aplicar filtros más complejos, como "Ventas donde el precio sea mayor al promedio".

## 3. Iteradores (SUMX, AVERAGEX)
A diferencia de `SUM`, que suma toda una columna, `SUMX` recorre una tabla fila por fila, hace un cálculo (ej. Precio * Cantidad) y luego suma los resultados. Esto te da una precisión total en modelos complejos.

---

## 💡 Un Salto Mental
CALCULATE no es solo una fórmula, es una forma de pensar. Te permite responder preguntas como: "¿Cuánto vendí de este producto comparado con el total de su categoría?". ¡Estás desbloqueando el verdadero potencial analítico!
