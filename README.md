# Laboratorio-1-Robotica-Industrial
## 1. Solucion Planteada
A continuacion se muestra la solucion planteada, la cual consiste en:

Primero la creacion del modelo 3d en inventor del tablero o Pastel adornado con las 5 primeras letras de los nombres de los integrantes (Sebastian y Andres) junto a una decoracion de un sombrero de paja. Segundo, el modelo de la herramienta a usar en el flanche del robot, la cual debe sostener fijamente un marcador en la punta y construirse posteriormetne usando impresion 3D y tubos de PVC. Seguidamente se procedio a implementar los modelos de la herramienta y del pastel en Robot studio para la creacion del Tooldata de la herramienta y el Workobject sobre el cual se trazaran las trayectorias que permitan dibujar las letras y la decoracion del pastel.

Habiendo hecho lo anterior, se ubican los objetivos sobre los cuales se quiere que pase el marcador y se trazan las trayectorias respectivas usando las funciones movl y movj en el simulador. Hechas las trayectorias y verificada la simualcion en Robotstudio se procede a cargar el codigo Rapid al Flex Pendant del robot manipulador real.

Antes de cargar el codigo se realiza la calibracion de la herramienta fisica usando el Flex Pendant y la opcion de 4 puntos para actualizar la informacion del TCP del robot, para despues actualizar la informacion del Workobject (tablero),usando 3 puntos, donde se dibujaran las letras y el sombrero de paja.
## 2. Diagrama de Flujo de Acciones de Robot
![DiagramaFlujoLab1](https://github.com/anhernadezdu/Laboratorio-1-Robotica-Industrial/assets/70985250/b701f764-fc35-47de-b7d8-55fd3c524727)

## 3. Ubicacion de Elementos en Planta
![UbicacionObjetosPlanta](https://github.com/anhernadezdu/Laboratorio-1-Robotica-Industrial/assets/70985250/89788107-3a91-473a-95f8-0f95eda5c5a5)
En el centro se puede ver el robot Manipulador IRB 140 , y ubicado diagonalmente a su izquierda se encuentra el pastel o en este caso Workobject, sobre el cual va a trabajar.


## 4. Descripcion de Funciones Utilizadas.
Para este laboratorio se urasorn las funciones **MOVL** y **MOVJ**.

- **MOVL**: Realiza un movimiento lineal de un punto u objetivo(Target) seleccionado a otro, de forma que el TCP pasa por los puntos seleccionados siguiendo el camino mas corto en el sistema coordenado usado, generalmente en coordenadas cartesianas. Usar esta funcion garantiza que todos los puntos seleccionados sean alcanzados por el TCP.
- **MOVJ**: Realiza un movimiento de un objetivo origen a otro de destino, de forma que el robot tenga que mover el menor numero de articulaciones para lograr ese objetivo. Adicionalmente, cuando existen varios puntos sobre los cuales se va a mover el TCP usando la funcion mencionada, el controlador realiza una interpolacion de los puntos seleccionados para crear la trayectoria mas facil de ralizar para el robot cumpliendo con lo dicho mas arriba. Usar esta funcion no garantiza que el TCP pase exactamente por todos lospuntos seleccionados.

## 5. Diseño de Herramienta
Para el diseño de la herramienta de trabajo se tuvieron en cuenta los siguientes requerimientos:
*La herramienta debe estar entre 30° y 60° con respesto al deflector final para evitar generar singularidades facilmente.
*Se necesita que sea modular para evitar problemas de transporte
*Dede ser de facil ensamblaje y alinación para que siempre tenga la misma disposición o almenos una muy cercana.
*Se necesita solides por si se generan fuerzas con el robot que no son deseadas se puedan soportar y la herramienta no salga afectada.
*Debe tener un lebe juego de contacto para que cuando se toque una superficie se pueda adaptar a esta.
Con estos requerimientos se penso primero en usar tubos de PVC por ser faciles de conseguir y se puede elaboar deforma modular la herremienta, asi en el mercado existen diferentes acoples que se puden usar en casos necesarios dando una versartilidad de armado sensilla. Despues de esto se consiguio un marcador borrable que seria la base de diseño, se consiguio uno de la marca Expo, el cual su diametro de donde se coge es de aproximadamente 18 mm dando a seleccionar un tubo de PVC de 3/4 in de 2.8 MP que era con el que se tenia menor juego posible pero al tenerse un diametro tan pequeno consegiir una brida no era posible por locual se opto por generar un diseño en inventor con agujeros con dimensiones apropiadas para el deflector final. Al revisar esto se encontro que la brida necesaria debia tener un tubo de acople pero el diametro exterior de este era de 26 mm dado que no se deseaba obstaculizar a los tornillos con cabeza bristol, con esto se penso en como acoplar los tubos de forma sencilla y que la construcción fuera solida obteniendo como mejor opción una rosca interna en la brida y una rosca de acople con el tubo para poder desarmar facilmente y ajustes sencillos

A continuacion se muestran los planos de la Herramienta fijadora de marcador diseñada para esta practica.
## 6. Codigo Rapid
Codigo Contenido en la Carpeta CodigoRapidLab1

## 7. Videos Simulacion e Implementacion Robot Real


https://github.com/anhernadezdu/Laboratorio-1-Robotica-Industrial/assets/70985250/6fe1bcc4-57a2-4a25-ad2e-d74ae39c21be

