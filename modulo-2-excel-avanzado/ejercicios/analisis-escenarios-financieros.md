# Taller Práctico: Planificación Financiera y Escenarios 📈

En este ejercicio final de la semana, ayudaremos a un emprendedor a proyectar sus ganancias y a tomar decisiones bajo diferentes condiciones del mercado.

## 📥 El Modelo de Negocio (Copia en Excel)

| Concepto | Valor |
| :--- | :--- |
| Precio de Venta | 150 |
| Unidades Vendidas | 200 |
| Costo Unitario | 80 |
| Costos Fijos | 5000 |
| **Utilidad Total** | **9000** | *(Fórmula: (Precio-Costo)*Unidades - Fijos)*

---

## 🛠 Retos de Análisis

### 1. El Punto de Equilibrio (Buscar Objetivo)
El emprendedor quiere saber exactamente cuántas unidades debe vender para que su utilidad sea **0** (punto de equilibrio).
1.  Usa `Buscar Objetivo`.
2.  Definir la celda: Utilidad Total.
3.  Con el valor: `0`.
4.  Cambiando la celda: Unidades Vendidas.
*   **Resultado**: ¿Cuántas unidades necesita vender para no perder dinero?

### 2. Proyectando el Futuro (Administrador de Escenarios)
Vamos a crear 3 visiones del negocio:
*   **Escenario A (Pesimista)**: Precio baja a 130 y Unidades bajan a 150.
*   **Escenario B (Actual)**: Los valores que tienes ahora (150 y 200).
*   **Escenario C (Optimista)**: Precio sube a 170 y Unidades suben a 300.

**Pasos:**
1.  Ve a `Análisis de hipótesis > Administrador de escenarios`.
2.  Agrega cada escenario dándole un nombre y seleccionando las celdas de "Precio" y "Unidades" como celdas cambiantes.
3.  Una vez creados los 3, haz click en el botón **Resumen**.
*   **Resultado**: Excel creará una hoja nueva comparando los 3 casos.

---

## 🏆 El Desafío Final: Optimización con Solver
(Si tienes Solver activado)
Encuentra la combinación ideal:
*   **Objetivo**: Maximizar la Utilidad.
*   **Restricción 1**: No puedes vender más de 500 unidades (capacidad de producción).
*   **Restricción 2**: El precio no puede ser mayor a 200 (competencia).
*   **Restricción 3**: El costo unitario sube a 90 si produces más de 400 unidades.

---
> **¡Felicitaciones!** Has terminado el Módulo 2. Ahora tienes las herramientas para enfrentar cualquier desafío de datos con confianza y profesionalismo.
