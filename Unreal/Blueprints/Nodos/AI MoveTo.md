# Nodo: AI MoveTo

## Descripción

El nodo **AI MoveTo** se utiliza para ordenar a un **Pawn** controlado por una **AIController** que se mueva a una ubicación específica en el mundo. Este nodo es esencial para la navegación y la inteligencia artificial en los videojuegos, permitiendo que los personajes controlados por IA se desplacen hacia un objetivo de manera autónoma.

---

## Funcionalidad

- **Movimiento de IA:** Ordena al **Pawn** controlar su movimiento hacia una **Destination** específica.
- **Usos comunes:**
    - Desplazar a un personaje de IA hacia un punto específico en el mapa.
    - Hacer que un personaje de IA persiga o se acerque a un **Target Actor**.
    - Implementar movimientos en situaciones como patrullaje, persecución o huida.

---

## Entradas

- **In:** Señal de ejecución que activa la operación del nodo.
- **Pawn:** El actor que se moverá. Generalmente, este es el **Pawn** controlado por la **AIController**.
- **Destination:** La ubicación en el mundo a la que el **Pawn** debe moverse, proporcionada como un **vector**.
- **Target Actor:** El actor hacia el cual se moverá el **Pawn** (opcional). El **Pawn** puede seguir a un actor en lugar de moverse a una ubicación fija.
- **Acceptance Radius:** El radio de aceptación alrededor de la **Destination**. El **Pawn** considera que ha llegado cuando está dentro de este radio.
- **Stop on Overlap:** Un valor booleano que determina si el movimiento debe detenerse cuando el **Pawn** entra en contacto con otro objeto o actor (superposición).

---

## Salidas

- **Out:** Señal de ejecución que indica que el nodo ha completado su operación.
- **On Success:** Señal de ejecución que se activa cuando el **Pawn** llega con éxito a la **Destination**.
- **On Fail:** Señal de ejecución que se activa si el movimiento falla, por ejemplo, si hay un obstáculo que impide el camino.
- **Movement Result:** Enum que devuelve el resultado del movimiento, proporcionando información sobre si el movimiento fue exitoso, fallido, o si ocurrió algún otro resultado relevante (como si el **Pawn** fue detenido por un obstáculo).