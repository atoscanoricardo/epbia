# Taller Práctico: Análisis de Crecimiento Temporal ⏳

El objetivo de este taller es comparar el rendimiento de este año contra el anterior para detectar tendencias de crecimiento.

## 🛠 Tareas de Inteligencia de Tiempo

### 1. Creación del Calendario
Si aún no tienes una tabla de calendario, ve a la pestaña `Modelado > Nueva Tabla` y pega este código:
`Calendario = CALENDARAUTO()`
*   *Nota*: Asegúrate de marcarla como "Tabla de fechas" en el menú superior.

### 2. Acumulados del Año (YTD)
Crea una medida que muestre cuánto llevamos vendido en el año actual:
*   `Ventas Acumuladas YTD = TOTALYTD([Ingresos Totales], 'Calendario'[Date])`

### 3. Comparativa Año Anterior
¿Cuánto vendimos en este mismo periodo el año pasado?
*   `Ventas SPLY = CALCULATE([Ingresos Totales], SAMEPERIODLASTYEAR('Calendario'[Date]))`

### 4. El KPI Maestro: % de Crecimiento
Calcula cuánto hemos crecido (o decrecido) comparado con el año anterior:
*   `Crecimiento YoY % = DIVIDE([Ingresos Totales] - [Ventas SPLY], [Ventas SPLY])`

---

## 🏆 Visualización de Tendencias
1.  Crea un **Gráfico de Líneas**.
2.  En el "Eje X" pon el **Mes** de tu tabla de Calendario.
3.  En "Valores" pon `Ingresos Totales` y `Ventas SPLY`.
*   **Análisis**: Podrás ver visualmente en qué meses superaste al año anterior y en cuáles estuviste por debajo.

---
> **Reflexión:** Sin DAX, hacer esta comparación mes a mes te tomaría horas de fórmulas manuales. ¡Power BI lo hace en segundos!
