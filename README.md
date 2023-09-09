# Laboratorio-1-Robotica-Industrial
## 1. Solucion Planteada
A continuacion se muestra la solucion planteada, la cual consiste en:

Primero la creacion del modelo 3d en inventor del tablero o Pastel adornado con las 5 primeras letras de los nombres de los integrantes (Sebastian y Andres) junto a una decoracion de un sombrero de paja. Segundo, el modelo de la herramienta a usar en el flanche del robot, la cual debe sostener fijamente un marcador en la punta y construirse posteriormetne usando impresion 3D y tubos de PVC. Seguidamente se procedio a implementar los modelos de la herramienta y del pastel en Robot studio para la creacion del Tooldata de la herramienta y el Workobject sobre el cual se trazaran las trayectorias que permitan dibujar las letras y la decoracion del pastel.

Habiendo hecho lo anterior, se ubican los objetivos sobre los cuales se quiere que pase el marcador y se trazan las trayectorias respectivas usando las funciones movl y movj en el simulador. Hechas las trayectorias y verificada la simualcion en Robotstudio se procede a cargar el codigo Rapid al Flex Pendant del robot manipulador real.

Antes de cargar el codigo se realiza la calibracion de la herramienta fisica usando el Flex Pendant y la opcion de 4 puntos para actualizar la informacion del TCP del robot, para despues actualizar la informacion del Workobject (tablero),usando 3 puntos, donde se dibujaran las letras y el sombrero de paja.
## 2. Diagrama de Flujo de Acciones de Robot
![DiagramaFlujoLab1](https://github.com/anhernadezdu/Laboratorio-1-Robotica-Industrial/assets/70985250/b701f764-fc35-47de-b7d8-55fd3c524727)


## 3. Descripcion de Funciones Utilizadas.
Para este laboratorio se urasorn las funciones **MOVL** y **MOVJ**.

- **MOVL**: Realiza un movimiento lineal de un punto u objetivo(Target) seleccionado a otro, de forma que el TCP pasa por los puntos seleccionados siguiendo el camino mas corto en el sistema coordenado usado, generalmente en coordenadas cartesianas. Usar esta funcion garantiza que todos los puntos seleccionados sean alcanzados por el TCP.
- **MOVJ**: Realiza un movimiento de un objetivo origen a otro de destino, de forma que el robot tenga que mover el menor numero de articulaciones para lograr ese objetivo. Adicionalmente, cuando existen varios puntos sobre los cuales se va a mover el TCP usando la funcion mencionada, el controlador realiza una interpolacion de los puntos seleccionados para crear la trayectoria mas facil de ralizar para el robot cumpliendo con lo dicho mas arriba. Usar esta funcion no garantiza que el TCP pase exactamente por todos lospuntos seleccionados.

## 4. Diseño de Herramienta
A continuacion se muestran los planos de la Herramienta fijadora de marcador diseñada para esta practica.
## 5. Codigo Rapid
Codigo Contenido en la Carpeta CodigoRapidLab1
## 6. Videos Simulacion e Implementacion Robot Real


https://github.com/anhernadezdu/Laboratorio-1-Robotica-Industrial/assets/70985250/6fe1bcc4-57a2-4a25-ad2e-d74ae39c21be

