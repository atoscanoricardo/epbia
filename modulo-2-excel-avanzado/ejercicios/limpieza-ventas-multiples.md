# Taller Práctico: Limpieza de Reportes Desordenados 🧹

Has recibido un reporte de ventas mensual que viene con un formato difícil de usar. Tu misión es dejarlo impecable usando Power Query.

## 📥 El Problema (Copia en Excel)

| REPORTE DE VENTAS Q1 | | | |
| :--- | :--- | :--- | :--- |
| Generado por: Sistema v2.0 | | | |
| | | | |
| ID_Venta | Producto | Enero | Febrero |
| 101 | Laptop | 500 | 450 |
| 102 | Mouse | 20 | 25 |
| 103 | Monitor | 200 | 210 |

---

## 🛠 Tareas de Transformación (Pasos en Power Query)

1.  **Carga los datos**: Selecciona el rango y ve a `Datos > De una tabla o rango`.
2.  **Limpia el encabezado**: 
    *   Quita las primeras 3 filas (donde están los títulos del sistema y filas vacías).
    *   Usa la opción "Usar la primera fila como encabezado".
3.  **Normaliza la tabla (Unpivot)**:
    *   Selecciona las columnas "Enero" y "Febrero".
    *   Haz click derecho y selecciona **"Anulación de dinamización de columnas"**.
    *   Verás cómo los meses pasan a una sola columna. Cambia el nombre a "Mes" y "Venta".
4.  **Asegura los tipos**: Verifica que la columna "Venta" sea de tipo **Número decimal** y "Mes" sea **Texto**.
5.  **Cargar**: Haz click en `Cerrar y cargar` para devolver los datos limpios a Excel.

---

## 🏆 El Reto de la Actualización
Una vez que tengas tu tabla limpia en Excel:
1.  Agrega una nueva fila a tu tabla ORIGINAL (la que estaba sucia).
2.  Ve a tu tabla LIMPIA, haz click derecho y dale a **"Actualizar"**.
3.  ¡Observa cómo el nuevo dato aparece ya transformado sin que hayas tenido que repetir los pasos!

---
> **Recuerda:** Power Query no modifica tus datos originales, crea una copia transformada. ¡Tus fuentes siempre estarán seguras!
