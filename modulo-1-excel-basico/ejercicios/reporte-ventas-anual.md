# Ejercicio Final Semana 1: Reporte Ejecutivo de Ventas 📊

Has sido contratado para presentar el resumen de ventas del primer trimestre ante la gerencia. Debes crear un Dashboard interactivo en una sola hoja.

## 📥 Datos de Entrenamiento (Copia en Excel)

| Sede | Mes | Ventas Realizadas | Meta de Ventas | Clientes Nuevos |
| :--- | :--- | :--- | :--- | :--- |
| Norte | Enero | 45000 | 40000 | 15 |
| Norte | Febrero | 38000 | 40000 | 12 |
| Norte | Marzo | 52000 | 45000 | 20 |
| Sur | Enero | 31000 | 35000 | 8 |
| Sur | Febrero | 33000 | 35000 | 10 |
| Sur | Marzo | 29000 | 35000 | 5 |

---

## 🛠 Instrucciones de Diseño

### 1. Estructura de Datos (El Motor)
*   Convierte los datos en una **TABLA** llamada `Tbl_Reporte`.
*   Asegúrate de que las columnas numéricas tengan formato de **Contabilidad** o **Moneda**.

### 2. Análisis (Las Fórmulas)
*   Crea una columna llamada **"% de Cumplimiento"** (Ventas / Meta).
*   Usa **Formato Condicional** (Semáforo de Iconos) para el cumplimiento:
    *   Verde: >= 100%
    *   Amarillo: 80% - 99%
    *   Rojo: < 80%

### 3. Visualización (El Dashboard)
*   **Gráfico Combinado:** Crea un gráfico que muestre las "Ventas Realizadas" como **Columnas** y la "Meta de Ventas" como una **Línea**. Agrúpalo por Sede y Mes.
*   **Interactividad:** Inserta un **Segmentador de Datos** (Slicer) para la columna "Sede". Al hacer click en "Norte", todo el gráfico debe filtrarse automáticamente.
*   **Tendencia Rápida:** Al lado de los datos de cada sede, inserta un **Minigráfico de Líneas** para ver el comportamiento de los "Clientes Nuevos".

### 4. Estética Profesional
*   Quita las líneas de cuadrícula (`Vista > Líneas de cuadrícula`).
*   Agrega un título grande y elegante en la parte superior: "REPORTE TRIMESTRAL DE DESEMPEÑO".

---

## 🏆 Criterio de Éxito
Tu Dashboard debe permitir a la gerencia saber en menos de 5 segundos:
1.  ¿Cuál sede cumplió la meta en marzo?
2.  ¿Cuál es la tendencia de captación de clientes nuevos?
3.  ¿En qué mes estuvimos más lejos de la meta?

---
> **¡Felicidades!** Has completado el Módulo 1. Estás listo para el Nivel Avanzado.
