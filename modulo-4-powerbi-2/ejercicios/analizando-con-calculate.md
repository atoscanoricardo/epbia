# Taller Práctico: Análisis Avanzado con CALCULATE 🧠

En este ejercicio final de DAX, resolveremos preguntas de negocio que requieren cambiar el contexto de filtro de forma inteligente.

## 📥 Datos de Contexto
Usaremos tu modelo de ventas ya creado en Power BI Desktop.

---

## 🛠 Tareas de DAX Pro

### 1. Ventas de una Sede Específica
Imagina que la gerencia siempre quiere ver las ventas de "Bogotá" en una tarjeta fija, sin importar qué otros filtros se apliquen en la página.
*   `Ventas Bogota = CALCULATE([Ingresos Totales], Geografía[Ciudad] = "Bogotá")`

### 2. Porcentaje de Participación (ALL)
¿Qué porcentaje del total nacional representa cada ciudad?
1.  Primero, calcula el total de todas las ventas ignorando filtros de ciudad:
    `Total Nacional = CALCULATE([Ingresos Totales], ALL(Geografía[Ciudad]))`
2.  Ahora, calcula el % de participación:
    `Participacion % = DIVIDE([Ingresos Totales], [Total Nacional])`
3.  Formato: Porcentaje (%).

### 3. Filtros Complejos (FILTER)
Crea una medida que sume las ventas, pero solo para aquellos productos que tienen un precio mayor a $500:
*   `Ventas Productos Premium = CALCULATE([Ingresos Totales], FILTER(Productos, Productos[Precio] > 500))`

---

## 🏆 El Dashboard de Análisis Pro
1.  Crea una **Gráfica de Barras** por Ciudad mostrando la `Participacion %`.
2.  Agrega una **Tarjeta** con `Ventas Productos Premium`.
3.  **Verificación**: Si filtras por una ciudad, verás que la medida `Total Nacional` no cambia. ¡Eso significa que ALL está funcionando correctamente!

---
> **Tip Profesional:** El uso combinado de CALCULATE y ALL es la base para crear reportes de participación de mercado y comparativas de rendimiento.
