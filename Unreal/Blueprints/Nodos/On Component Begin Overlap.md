---
Tipo:
  - Nodo de flujo
---
# Nodo: On Component Begin Overlap
## Descripción
El nodo **On Component Begin Overlap** se utiliza para detectar cuándo otro objeto o actor comienza a superponerse con un componente específico, como un **Collision Box**, **Static Mesh** o cualquier componente con colisión habilitada.

---
## Funcionalidad
- **Evento dinámico:** Este nodo se ejecuta automáticamente cuando ocurre una superposición en tiempo de ejecución.
- **Usos comunes:**
  - Activar eventos al entrar en un área (trampas, activación de puertas, etc.).
  - Detectar interacciones entre el jugador y objetos.
  - Generar señales en sistemas de juego basados en colisiones.

---
## Entradas
- **None:** Este nodo no requiere entradas.

---
## Salidas
- **Other Actor:** Referencia al actor que comenzó la superposición.
- **Other Component:** Referencia al componente del actor que se superpone.
- **Other Body Index:** Índice del cuerpo físico asociado (en casos de física compleja).
- **b From Sweep:** Booleano que indica si la superposición ocurrió como parte de un movimiento barrido.
- **Sweep Result:** Información detallada sobre el impacto (si aplica).