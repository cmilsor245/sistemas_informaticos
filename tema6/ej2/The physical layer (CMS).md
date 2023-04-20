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

<p><b>3. Las redes actuales (Escribe una breve explicación sobre los siguientes conceptos)...</b></p>

<li><b>1000BASE-T: </b>Se refiere a un estándar de Ethernet que utiliza cable de par trenzado para transmitir datos a una velocidad de 1Gbps.</li>

<li><b>¿Qué es la fibra óptica? Cuenta algo sobre los conectores LC y SC: </b>La fibra óptica es un medio de transmisión que utiliza cables de fibra óptica para transmitir datos mediante pulsos de luz. Los conectores LC y SC son tipos de conectores de fibra óptica utilizados para conectar cables de fibra óptica a dispositivos de red.</li>

<li><b>Conector RJ45 y el estándar EIA/TIA 568-B: </b>El conector RJ45 es un tipo de conector utilizado en Ethernet y otros tipos de redes de área local. El estándar EIA/TIA 568-B es un conjunto de especificaciones para la instalación de cables de red.</li>

<li><b>Conector SFP: </b>Se trata de un módulo óptico que permite la conexión de dispositivos de red como switches, routers y otros equipos de red que utilizan fibra óptica para transmitir datos. Los conectores SFP son pequeños y modulares, lo que permite una fácil instalación y reemplazo en los dispositivos de red.</li>

<p><b>4. Nuevas tecnologías en conexiones Ethernet: RJ45 CAT 6a, RJ45 CAT 7 y SFP+RJ45. ¿Qué son cada una de ellas? Busca información sobre estos conectores y explica las tasas de velocidad máxima y la distancia máxima admitida.</b></p>

<p>RJ45 es un tipo de conector que se utiliza comúnmente para conectar dispositivos de red, como computadoras y routers, a una red Ethernet. El RJ45 CAT 6a es una versión mejorada del conector RJ45 estándar y admite velocidades de hasta 10 Gbps a distancias de hasta 100 metros. El RJ45 CAT 7 es otra versión mejorada del conector RJ45 que admite velocidades de hasta 10 Gbps a distancias de hasta 100 metros, pero también está diseñado para reducir la interferencia electromagnética. El SFP+RJ45 es un conector que se utiliza con transceptores SFP+ y admite velocidades de hasta 10 Gbps a distancias de hasta 30 metros.</p>

<p>Es importante recordar que estos conectores tienen una distancia máxima recomendada para su uso. Sin embargo, esta distancia puede variar dependiendo de la calidad del cable que se esté utilizando y si hay alguna interferencia electromagnética. También es importante tener en cuenta que la velocidad máxima de la red no solo depende del tipo de conector que se esté utilizando, sino también de otros factores en la red, como la capacidad de los dispositivos y la cantidad de tráfico que se esté transmitiendo.</p>

<p><b>5. ¿Qué es IEEE 802.11x? Recuerda... siempre se aprecia una explicación breve pero completa.</b></p>

<p>IEEE 802.11x es un conjunto de estándares para redes inalámbricas, también conocidas como Wi-Fi. Estos estándares se utilizan para establecer una comunicación inalámbrica entre dispositivos en una red, permitiendo que los dispositivos se conecten entre sí sin cables. IEEE 802.11x establece normas para la frecuencia de operación, los modos de transmisión, los métodos de seguridad y los requisitos de rendimiento de las redes inalámbricas.</p>

<p><b>6. Busca el hardware de red necesario para disfrutar de una red de 10Gbps en casa. Considera que en casa tienes 3 hosts: un ordenador de sobremesa, un portátil y un NAS de Qnap donde almacenas toda tu información crítica (fotos personales e informes y trabajos técnicos...) Da una lista con los precios de estos componentes de hardware y cables necesarios.</b></p>

<li>Un switch de red compatible con 10 Gbps, como el <a href="https://www.amazon.es/Netgear-XS508M-100EUS-gestionable-10-Gigabit-Multi-Gigabit/dp/B07554MF44?th=1">NETGEAR 8-Port 10G Multi-Gigabit Ethernet Unmanaged Switch</a> (precio aproximado: 350€).</li>

<li>Tarjeta de red de 10 Gbps para el ordenador de sobremesa y el portátil, como la tarjeta de red <a href="https://www.asus.com/networking-iot-servers/wired-networking/all-series/xg-c100c/">ASUS XG-C100C</a> (precio aproximado: 100€ cada una).</li>

<li>Adaptador de red de 10 Gbps para el NAS de Qnap, como el adaptador de red <a href="https://www.qnap.com/en/product/qxg-10g1t">QNAP QXG-10G1T</a> (precio aproximado: 80€).</li>

<li><a href="https://www.amazon.es/SEBSON-Ethernet-apantallado-Conector-Ordenador/dp/B07N2XV5RD/ref=sr_1_8?keywords=cable%2Bcat%2B7%2B10gbps&qid=1681993533&sr=8-8&th=1">Cable de red CAT 6a o CAT 7</a> para conectar los dispositivos al switch (precio aproximado: 20€ por cable).</li>