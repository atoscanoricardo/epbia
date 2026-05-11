# Taller Práctico: Dashboard Interactivo de Ventas 📊

En este ejercicio final de visualización, construirás un reporte de ventas que permita a un gerente explorar la información desde lo general hasta el detalle.

## 🛠 Tareas de Diseño

### 1. El Resumen Ejecutivo (KPIs)
1.  En la parte superior, coloca 3 **Tarjetas** con tus medidas DAX: `Ingresos Totales`, `Cantidad de Ventas` y `Ticket Promedio`.
2.  Dales un diseño limpio: quita la etiqueta de categoría y ponle un título propio más elegante.

### 2. Análisis Geográfico e Interacción
1.  Inserta un **Mapa** que muestre las ventas por "Ciudad".
2.  Al lado, inserta un **Gráfico de Barras** por "Categoría".
3.  **Prueba la interacción**: Haz click en una ciudad en el mapa. Verás cómo el gráfico de barras se resalta automáticamente para mostrarte las ventas de esa ciudad específica.

### 3. Implementando el Drill-Down
1.  Crea un **Gráfico de Columnas**.
2.  En el "Eje X", arrastra primero el campo **Categoría** y debajo de él el campo **Nombre Producto**.
3.  Activa el botón de "Drill-down" (la flecha hacia abajo) en el gráfico.
4.  Haz click en una categoría (ej. "Hardware") y observa cómo el gráfico cambia para mostrarte los productos específicos de esa categoría.

### 4. Filtros de Control
1.  Agrega un **Segmentador (Slicer)** de tipo "Menú desplegable" para el campo **Año**.
2.  Configúralo para que sea un "Filtro de selección única" (para que el reporte siempre muestre un año a la vez).

---

## 🏆 El Gran Reto Final: Tooltip Personalizado
1.  Crea una nueva página de reporte llamada `Tooltip_Producto`.
2.  En la configuración de la página, activa la opción **"Información sobre herramientas"**.
3.  Crea un pequeño gráfico de pastel en esa página que muestre el % de ventas por ciudad.
4.  Vuelve a tu página principal, selecciona el gráfico de productos, ve a Formato > Información sobre herramientas y elige la página `Tooltip_Producto`.
5.  **Resultado**: ¡Al pasar el mouse sobre un producto, verás el gráfico de pastel apareciendo mágicamente!

---
> **Meta:** Tu dashboard debe ser tan intuitivo que no necesite un manual de instrucciones. ¡La curiosidad del usuario debe guiar el análisis!
