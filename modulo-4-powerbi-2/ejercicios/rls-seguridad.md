# Taller Práctico: Configurando Seguridad por Región (RLS) 🛡️

Garantizaremos que cada gerente solo pueda ver la información de su propia ciudad.

## 🛠 Pasos para la Seguridad

### 1. Crear el Rol
1.  En Power BI Desktop, ve a la pestaña **Modelado > Administrar roles**.
2.  Haz click en `Crear` y ponle el nombre `Gerente_Bogota`.
3.  En las tablas de la izquierda, selecciona tu tabla de **Geografía** o **Sedes**.
4.  Escribe la regla DAX: `[Ciudad] = "Bogotá"`.
5.  Haz click en Guardar.

### 2. Probar la Seguridad
1.  En la misma pestaña Modelado, haz click en **Ver como**.
2.  Marca la casilla de `Gerente_Bogota`.
3.  **¡Observa!** Tu reporte completo se filtrará automáticamente. Si tenías ventas en 10 ciudades, ahora solo verás Bogotá.
4.  Haz click en "Detener visualización" para volver a ver todo.

### 3. Publicación
Una vez que subas el reporte a Power BI Service:
1.  Ve a la configuración del **Conjunto de datos**.
2.  Busca la opción **Seguridad**.
3.  Agrega los correos electrónicos de las personas que deben pertenecer al rol de Bogotá.

---

## 🏆 Criterio de Éxito
Cuando el gerente de Bogotá abra el reporte, no verá un mensaje de "Acceso denegado", simplemente verá sus datos como si no existiera nada más. ¡Privacidad y limpieza total!
