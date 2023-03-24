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
