# Guía de Sesión 4: Seguridad y Gobierno de Datos (RLS)

Cuando manejas información sensible (como salarios o datos de clientes), no todos deben ver todo. Hoy aprenderás a configurar la **Seguridad a Nivel de Fila (Row-Level Security)**.

---

## 1. ¿Qué es RLS?
Es una técnica que permite que un mismo reporte muestre datos diferentes según quién lo abra.
*   **Ejemplo**: El gerente de ventas de "Norte" solo ve los datos de su sede, mientras que el Director General ve todo el país.

## 2. Roles y DAX de Seguridad
Aprenderás a crear "Roles" (ej. Rol_Vendedores) y a usar fórmulas DAX simples para filtrar sus datos.
*   Filtro: `[Ciudad] = "Bogotá"`
*   Esto asegura que los datos estén protegidos desde el origen.

## 3. Publicación y Gateways
Entenderemos cómo mantener los datos actualizados automáticamente cuando la fuente es un archivo local en tu computadora, usando los **Gateways** (Puertas de enlace).

---

## 💡 Responsabilidad y Ética
Como analista de datos, eres el guardián de la información. Configurar correctamente la seguridad no es solo una tarea técnica, es un compromiso ético con la privacidad de tu organización.
