# Taller Práctico: Gestión de Inventarios Inteligente 📦

En este reto, ayudaremos a una distribuidora de tecnología a organizar su inventario usando las funciones más potentes de Excel Avanzado.

## 📥 Datos de la Bodega (Copia en Excel)

| SKU | Producto | Categoría | Stock | Precio Unitario |
| :--- | :--- | :--- | :--- | :--- |
| TEC-001 | Laptop Pro | Hardware | 15 | 1200 |
| TEC-002 | Mouse Wireless | Accesorios | 50 | 25 |
| TEC-003 | Monitor 4K | Hardware | 8 | 450 |
| TEC-004 | Teclado Mecánico | Accesorios | 0 | 80 |
| TEC-005 | Disco SSD | Almacenamiento | 22 | 110 |

---

## 🛠 Tareas de Automatización

### 1. El Buscador Maestro (BUSCARX)
Crea una zona de consulta donde, al escribir un **SKU**, Excel te devuelva automáticamente el **Producto** y el **Precio**.
*   **Reto:** Si el SKU no existe, la fórmula debe mostrar el mensaje: *"Producto no registrado"*.

### 2. Extracción de Categorías (UNICOS y ORDENAR)
A un lado de tu tabla, genera automáticamente una lista de todas las **Categorías** que existen en la bodega, sin que se repitan y organizadas alfabéticamente.
*   *Beneficio:* Esta lista se actualizará sola si mañana agregas una categoría nueva como "Software".

### 3. Filtro de Stock Crítico (FILTRAR)
Crea una sección llamada **"Alerta de Reposición"**. Usa la función `FILTRAR` para que Excel muestre automáticamente todos los productos cuyo **Stock sea menor a 10**.
*   *Nota:* Verás cómo los resultados "derraman" hacia abajo automáticamente.

### 4. Validador Dinámico
Crea una lista desplegable (Validación de Datos) para elegir una categoría. Debajo de ella, usa `FILTRAR` para mostrar todos los productos que pertenecen a la categoría seleccionada.

---

## 🏆 Reflexión Final
Observa cómo, al cambiar un dato en la tabla principal (ej. bajar el stock de un producto a 5), todos tus reportes auxiliares se actualizan al instante sin que tengas que volver a filtrar o copiar nada. ¡Ese es el poder de la automatización dinámica!

---
> **Tip Profesional:** Recuerda que puedes combinar funciones. Por ejemplo: `=ORDENAR(UNICOS(C2:C100))` para obtener una lista limpia y organizada en un solo paso.
