# Animación por Ordenador - Universidad de Granada
En este repositorio se encuentran las prácticas relacionadas con la asignatura Animación por Ordenador impartida en el Grado de Ingeniería Informática de la Universidad de Granada. La realización de las prácticas se ha llevado a cabo con el software de creación de gráficos y animaciones Autodesk 3DS Max.

## Práctica 1 - Introducción a la animación por claves
El objetivo de esta práctica es establecer uan toma de contacto con el proceso de animación por claves con la herramienta Autodesk 3DS Max. Para lograrlo, la práctica consiste en crear varias escenas sencillas sobre las que se plantean una serie de ejercicios de animación por claves.

### Escena 1 - Control de peso
La primera escena consiste en dos esferas P1 (roja) y P2 (verde) que interactúan con dos cajas C1 (azul) y C2 (amarilla) respectivamente. En el primer caso, P1 debe chocar con C1 y rebotar sin que la caja se mueva. Por otro lado, P2 debe chocar con C2 y empujar a la caja, es decir, deben moverse juntos.

![image](https://user-images.githubusercontent.com/72798314/227632990-3c42515c-e551-4d0d-ab8d-2171a4790342.png)

### Escena 2 - Materiales
En esta escena se pretenden simular dos materiales distintos. Hay dos esferas P1 (verde) y P2 (morada) que representan una pelota de goma y una bola de bolos respectivamente. Para lograr el efecto de simular la caída se ha optado por modificar la velocidad de caída y cuánto rebotan las esferas. P1 al ser de goma caerá más lento y rebotará más veces que P2. Es importante destacar que no se ha utilizado un sistema de físicas para la animación. A continuación se muestra la escena y las claves para utilizadas para animar cada una de las esferas en el eje Z (altura).

![image](https://user-images.githubusercontent.com/72798314/227633737-6ab42842-3ad0-4b5f-8519-39f967db2e4f.png)

![image](https://user-images.githubusercontent.com/72798314/227634351-b45d1d11-24b0-4038-9342-b5417575aafa.png)

### Escena 3 - Péndulo
La tercera y última escena pretende simular el movimiento de un péndulo que está formado por un brazo que sostiene un contrapeso, en este caso una esfera. La dificultad de este ejercicio reside en que hay que animar dos objetos y uno depende de otro (la esfera depende del movimiento del brazo). Para resolver este problema es necesario utilizar un modelo jerárquico en el que la esfera es un nodo hijo del brazo. De esta manera, al rotar el brazo también lo hará la esfera. A continuación se muestra la escena con las claves utilizadas para animar el péndulo.

![image](https://user-images.githubusercontent.com/72798314/227635534-269295ee-a55e-4307-b8cd-9c73cd390f23.png)

![image](https://user-images.githubusercontent.com/72798314/227636249-109c30f5-0968-459c-bbd3-973a5a6bddad.png)

## Práctica 2 - Uso de curvas
El objetivo de esta segunda práctica consiste en trabajar con el uso de curvas de función para controlar las animaciones. Se pretende realizar varios ejercicios aplicando la configuración de dichas curvas. También se introduce el concepto de capa, es decir, en vez de crear un archivo por cada animación todas se crean en el mismo archivo y se dividen en capas entre las que podemos cambiar. Por este motivo, a partir de la práctica 2 en adelante solo habrá un archivo de 3DS Max.

### Escena 1 - Cubos desplazandose
La primera escena sonsite en cuatro cubos que se desplazan desde un punto A hasta un punto B. Cada una de los cubos tiene una curva de movimiento diferente asociada (lineal, acelerado, decelerado y acelerado-decelerado). Se necesitan dos fotogramas clave, uno cuando el cubo está en el punto A y otro cuando está en el punto B. Para cambiar las velocidades de la animación se modifican las curvas de movimiento. A continuación se muestra la configuración de la escena con las claves utilizadas.

![image](https://user-images.githubusercontent.com/72798314/227638205-f4456cb8-cb8b-4dd7-8a7c-e80ee1be0c2d.png)

![image](https://user-images.githubusercontent.com/72798314/227638302-165f21ea-e500-4a58-8428-61fa91f8cb69.png)

### Escena 2 - Salto de coche
La segunda escena consiste en animar un coche que salta por una rampa. Este debe empezar parado y realizar los siguientes pasos:
1. Arrancar
2. Acelerar
3. Subir rampa
4. Saltar
5. Aterrizar
6. Frenar
7. Detenerse

Para comenzar, se ha modelado un coche mediante un modelo jerárquico. Está formado por dos cubos de distintas dimensiones para la carrocería y cuatro cilindros para las ruedas. Todas las piezas están conectadas como nodos hijo a cubo inferior de la carrocería. Este logra que centro de coordenadas del objeto esté lo más centrado posible, haciendo más facil colocarlo en la escena.
El siguiente paso es animar el movimiento del coche. Debido a la complejidad de la animación se ha decidido separarla en partes que se animan por separado. El punto más delicado de la animación es lograr que el coche se monte en la rampa si que la traspase o flote. Por este motivo se han añadido un par de claves en este punto para una animación más realista. A continuación, se muestra la escena ya las claves utilizadas (traslación en X, Z y rotación en X).

![image](https://user-images.githubusercontent.com/72798314/227641115-30890850-330e-4b16-865a-0a0240051881.png)

![image](https://user-images.githubusercontent.com/72798314/227641464-6eadb6a6-4626-4ca1-b861-7351f321773d.png)

### Escena 3 - Pelota botando
La tercera escena consiste en una esfera que bota sobre una mesa varias veces y después cae al suelo. La altura de cada bote debe ser la mitad del anterior, es decir, si en el primer bote la pelota alcanza una altura de 100, el segundo alcanzará 50, 25 así sucesivamente hasta que se caiga de la mesa. Para esta animación se ha modelado una mesa mediante un modelo jerárquico utilizando cubos de varias dimensiones para las patas y la tabla. Esta animación solo tiene claves en de traslación en los ejes X (desplazamiento lateral) y Z (desplazamiento vertical). A continuación se muestra la escena y las claves utilizadas.

![image](https://user-images.githubusercontent.com/72798314/227642355-d308a7a6-5b6f-406e-9029-827910cd9d01.png)

![image](https://user-images.githubusercontent.com/72798314/227642487-33118f5e-d369-409c-bd10-53be4777d179.png)

### Escena 4 - Montacargas
La cuarta y última escena de esta práctica consiste en aplicar uno de los principios de la animación, en concreto Overlap y Follow-through. Para ello se diseña un montacargas que consiste en un brazo formado por varias articulaciones atadas a una base que se mueve. El objetivo de este ejercicio consiste en simular como las distintas secciones del brazo se mueven a distintas velocidades. Para crear el montacargas se ha utilizado un modelo jerárquico en el que la base es el nodo padre y cada una de las articulaciones es un nodo hijo del anterior. Para animar la base solo son necesarios dos claves, la de inicio y la de destino. Pero a cada articulación es necesario añadirle un cierto grado de rotación para lograr ese efecto de Overlap y Follow-through. A continuación se muestra la escena y las claves utilizadas (traslación lineal en X para la base y rotaciones en el eje Y.

![image](https://user-images.githubusercontent.com/72798314/227643310-9a58488e-b2f4-418b-a136-a3ab8909176c.png)

![image](https://user-images.githubusercontent.com/72798314/227643516-0acdf54b-2a05-47f1-a059-bd692f563667.png)

## Práctica 3 - Interacción entre objetos, trayectorias y timing
El objetivo de esta práctica consiste en poner a prueba todos los conocimientos adquiridos en las dos prácticas anteriores. Para ello, solo se presenta un único ejercicio que trata de componer una escena con dos plataformas de salto, un balancín y dos esferas. Las esferas saltarán entre el trampolín y su plataforma correspondiente turnándose, primero una y luego la otra. A su vez, habrá colocadas tres luces en la escena. Estás estará encima de las plataformas y el trampolín, y cambiarán de color e intensidad dependiendo si una esfera está pasando por debajo. Además, como la segunda parte de la animación es lo mismo que la primera pero reproducido a la inversa se debe automatizar el proceso para que se repita en bucle. Finalmente se añade una cámara que orbita a la escena.

### Puesta en escena
El primer paso es modelar todos los elementos necesarios y colocarlos en su posición inicial en la escena. Las plataformas están construidas con un modelo jerárquico formado por dos cilindros siendo el inferior el nodo padre. El trampolín también está construido con un modelo jerárquico formado por un prisma triangular colocado sobre un costado (nodo padre) y una prisma rectagular muy alargado a modo de tabla. A continuación, se muestra una ilustración de la escena.

![image](https://user-images.githubusercontent.com/72798314/230965387-44461ed0-01b6-4903-9c80-ea19c5202f73.png)

### Fotogramas clave
Para poder animar el movimiento de las esferas y el trampolín es necesario crear claves. Este proceso se debe hacer de manera simultánea para sincronizar de manera perfecta la caida de las esferas con el balanceo del trampolín. Las claves de una esfera son las misma que la otra pero a la inversa, es decir, cuando una sube la otra baja. Hasta este momento solo hay creadas claves para la mitad de la animación, para automatizar la segunda mitad en el menú "Param Curve Out-of-Range Types" elegimos el modo "Ping Pong". Las siguientes ilustraciones muestran las claves para las esferas (traslación en X y Z) y el trampolín (rotación en Z) respectivamente.

![image](https://user-images.githubusercontent.com/72798314/230966665-9274ec63-2c77-462a-9f78-d5af0f0819d1.png)

![image](https://user-images.githubusercontent.com/72798314/230966831-0b3af6af-fc89-4fec-926e-f7a9042b33b7.png)

### Luces en la escena
El siguiente paso es añadir tres luces, dos sobre las plataformas y una sobre el trampolín. Estas luces son de tipo "Free Light" y están configuradas para que tengan su intensidad máxima y color blanco cuando haya una esfera pasando por debajo y su intensidad mínima y color rojo cuando no hayan esferas pasando. En la siguiente ilustración se muestra la composición de la escena con las luces añadidas.

![image](https://user-images.githubusercontent.com/72798314/230967789-aa8b1f9d-f218-4a1e-b70c-30ad0cd075c1.png)

Para lograr dichos efectos de luz es necesario añadir determinados fotogramas claves para la intesidad y el color. También se ha automatizado el proceso con el método mencionado en el paso anterior. A continuación, se muestras ilustraciones que muestran las claves de la intensidad y color respectivamente para las tres luces.

![image](https://user-images.githubusercontent.com/72798314/230968424-ecbc3a14-ef00-4cfe-9ad4-7b2c594b1a34.png)

![image](https://user-images.githubusercontent.com/72798314/230968509-f25da43c-08db-4b66-bca7-bc0797c01388.png)

### Movimiento de la cámara
El último paso es crear una cámara que orbite a la escena. Para ello, se añade una cámara de tipo "Target" y se configurar su posición y a donde apunta. Para hacer que orbite se crea un "Helper", se pone a la cámara como nodo hijo y se añaden las claves necesarias para que rote el "Helper" arrastrando la cámara consigo (rotación en Z). También se ha añadido una cuarta luz que acompaña a la cámara para alumbrar la escena (nodo hijo), sino fuera por esta luz la escena se vería muy oscura. Las ilustraciones siguiente muestran la disposición de la cámara y las claves empleadas para la rotación.

![image](https://user-images.githubusercontent.com/72798314/230969437-e34727b1-a211-4991-99c7-3398048b95ae.png)

![image](https://user-images.githubusercontent.com/72798314/230969524-c75358fb-4517-424f-bb3f-7077dc42af6b.png)

![render](https://user-images.githubusercontent.com/72798314/230969794-b9d26eb1-4a76-4bdb-a82a-cfd10f09abf4.jpg)

## Práctica 4 - Animación con restricciones
Esta práctica tiene como ejercicio una única escena en la que se utilizarán todas las restricciones de animación que ofrece 3DS Max (path, look at, link o position). Además, debe haber una c´mara que siga el recorrido por la escena.

### Modelado
Esta etapa se centra en el diseño y construcción de los objetos que habrá en la escena para su posterior animación. Los dos principales elementos para modelar son una espada y un coche.
La espada se ha construido mediante un modelo jerárquico utilizando cilindros y conos. En la siguiente ilustración se muestra el resultado final.

![image](https://user-images.githubusercontent.com/72798314/233962981-550517dd-bbd8-45ed-8346-9f4e24ee7131.png)

El modelo del coche se ha mejorado con respecto a la práctica 2. Para ello, se han utilizado "Compound Objects" para recrear un modelado más realista. Este tipo de objetos permiten operaciones geométricas como la unión, intersección, resta... El modelo del ocche consiste en un modelo jerárquico donde el chasis es el nodo padre y todos los demás elementos son nodos hijo. La siguiente ilustración muestra el resultado final.

![image](https://user-images.githubusercontent.com/72798314/233963401-a47ed3a6-4773-45e8-bbd5-b7cad05effe8.png)

### Animación: cambio de mano
La espada comienza ligada a una esfera M1 que la sostiene y se mueve con esta. Cuando se acerca a M2 (otra esfera), la espada se desprende de M1 y salta hasta M2 para ligarse a esta. Finalmente, M2 se aleja con la espada. Para realizar este movimiento se ha utilizado la restricción Link Constraint. Inicialmente, la espada tiene la restricción ligada a M1, cuando salta se enlaza a World y cuando termina el salto se enlaza a M2. Las únicas claves que son necesarias para el movimiento de la espada son las del salto.

### Animación: subida en la grúa
M2, que sostiene la espada, comienza a moverse hacia la grúa, cuando está cerca, la espada vuelve a saltar hacia la grúa. Esto se hace como en el apartado anterior, enlazando a World, animando el salto de la espada y enlazando a la base de la grúa. En las siguientes ilustraciones se muestran la restricción de tipo Link Constraint y las claves para los saltos de la espada.

![image](https://user-images.githubusercontent.com/72798314/233964918-251bf47b-ab11-47ef-9483-ed3071a94190.png)

![image](https://user-images.githubusercontent.com/72798314/233964938-e394045b-64dc-4fa0-a371-e321e0056440.png)

### Animación: movimiento de la grúa
Para lograr que la grúa gire con las plataformas no se podría usar un modelo jerárquico porque, de ser así, las plataformas también rotaría. Para ello, es necesario utilizar la restricción Position Constraint que hace que la posición de un objeto esté fijada por otro, pero no afecta a su rotación. Primero, se modela el cilindro que sujetará las dos plataformas y se le colocará un helper en cada extremo como nodos hijo. De esta manera, se pueden utilizar ambos helpers como elementos a los que se fijará la posición de las plataformas. Finalmente, se anima mediante claves la rotación de la grúa y como la espada sigue enlazada a una de las bases, esta también rotará con la grúa.

### Animación: orientación de la espada
La espada comienza apuntando hacia arriba, pero en un determinado momento de la animación (cuando la grúa llega a su punto superior), la espada debe cambiar su orientación para apuntar al coche. Para lograr este efecto se ha ce uso de la restricción Look At Constraint que modifica la orientación de un objeto para que mire a otro.Para que la espada no esté mirando constantemente al coche se cambia su peso para que mira hacia arriva al principio y cuando toque mirarlo se le aumenta el peso. El problema que surge es que 3DS Max si no detecta ningún objeto con peso, hace que la espada apunte al origen de coordenanadas. Esto se soluciona añadiendo un helper encima de la espada que la acompaña a lo largo de todo el recorrido y se le asigna un peso.

![image](https://user-images.githubusercontent.com/72798314/233966549-f2ad68d7-9dca-4c24-b438-bad34e60f957.png)

![image](https://user-images.githubusercontent.com/72798314/233966564-0ea73ea5-addc-4a5c-8597-a7f33a51e7c2.png)

### Animación: movimiento del coche
Para lograr que el coche se mueva por la escena se utilizará la restricción Path Constraint que modifica la posición y, opcionalmente, la rotación (con la opción follow) de un objeto para que siga un camino definido por un spline. Primeramente, hay que crear el spline que es una curva definida por un conjunto de puntos. Después, se le asigna el spline a la restricción path del coche para que siga el camino y se crean las claves necesarias para que empiece a moverse en el instante que queramos.

![image](https://user-images.githubusercontent.com/72798314/233967043-401de880-55bf-4d15-9551-3ec62117aa2e.png)

![image](https://user-images.githubusercontent.com/72798314/233967083-68c0269a-7196-4597-bd3c-1fda971e6101.png)

### Cámara
El último apartado para terminar la animación es colocar una cámara que se mueva por la escena enfocando la acción principal en cada momento. Para ello, se ha utilizado una cámara de tipo Target que se mueve sobre un spline mediante la restricción Path Constraint (sin la opción follow). Para la cámara ha habido que crear varias claves para sincronizar el movimiento con la acción de la escena.

![image](https://user-images.githubusercontent.com/72798314/233967461-41ae6d6b-21ce-491c-9c6f-025411fe47f9.png)

![image](https://user-images.githubusercontent.com/72798314/233967596-a34e5b26-057d-4e88-aa0e-0d0be98d85ef.png)

