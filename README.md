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
