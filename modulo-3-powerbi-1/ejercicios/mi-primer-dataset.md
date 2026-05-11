# Taller Práctico: Mi Primer Dataset en Power BI 🚀

En este primer ejercicio, aprenderemos a traer datos desde la web y desde Excel para crear la base de un tablero de control.

## 📥 Paso 1: Obtener Datos de la Web
Imagina que quieres analizar el valor del dólar para tus ventas.
1.  En Power BI Desktop, ve a `Obtener Datos > Web`.
2.  Busca una URL que contenga una tabla de divisas (o usa una de ejemplo que te proporcione el instructor).
3.  Selecciona la tabla en el Navegador y haz click en **Transformar Datos**.

## 🛠 Paso 2: Limpieza en Power Query (BI)
Dentro del editor:
1.  **Elimina columnas innecesarias**: Quédate solo con "Moneda" y "Valor".
2.  **Cambia el tipo de dato**: Asegúrate de que el Valor sea "Número decimal". Si tiene puntos o comas que Excel/Power BI no reconoce, usa "Reemplazar valores".
3.  **Renombra la consulta**: Ponle un nombre claro como `Dolar_Hoy`.

## 📥 Paso 3: Conectar con tus Ventas (Excel)
1.  Sin cerrar Power Query, ve a `Nueva Fuente > Excel`.
2.  Carga un archivo de ventas que hayas creado en el Módulo 1.
3.  Usa la función **Anular dinamización de columnas** si tus datos tienen meses en las columnas.

---

## 🏆 El Resultado Esperado
Al finalizar, debes tener dos tablas cargadas en el panel de **Datos** (a la derecha) de Power BI Desktop.
*   `Dolar_Hoy` (Datos de la web).
*   `Ventas_Historicas` (Tus datos de Excel limpios).

---
> **Reflexión:** ¿Notaste que el editor de Power Query es idéntico al de Excel? ¡Toda tu experiencia previa te está sirviendo ahora mismo para ser un experto en BI!
