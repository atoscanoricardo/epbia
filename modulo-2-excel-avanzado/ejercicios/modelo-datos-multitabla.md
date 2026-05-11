# Taller Práctico: Análisis Multi-Tabla (Sin BUSCARV) 🔗

En este ejercicio, actuarás como el consultor de una cadena de tiendas. Tienes dos tablas separadas y debes crear un reporte unificado.

## 📥 Datos de Origen (Copia en Excel)

### Tabla 1: Ventas (Nombre de tabla: `Tbl_Ventas`)
| ID_Producto | Cantidad | Fecha |
| :--- | :--- | :--- |
| P01 | 10 | 01/05/2026 |
| P02 | 5 | 02/05/2026 |
| P01 | 2 | 03/05/2026 |

### Tabla 2: Catálogo (Nombre de tabla: `Tbl_Productos`)
| ID_Producto | Nombre Producto | Precio |
| :--- | :--- | :--- |
| P01 | Café Espresso | 2.5 |
| P02 | Latte Macchiato | 3.5 |

---

## 🛠 Pasos para el Modelado

1.  **Crea las Tablas**: Convierte ambos rangos en Tablas (`Ctrl + T`) y dales los nombres indicados arriba.
2.  **Crea la Tabla Dinámica**:
    *   Ve a `Insertar > Tabla Dinámica`.
    *   **¡Importante!**: Marca la casilla *"Agregar estos datos al Modelo de datos"*.
3.  **Crea la Relación**:
    *   Una vez abierta la Tabla Dinámica, ve a la pestaña `Análisis de tabla dinámica > Relaciones`.
    *   Haz click en `Nuevo` y conecta `Tbl_Ventas` (ID_Producto) con `Tbl_Productos` (ID_Producto).
4.  **Diseña el Reporte**:
    *   Arrastra el **Nombre Producto** (de la tabla de Catálogo) a las Filas.
    *   Arrastra la **Cantidad** (de la tabla de Ventas) a los Valores.
5.  **Crea una Medida DAX (Opcional/Avanzado)**:
    *   Ve a la pestaña `Power Pivot` (o haz click derecho en el nombre de la tabla en el panel lateral de la Tabla Dinámica) y selecciona `Agregar medida`.
    *   Nombre: `Ingreso Total`.
    *   Fórmula: `=SUMX(Tbl_Ventas, Tbl_Ventas[Cantidad] * RELATED(Tbl_Productos[Precio]))`.

---

## 🏆 El Dashboard Final
1.  Inserta un **Segmentador** por "Nombre Producto".
2.  Inserta una **Escala de Tiempo** por "Fecha".
3.  Comprueba que, al filtrar, todo tu reporte se ajusta perfectamente usando datos de ambas tablas a la vez.

---
> **Reflexión:** ¿Notaste que no tuvimos que escribir ni un solo BUSCARV para saber cuánto dinero generó el Café Espresso? ¡Esa es la eficiencia del modelado!
