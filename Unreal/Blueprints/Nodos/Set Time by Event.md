---
Tipo:
  - Nodo de flujo
---
# Nodo: Set Timer by Event

## Descripción
El nodo **Set Timer by Event** permite configurar un temporizador que ejecutará un evento personalizado después de un intervalo de tiempo específico. Es útil para programar tareas repetitivas o diferidas.

---
## Entradas
1. **Event:** Referencia al evento que se ejecutará cuando el temporizador finalice.
2. **Time:** (Tipo: `Float`) Tiempo en segundos antes de que se dispare el evento.
3. **Looping:** (Tipo: `Boolean`) Define si el temporizador debe repetirse indefinidamente.

---
## Salidas
- **Timer Handle:** (Tipo: `FTimerHandle`) Identificador del temporizador creado, útil para manipularlo posteriormente.