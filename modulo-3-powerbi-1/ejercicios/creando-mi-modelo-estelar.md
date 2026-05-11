# Taller Práctico: Creando mi Modelo Estelar 🌟

En este ejercicio, organizaremos la información de una empresa para que Power BI pueda analizarla correctamente.

## 📥 Datos de Preparación
Imagina que tienes 3 tablas cargadas en Power BI Desktop:
1.  **Ventas**: (ID_Producto, ID_Cliente, Cantidad, Fecha). -> *Esta es tu tabla de HECHOS.*
2.  **Productos**: (ID_Producto, Nombre, Precio, Categoría). -> *Esta es una DIMENSIÓN.*
3.  **Clientes**: (ID_Cliente, Nombre_Cliente, Ciudad). -> *Esta es otra DIMENSIÓN.*

---

## 🛠 Tareas de Modelado

### 1. La Vista de Modelo
Haz click en el icono de **Modelo** (el tercer icono en la barra lateral izquierda de Power BI Desktop). Aquí verás tus tablas como rectángulos flotantes.

### 2. Creando el Puente (Relaciones)
1.  Busca el campo `ID_Producto` en la tabla **Productos**.
2.  Haz click y arrástralo hasta el campo `ID_Producto` en la tabla **Ventas**.
3.  Power BI creará una línea. Verifica que tenga un **"1"** del lado de Productos y un **"*"** del lado de Ventas.
4.  Repite el proceso para conectar `ID_Cliente` de la tabla **Clientes** con la tabla **Ventas**.

### 3. Organizando el Lienzo
Para que tu modelo sea fácil de leer por otros colegas:
*   Coloca la tabla de **HECHOS (Ventas)** en el centro y abajo.
*   Coloca las **DIMENSIONES (Productos, Clientes)** arriba, rodeando a la tabla de hechos. 
*   *¿Ves por qué se llama Esquema en Estrella?* La tabla de hechos es el centro y las dimensiones son las puntas.

---

## 🏆 El Gran Beneficio
Ahora ve a la vista de **Informe** (el primer icono) y prueba esto:
1.  Arrastra el **Nombre_Cliente** de la tabla Clientes a un gráfico.
2.  Arrastra la **Cantidad** de la tabla Ventas al mismo gráfico.
3.  **¡Éxito!** Power BI sabe exactamente qué cliente compró cada cantidad gracias a la relación que acabas de crear.

---
> **Tip Profesional:** Si el modelo está bien hecho, rara vez tendrás que usar fórmulas complejas para ver resultados básicos. ¡El modelo hace el trabajo pesado por ti!
