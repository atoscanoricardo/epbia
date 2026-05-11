# Taller Práctico: Dashboard de Recursos Humanos 👥

Como analista de RRHH, has recibido una base de datos de empleados que necesita ser procesada para el reporte anual.

## 📥 Datos de Entrada (Copia en Excel)

| ID Empleado | Nombre Completo | Fecha Ingreso | Departamento | Salario Base |
| :--- | :--- | :--- | :--- | :--- |
| ADM-2021-01 | CARLOS ARTURO RUIZ | 15/01/2021 | ADMINISTRACION | 2500 |
| VEN-2022-05 | ana maria suarez | 10/03/2022 | VENTAS | 1800 |
| TEC-2020-12 | pedro pablo leon | 01/12/2020 | TECNOLOGIA | 3200 |
| VEN-2023-02 | LUCIA MENDEZ | 20/02/2023 | VENTAS | 1900 |

---

## 🛠 Tareas de Análisis

### 1. Extracción de Metadatos (Texto)
*   **Año de Contratación:** Extrae el año que está dentro del "ID Empleado" (los 4 números del medio) usando `EXTRAE`.
*   **Primer Nombre:** Extrae solo el primer nombre de la columna "Nombre Completo" usando una combinación de `IZQUIERDA` y `HALLAR`.
*   **Correo Corporativo:** Genera un correo usando `UNIRCADENAS` con el formato: `nombre.apellido@empresa.com` (Usa `MINUSC` para que quede todo en minúsculas).

### 2. Cálculos de Tiempo (Fechas)
*   **Antigüedad:** Calcula cuántos **años completos** lleva cada empleado en la empresa usando la función `SIFECHA`.
*   **Próxima Evaluación:** Las evaluaciones son exactamente 6 meses después de la fecha de ingreso. Usa `FECHA.MES` para calcularla.

### 3. Estadísticas de Departamento (Lógica)
Crea una pequeña tabla resumen a un lado para responder:
*   ¿Cuánto es el **Salario Total** pagado solo al departamento de "VENTAS"? (`SUMAR.SI.CONJUNTO`)
*   ¿Cuántos empleados hay en "ADMINISTRACION"? (`CONTAR.SI.CONJUNTO`)
*   ¿Cuál es el **Salario Promedio** de los empleados con más de 2 años de antigüedad?

---

## 🏆 El Desafío Visual: Semáforo de Salarios
Usa **Formato Condicional** con fórmulas:
*   Si el salario es mayor al promedio de toda la lista, ilumina la fila de color verde claro.
*   Si el empleado ingresó este año, pon su nombre en **Negrita y Azul**.

---
> **Tip:** Recuerda convertir tus datos en **TABLA (Ctrl + T)** antes de empezar para que tus fórmulas sean más fáciles de leer.
