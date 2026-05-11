# Guía de Sesión 2: Inteligencia de Tiempo (Time Intelligence)

En el mundo de los negocios, los números no significan nada sin comparación. ¿Vendimos 100? Genial, pero ¿cuánto vendimos el año pasado por estas fechas? Hoy aprenderás a hacer que Power BI viaje en el tiempo.

---

## 1. La Tabla de Calendario (Dim_Date)
Para que las funciones de tiempo funcionen, **siempre** necesitas una tabla de calendario que tenga una fila por cada día, sin saltos. Es la base de todo análisis temporal serio.

## 2. Funciones de Acumulado (YTD, QTD, MTD)
*   **TOTALYTD**: Suma todo desde el 1 de enero hasta la fecha actual. 
    *   `Ventas YTD = TOTALYTD([Ventas Totales], 'Calendario'[Fecha])`
*   **TOTALQTD**: Acumulado del trimestre.
*   **TOTALMTD**: Acumulado del mes.

## 3. Comparativas con el Pasado
*   **SAMEPERIODLASTYEAR**: Te permite ver qué pasó exactamente el año pasado en el mismo periodo.
    *   `Ventas Año Anterior = CALCULATE([Ventas Totales], SAMEPERIODLASTYEAR('Calendario'[Fecha]))`
*   **DATEADD**: La navaja suiza. Puedes retroceder o avanzar días, meses o años.

---

## 💡 El Valor del Crecimiento
Con estas funciones podrás crear la medida más famosa de los reportes gerenciales: el **% de Crecimiento (Year over Year)**. Ayudarás a tu empresa a entender si realmente están progresando o no.
