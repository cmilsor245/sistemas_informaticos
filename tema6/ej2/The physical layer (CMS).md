<style>
  h1, h2, h3, h4, h5, h6{
    text-align: center;
    font-weight: bold;
    border: none;
    margin-bottom: 0px;
  }

  p{
    text-align: justify;
  }

  img{
    border: 2px solid black;
  }
</style>

<h1>TASK 2 - THE PHYSICAL LAYER</h1>

<h4>CHRISTIAN MILLÁN SORIA</h4>

<hr>

<p><b>1. ¿Qué es una topología de red? Describe y utiliza imágenes para explicar la red en estrella y la red en árbol.</b></p>

<p>Una topología de red se refiere a la estructura física o lógica de una red informática.</p>

<h3>RED EN ESTRELLA</h3>

<img src="img/1.png">

<p>En la red en estrella, todos los dispositivos están conectados al nodo central (switch) a través de un cable. Este nodo central es responsable de dirigir el tráfico de la red y actúa como un punto de control para la comunicación entre los dispositivos. Si un dispositivo desea comunicarse con otro dispositivo, envía los datos al nodo central, que luego los retransmite al dispositivo de destino.</p>

<h3>RED EN ÁRBOL</h3>

<img src="img/2.png">

<p>En la red en árbol, los dispositivos se organizan en varias ramas que se extienden desde un nodo raíz. Los dispositivos se conectan a través de enlaces de red en una estructura jerárquica. Los dispositivos en los niveles superiores de la jerarquía actúan como concentradores para los dispositivos en los niveles inferiores. Si un dispositivo desea comunicarse con otro dispositivo, los datos se transmiten a través de los enlaces de red y los concentradores de nivel superior hasta que llegan al dispositivo de destino.</p>

<p>*Es importante destacar que cada tipo de topología tiene sus propias ventajas y desventajas en términos de escalabilidad, confiabilidad y complejidad de la red.</p>

<p><b>2. ¿Qué es el protocolo IEEE 802.3? ¿Qué es un marco Ethernet? Explica brevemente cada uno de los campos más importantes de un marco 802.3.</b></p>

<p>El protocolo IEEE 802.3 es un conjunto de estándares que define cómo se deben comunicar los dispositivos en una red de área local (LAN). Este protocolo especifica los detalles técnicos sobre cómo los dispositivos envían y reciben datos a través de los cables de red.</p>

<p>Antes de que un dispositivo envíe un marco Ethernet, primero se envía un preámbulo de 7 bytes. El preámbulo se utiliza para sincronizar los relojes de los dispositivos que envían y reciben el marco. Además, también se utiliza para indicar el inicio de un marco y para alertar a los dispositivos de que se avecina un marco de datos.</p>

<p>Un marco Ethernet es la unidad básica de datos que se transmite en una red Ethernet. Un marco Ethernet típicamente consta de seis campos diferentes. Estos campos son:</p>

<li>Dirección MAC de origen: identifica la dirección MAC del dispositivo que envía el marco.</li>

<li>Dirección MAC de destino: identifica la dirección MAC del dispositivo receptor del marco.</li>

<li>Tipo de protocolo: indica el tipo de protocolo utilizado para la carga útil de datos del marco.</li>

<li>Datos de la carga útil: es el contenido real que se está transmitiendo en el marco, como por ejemplo un mensaje de correo electrónico o una imagen.</li>

<li>Relleno: se utiliza para llenar el marco y garantizar que tenga una longitud mínima.</li>

<li>Campo FCS (Frame Check Sequence): contiene un valor numérico utilizado para detectar errores en la transmisión del marco.</li>

<p><b>3. </b></p>