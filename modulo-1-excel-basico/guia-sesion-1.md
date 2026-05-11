# Guía de Sesión 1: Domina la Interfaz y los Cimientos

Para ser un experto en Excel, no necesitas saber mil fórmulas; necesitas entender cómo Excel "piensa". En esta sesión transformaremos tu relación con la cuadrícula.

---

## 1. El ADN de Excel: ¿Por qué fallan los archivos?
La mayoría de los errores en Excel ocurren por una mala estructura inicial.
*   **Formatos Pro:** Nunca uses `.xlsx` si vas a tener macros (usa `.xlsm`) o si el archivo es gigante (usa `.xlsb` - Binario).
*   **La Cinta de Opciones:** Vamos a limpiar el desorden. 
    *   *Truco:* Click derecho en cualquier pestaña > "Personalizar cinta de opciones" > Activa la pestaña **Programador**.

## 2. Gestión Ninja de Datos (Sin escribir)
*   **Flash Fill (Control + E):** La función más "mágica" de Excel. Si tienes una columna con "Juan Perez" y quieres separar el nombre, escribe "Juan" en la celda de al lado y presiona `Ctrl + E`. Excel aprenderá el patrón.
*   **Validación de Datos con Listas:** Evita que los usuarios escriban "Bogotá", "bogota" y "BOG". Estandariza la entrada.

## 3. El Poder de las Referencias ($)
Dominar el uso de los signos de pesos es uno de los pasos más importantes para ganar agilidad en Excel. Estas referencias nos permiten automatizar cálculos complejos con facilidad:
*   `A1`: **Referencia Relativa**. Cambia al mover la fórmula (ideal para cálculos en serie).
*   `$A$1`: **Referencia Absoluta**. Se mantiene fija sin importar a dónde muevas la fórmula (perfecto para tasas de IVA o valores fijos).
*   `$A1`: **Mixta (Columna fija)**. Permite que la fila cambie, pero la columna se mantiene constante.
*   `A$1`: **Mixta (Fila fija)**. Permite que la columna cambie, pero la fila se mantiene constante.

---

## ⚡ Reto de la Sesión: "Startup Coffee Shop"
Imagina que eres el Data Analyst de una nueva cadena de café. Tus datos están sucios y las fórmulas no funcionan.

1.  **Limpieza:** Usa `LIMPIAR` y `ESPACIOS` para corregir los nombres de los productos que vienen de un sistema viejo.
2.  **Cálculos Dinámicos:** Crea una fórmula de IVA que siempre apunte a una celda fija de "Configuración" usando `$`.
3.  **Visualización Flash:** Inserta minigráficos (Sparklines) para ver la tendencia de ventas de cada barista en una sola celda.

---

> **Próximo Paso:** Ve a la carpeta `/ejercicios` y abre el archivo `caso-cafe-startup.md` para empezar el taller práctico.
