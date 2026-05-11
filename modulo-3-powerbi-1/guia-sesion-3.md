# Guía de Sesión 3: Fundamentos de DAX (El Lenguaje del Análisis)

¡Bienvenido al motor de inteligencia de Power BI! **DAX (Data Analysis Expressions)** es el lenguaje de fórmulas que te permitirá crear indicadores potentes. Aunque se parece a las fórmulas de Excel, DAX es mucho más eficiente y flexible una vez que entiendes cómo funciona.

---

## 1. ¿Columna Calculada o Medida?
Esta es la pregunta más importante en Power BI. La respuesta depende de *cuándo* quieres que ocurra el cálculo:

*   **Columna Calculada**: Se calcula fila por fila y se guarda en la memoria. Úsala solo si necesitas usar ese dato como un filtro o categoría (ej. Categorizar un producto como "Caro" o "Barato").
*   **Medida (¡Nuestra favorita!)**: Se calcula "al vuelo" cuando la arrastras a un gráfico. No ocupa espacio extra y es increíblemente rápida. Úsala para casi todo: sumas, promedios, porcentajes, etc.

## 2. La Regla de Oro del Contexto
DAX no piensa en celdas individuales como Excel (A1, B2). DAX piensa en **Contextos de Filtro**. 
*   Si pones una medida de `Total Ventas` en una tabla por "Ciudad", la medida se filtrará automáticamente para cada ciudad. ¡Tú solo escribes la fórmula una vez y ella se adapta a todo!

## 3. Funciones Esenciales para Empezar
Aquí tienes tu primer kit de herramientas DAX:
*   **`SUM`**: Suma todos los valores de una columna. 
    *   `Ventas Totales = SUM(Ventas[Monto])`
*   **`COUNTROWS`**: Cuenta cuántas filas tiene una tabla (ideal para contar pedidos o facturas).
    *   `Total Pedidos = COUNTROWS(Ventas)`
*   **`DISTINCTCOUNT`**: Cuenta cuántos valores únicos hay (ej. cuántos clientes diferentes compraron).
*   **`DIVIDE`**: La forma más segura de dividir. Si el denominador es cero, te devuelve un blanco en lugar de un error.
    *   `Margen % = DIVIDE([Utilidad], [Ventas])`

---

## 💡 Un Consejo para tu Aprendizaje
DAX puede parecer intimidante al principio, pero recuerda: **Empieza simple**. No necesitas fórmulas de 10 líneas para obtener grandes resultados. Con las funciones básicas y un buen modelo de datos, ya eres capaz de responder el 80% de las preguntas de cualquier negocio. ¡Vamos a practicar!

---
> **Próximo Paso:** Crea tus propios indicadores de éxito en el ejercicio `mis-primeras-medidas-dax.md`.
