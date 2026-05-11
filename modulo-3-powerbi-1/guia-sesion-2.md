# Guía de Sesión 2: Modelado de Datos (El Corazón de Power BI)

Si Power Query es el "portero" que limpia los datos, el **Modelo de Datos** es el "arquitecto" que decide cómo se conectan las tablas para que todo funcione a la perfección. Un buen modelo hace que Power BI sea increíblemente rápido y fácil de usar.

---

## 1. El Esquema en Estrella: La Estructura de los Ganadores
En Power BI, no solemos usar una sola tabla gigante. En su lugar, usamos un **Esquema en Estrella**, que divide la información en dos tipos de tablas:

*   **Tablas de Hechos (Facts)**: Son las tablas que contienen lo que queremos medir (ej. Ventas, Pedidos, Transacciones). Suelen tener muchas filas y pocos datos de texto (solo IDs y números).
*   **Tablas de Dimensiones (Dimensions)**: Son los "diccionarios" que describen los hechos (ej. Tabla de Clientes, Tabla de Productos, Tabla de Calendario). Responden al *quién*, *dónde*, *cuándo* y *qué*.

## 2. Relaciones y Cardinalidad
Para que las tablas se hablen entre sí, creamos relaciones. Lo más común es la relación **1 a Varios (1:*)**:
*   **1**: Un producto solo aparece una vez en el Catálogo (Dimensión).
*   **\***: Ese mismo producto puede aparecer muchas veces en la tabla de Ventas (Hechos).

## 3. La Dirección del Filtro
Verás una flecha en la línea que une tus tablas. Por defecto, el filtro siempre "fluye" de la Dimensión hacia los Hechos. 
*   *Regla de Oro*: Las Dimensiones filtran a los Hechos. Si quieres saber las ventas de "Colombia", seleccionas el país en la tabla de Geografía y Power BI buscará automáticamente todas las ventas relacionadas en la tabla de Hechos.

---

## 💡 ¿Por qué es importante?
Un modelo bien diseñado evita errores de cálculo y permite que tus reportes carguen en milisegundos. Además, es la base fundamental para aprender DAX (el lenguaje de fórmulas de Power BI) en la siguiente sesión. ¡Estás dominando el arte de la arquitectura de datos!

---
> **Próximo Paso:** Construye tu primer modelo relacional en el ejercicio `creando-mi-modelo-estelar.md`.
