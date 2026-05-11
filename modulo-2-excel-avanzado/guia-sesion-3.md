# Guía de Sesión 3: Tablas Dinámicas Pro y Power Pivot

Hasta ahora hemos trabajado con una sola tabla a la vez. Pero en el mundo real, la información suele estar repartida en varios archivos (ej. una tabla de "Ventas", otra de "Clientes" y otra de "Productos"). Hoy aprenderás a unirlas todas sin usar ni un solo BUSCARV.

---

## 1. El Modelo de Datos (Power Pivot)
El Modelo de Datos es como un "pegamento" inteligente. Permite que Excel entienda que el "ID_Producto" en tu tabla de ventas es el mismo que está en tu catálogo de productos.
*   **Ventaja**: Tus archivos pesan menos y son mucho más rápidos.
*   **Cómo empezar**: Al crear una Tabla Dinámica, asegúrate de marcar la casilla **"Agregar estos datos al Modelo de datos"**.

## 2. Relaciones: El fin del BUSCARV
En lugar de traer manualmente el nombre del producto a la tabla de ventas, creamos una **Relación**. 
*   Imaginalo como un puente: Una vez construido, puedes arrastrar el "Nombre del Producto" directamente a tu Tabla Dinámica y Excel sabrá exactamente cuánto se vendió de cada uno.

## 3. Campos Calculados vs. Medidas DAX
*   **Campos Calculados**: Son cálculos simples dentro de una tabla dinámica tradicional (ej. Ventas * 0.10).
*   **Medidas DAX (Data Analysis Expressions)**: Son fórmulas mucho más potentes que viven en el Modelo de Datos. 
    *   *Ejemplo de Medida:* `Total Ventas := SUM([Monto])`. 
    *   La gran ventaja de las medidas es que son inteligentes y se adaptan a cualquier filtro que pongas en tu reporte.

## 4. Segmentadores y Escalas de Tiempo
Para que tu reporte sea realmente "Pro", usaremos herramientas visuales:
*   **Segmentadores (Slicers)**: Botones para filtrar por Categoría, Ciudad, etc.
*   **Escalas de Tiempo**: Un control deslizante especial para filtrar fechas por meses, trimestres o años con un solo toque.

---

## 💡 Un Salto de Calidad
Aprender a modelar datos es lo que separa a un usuario de Excel de un **Analista de Datos**. Esta estructura que estamos aprendiendo hoy es la base exacta sobre la que funciona Power BI. ¡Estás construyendo el puente hacia tu futuro éxito!

---
> **Próximo Paso:** Pon manos a la obra con el ejercicio `modelo-datos-multitabla.md`.
