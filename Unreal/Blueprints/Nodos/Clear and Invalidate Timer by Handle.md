---
Tipo:
  - Nodo de flujo
---
# Nodo: Clear and Invalidate Timer by Handle
## Descripción
El nodo **Clear and Invalidate Timer by Handle** se utiliza para detener un temporizador (Timer) y marcarlo como no válido, liberando así cualquier recurso asociado. Es útil para manejar temporizadores dinámicos y asegurarse de que ya no se ejecuten o consuman recursos.

---
## Funcionalidad
- **Finaliza un temporizador activo:** Detiene la ejecución del temporizador identificado por su "Handle".
- **Invalida el temporizador:** Asegura que el "Handle" ya no sea válido, previniendo futuros usos no intencionados.
- **Control dinámico:** Es comúnmente usado en sistemas que dependen de la manipulación y limpieza de temporizadores en tiempo de ejecución.

---
## Entradas
1. **Timer Handle:** (Tipo: `FTimerHandle`) El identificador del temporizador que se desea detener e invalidar. Este Handle es generado al iniciar el temporizador con nodos como **Set Timer by Function Name** o **Set Timer by Event**.

---
## Salidas
- Este nodo no tiene salidas directas.