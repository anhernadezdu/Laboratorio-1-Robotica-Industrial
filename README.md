# Laboratorio-1-Robotica-Industrial
## 1. Solucion Planteada
A continuacion se muestra la solucion planteada, la cual consiste en: Primero la creacion del modelo 3d en inventor de las 5 primeras letras de los nombres de los integrantes (Sebastian y Andres) junto a una decoracion de un sombrero de paja. Segundo el modelo de la herramienta a usar, hecha con tubos de pvc para el cuerpo y PLC para la base de la misma. Seguidamente se procedio a implementar el modelo de la herramienta en Robot studio para la creacion de
## 2. Diagrama de Flujo de Acciones de Robot


## 3. Descripcion de Funciones Utilizadas.
Para este laboratorio se urasorn las funciones **MOVL** y **MOVJ**.

- **MOVL**: Realiza un movimiento lineal de un punto u objetivo(Target) seleccionado a otro, de forma que el TCP pasa por los puntos seleccionados siguiendo el camino mas corto en el sistema coordenado usado, generalmente en coordenadas cartesianas. Usar esta funcion garantiza que todos los puntos seleccionados sean alcanzados por el TCP.
- **MOVJ**: Realiza un movimiento de un objetivo origen a otro de destino, de forma que el robot tenga que mover el menor numero de articulaciones para lograr ese objetivo. Adicionalmente, cuando existen varios puntos sobre los cuales se va a mover el TCP usando la funcion mencionada, el controlador realiza una interpolacion de los puntos seleccionados para crear la trayectoria mas facil de ralizar para el robot cumpliendo con lo dicho mas arriba. Usar esta funcion no garantiza que el TCP pase exactamente por todos lospuntos seleccionados.
- 
## 4. Diseño de Herramienta

## 5.Codigo Rapid
