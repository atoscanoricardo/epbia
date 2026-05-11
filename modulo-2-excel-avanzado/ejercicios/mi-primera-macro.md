# Taller Práctico: Tu Primer Botón de Automatización 🤖

Hoy crearemos una macro que limpie automáticamente un formulario de entrada de datos, ahorrándonos el trabajo de borrar celda por celda.

## 📥 El Escenario (Copia en Excel)

Imagina un formulario simple de registro de pedidos:
*   Celda B2: Nombre Cliente
*   Celda B3: Producto
*   Celda B4: Cantidad

Escribe algunos datos de prueba en esas celdas.

---

## 🛠 Pasos para Crear la Macro

### 1. Preparación
*   Asegúrate de tener datos en B2, B3 y B4.
*   Ve a la pestaña `Programador` y selecciona **Grabar macro**.
*   Nombre de la macro: `LimpiarFormulario`.
*   Asigna una tecla de método abreviado (opcional): `Ctrl + Shift + L`.

### 2. La Grabación (¡Atención!)
Desde este momento, Excel está grabando. Realiza solo estos pasos:
1.  Selecciona el rango `B2:B4`.
2.  Presiona la tecla `Suprimir` (Delete) para borrar el contenido.
3.  Selecciona la celda `B2` (para que el cursor quede listo para el siguiente pedido).
4.  Ve a la pestaña `Programador` y haz click en **Detener grabación**.

### 3. El Toque Profesional: El Botón
Una macro es más divertida si tiene un botón:
1.  Ve a `Insertar > Ilustraciones > Formas` y dibuja un rectángulo pequeño al lado del formulario.
2.  Escribe "LIMPIAR" dentro de la forma y dale un color bonito.
3.  Haz click derecho sobre la forma y selecciona **Asignar macro**.
4.  Elige `LimpiarFormulario` de la lista y dale a Aceptar.

---

## 🏆 El Desafío Final
1.  Llena el formulario con datos nuevos.
2.  Presiona tu nuevo botón.
3.  **¡Magia!** Los datos desaparecen y el cursor vuelve a la primera celda.

---
> **Tip:** No olvides guardar tu archivo como **Libro de Excel habilitado para macros (.xlsm)** o perderás tu trabajo al cerrar el archivo.
