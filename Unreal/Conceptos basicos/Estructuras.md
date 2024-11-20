# Estructuras
## Descripción
Las estructuras (`Structs`) son colecciones de datos que agrupan múltiples valores bajo un solo contenedor. Se utilizan para organizar datos complejos.

---
## Características
- Pueden contener varios tipos de datos: `Boolean`, `Integer`, `Float`, `String`, `Vector`, etc.
- Los valores individuales dentro de una estructura se llaman **campos** o **miembros**.
- Simplifican el manejo de datos relacionados.

---
## Cómo Crear una Estructura
1. Ve al **Content Browser** y haz clic derecho.
2. Selecciona **Blueprints > Structure**.
3. Define los campos con su tipo correspondiente en el editor de la estructura.

---
## Usos Comunes
1. **Agrupación de datos relacionados**: Ejemplo: Información de un personaje (nombre, salud, nivel).
2. **Tablas de datos**: Combina estructuras con **Data Tables** para manejar configuraciones o estadísticas masivas.
3. **Organización y reutilización**: Mejora la claridad al manejar datos relacionados.

---
## Ejemplo
Una estructura para un inventario de armas:
- **Nombre**: `String`
- **Daño**: `Float`
- **Peso**: `Float`
- **Rareza**: `Enum`

---
## Ventajas
- Evitan la creación de múltiples variables independientes.
- Permiten actualizar y acceder a datos relacionados de forma centralizada.