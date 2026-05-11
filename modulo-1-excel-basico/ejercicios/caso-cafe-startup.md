# Taller Práctico: Caso "Startup Coffee Shop" ☕

Este ejercicio simula un entorno real de trabajo. Tu objetivo es transformar una lista de ventas desordenada en un reporte profesional.

## 📥 Datos de Origen (Copia esto en Excel)

| Fecha | Barista | Producto | Precio Unitario | Cantidad | Total Bruto |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 01/05/2026 | juan perez | Latte | 3.5 | 2 | |
| 01/05/2026 | MARIA LOPEZ | Capuccino | 4.0 | 5 | |
| 02/05/2026 | juan perez | expresso | 2.5 | 10 | |
| 02/05/2026 | maria lopez | Latte | 3.5 | 1 | |

---

## 🛠 Tareas a Realizar

### Fase 1: Limpieza Inteligente
1.  **Formato de Nombres:** Crea una nueva columna llamada "Barista Limpio". Usa la función `NOMPROPIO()` para que "juan perez" se convierta en "Juan Perez".
2.  **Relleno Rápido:** En la columna "Código Producto", escribe el código del primer producto manualmente (Ej: LAT-01) y usa `Ctrl + E` para que Excel genere el resto basándose en el nombre.

### Fase 2: Lógica Financiera
1.  **Cálculo de Totales:** En "Total Bruto", multiplica Precio * Cantidad.
2.  **IVA Dinámico:** Crea una celda fuera de la tabla (ej. en `H1`) que diga "19%". Calcula el IVA en una nueva columna usando **referencias absolutas** (`$H$1`) para que puedas arrastrar la fórmula sin errores.

### Fase 3: Validación y Estándares
1.  **Lista Desplegable:** Configura la columna "Producto" para que solo permita elegir entre: *Latte, Capuccino, Expresso, Mocca*.
2.  **Alerta de Stock:** Usa **Formato Condicional** para que si la "Cantidad" es mayor a 8, la celda se ponga en rojo con texto blanco (Alerta de alta demanda).

---

## 🏆 Bonus: El Reporte Ejecutivo
Convierte todo el rango de datos en una **TABLA** (`Ctrl + T`). 
*   Dale un nombre a la tabla: `Tbl_Ventas`.
*   Activa la "Fila de Totales".
*   Inserta un **Segmentador de Datos** por "Barista" para filtrar las ventas con un solo click.

---
> **Meta:** El reporte debe verse limpio, profesional y ser a prueba de errores humanos.
