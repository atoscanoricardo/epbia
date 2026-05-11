# Taller Práctico: Mis Primeras Medidas DAX 🧮

En este ejercicio, crearemos los indicadores clave (KPIs) para una tienda de electrónica. Usaremos los datos que cargamos y modelamos en las sesiones anteriores.

## 🛠 Tareas de Cálculo

### 1. La Medida Base: Ingresos Totales
1.  En el panel de **Datos**, haz click derecho en la tabla `Ventas` y selecciona **Nueva medida**.
2.  Escribe la fórmula:
    `Ingresos Totales = SUM(Ventas[Monto])`
3.  Formato: Selecciona la medida y en la pestaña "Herramientas de medición" ponle formato de **Moneda ($)**.

### 2. Contando nuestra Actividad
1.  Crea una medida para saber cuántas ventas hemos realizado:
    `Cantidad de Ventas = COUNTROWS(Ventas)`
2.  Crea una medida para saber cuántos clientes diferentes nos han comprado:
    `Clientes Unicos = DISTINCTCOUNT(Ventas[ID_Cliente])`

### 3. Calculando el Ticket Promedio (DIVIDE)
¿Cuánto nos compra un cliente en promedio cada vez que viene?
1.  Crea la medida:
    `Ticket Promedio = DIVIDE([Ingresos Totales], [Cantidad de Ventas])`
2.  *¿Por qué usamos DIVIDE?* Porque si un día no tenemos ventas, la fórmula no nos dará un error, simplemente quedará en blanco.

---

## 🏆 El Dashboard de KPIs
Ahora que tienes tus medidas, vamos a visualizarlas:
1.  Arrastra un objeto visual de **Tarjeta** (Card) al lienzo.
2.  Pon la medida `Ingresos Totales` en ella.
3.  Crea otras tarjetas para `Clientes Unicos` y `Ticket Promedio`.
4.  Agrega un **Segmentador** (Slicer) con la columna "Categoría" de la tabla Productos.
5.  **¡Observa la magia!** Al cambiar la categoría, todas tus tarjetas DAX se recalculan instantáneamente para mostrarte solo los datos de esa categoría.

---
> **Reto Extra:** Intenta crear una medida llamada `Venta Maxima` usando la función `MAX(Ventas[Monto])`. ¿Cuál fue el pedido más grande de la historia de la tienda?
