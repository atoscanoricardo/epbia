# Guía de Sesión 3: El Arte de Presentar Datos (Storytelling Visual)

Un reporte que nadie entiende es un reporte que no sirve. En esta sesión aprenderemos a pasar de "tablas aburridas" a tableros de control (Dashboards) que facilitan la toma de decisiones.

---

## 1. Menos es Más: Limpieza Visual
Antes de insertar un gráfico, debemos limpiar la "ruido":
*   **Adiós a las líneas de cuadrícula:** Ve a la pestaña `Vista` y desactiva "Líneas de cuadrícula". Esto hace que tu reporte parezca una aplicación o sitio web, no una hoja de cálculo.
*   **Colores con Propósito:** No uses colores al azar. Usa el color de la marca de tu empresa o usa gris para lo neutral y un color fuerte (como azul o naranja) para lo que quieres resaltar.

## 2. Gráficos de Alto Impacto
*   **Gráficos Combinados:** Úsalos para comparar dos métricas diferentes (ej. Barras para "Ventas" y una Línea para "% de Margen").
*   **Minigráficos (Sparklines):** Gráficos que viven dentro de una celda. Perfectos para mostrar tendencias de los últimos 6 meses sin ocupar espacio.
*   **Segmentadores de Datos (Slicers):** Son botones interactivos que filtran tus tablas y gráficos con un click. *Nota: Solo funcionan si tus datos están en formato de TABLA.*

## 3. Preparación para el Nivel Avanzado
¿Por qué insistimos tanto en las **Tablas (Ctrl + T)**?
1.  **Rangos Dinámicos:** Si agregas un nuevo dato al final, la tabla crece sola y tus gráficos se actualizan automáticamente.
2.  **Referencias Estructuradas:** En lugar de `=SUMA(A2:A500)`, verás `=SUMA(Ventas[Total])`. Mucho más fácil de entender.
3.  **Puente a Power BI:** Power BI ama las tablas. Si aprendes a estructurarlas bien aquí, la Semana 3 será pan comido.

---

## ⚡ El Checklist de un Reporte Profesional
1.  [ ] ¿Tiene un título claro?
2.  [ ] ¿Los números tienen formato de moneda o millares?
3.  [ ] ¿Se eliminaron las líneas de cuadrícula de Excel?
4.  [ ] ¿Es interactivo (tiene segmentadores)?

---
> **Próximo Paso:** Realiza el ejercicio final `reporte-ventas-anual.md` para graduarte de la Semana 1.
