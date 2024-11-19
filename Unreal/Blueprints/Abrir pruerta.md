---
Tipo:
  - Apuntes
  - Ejemplos
---
## Subir puerta
![[Pasted image 20241119174704.png]]

![[Pasted image 20241119173725.png]]


"On Component Begin Overlap" conectamos "Other Actor" a un Cast to *Nombre* para comprobar si ese actor que entro es de ese tipo o no.

![[Pasted image 20241119174811.png|400 ]]
"Set Time by Event" es como un imvoke y imonke repetier (Solo si se activa el tick del loop), este estara conectado a un nodo evento que en este caso se llama "Cerrar puerta"

![[Pasted image 20241119175755.png]]
Lo primero que tenemos es un "Brench" que es meramente un If, en el cual para comprobar la condición tendremos conectado el nodo "Greater Equal" que es un "mayor que" y este estara comprobando el porcentaje.

Si es True es que ya ha llegado al 100% (1 en la variable float) cancelara el bucle con un "Clear and Invalidate Timer by Handle" el Handle es el valor retornado del nodo "Set time by event"

En el caso si es false tendremos lo siguiente.
![[Pasted image 20241119180533.png]]
Primero nuestro "Branch" cuando da false estara conectado al set de la variable float "porcentaje" y el set se establecera con un nodo "add" el cual suma la variable porcentaje actual con la variable valor sumar.

Luego seguirá con el nodo "Set Relative location" el cual tiene un nodo "Lerp" ([[Función pura|Función pura]]) que en A tendrá la altura base de nuestro objeto y en B hasta la altura que tiene que llegar, como Alpha usaremos el valor del porcentaje todo esto retornara un valor el cual representa la altura de ese porcentaje,.

## Bajar puerta

