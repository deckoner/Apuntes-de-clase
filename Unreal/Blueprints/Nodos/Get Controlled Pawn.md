# Nodo: Get Controlled Pawn
## Descripción
El nodo **Get Controlled Pawn** se utiliza para obtener el **Pawn** que está actualmente siendo controlado por un **PlayerController**. Este nodo es útil cuando se necesita acceder al actor o personaje que el jugador está controlando en el juego, permitiendo manipularlo o interactuar con él de manera directa.

---
## Funcionalidad

- **Obtención del Pawn controlado:** Devuelve el **Pawn** que está siendo controlado activamente por el **PlayerController**.
- **Usos comunes:**
    - Acceder al **Pawn** del jugador para realizar acciones, como moverlo, actualizar su estado o aplicar habilidades.
    - Verificar qué **Pawn** está siendo controlado en caso de que haya múltiples jugadores o personajes en el juego.
    - Obtener el **Pawn** para manipular su posición, rotación o aplicar efectos específicos.

---
## Entradas

- **Target:** El **PlayerController** que está controlando el **Pawn**. Este valor puede ser el **PlayerController** actual o uno específico si se está trabajando con múltiples controladores de jugador.

---
## Salidas

- **Return Value:** Devuelve el **Pawn** que está siendo controlado por el **PlayerController** especificado. Esto puede ser cualquier tipo de **Pawn**, como un personaje, vehículo o cualquier otro actor que pueda ser controlado.