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

<h1>TASK 4 - IPV4 ADDRESSING EXERCISES</h1>

<h4>CHRISTIAN MILLÁN SORIA</h4>

<h4>1º DAW TARDE</h4>

<hr>

<p><b>1. Enumera las clases de direcciones IPv4 existentes. Describe el rango del primer byte para cada una de ellas.</b></p>

<img src="img/1.png">

<p>Hay 5 clases de direcciones IPv4:</p>

<li>Clase A: El primer byte de una dirección de Clase A está en el rango de 1 a 126. Los primeros bits (el primer bit es siempre 0) representan el número de red y los últimos tres bytes representan el número de host.</li>

<br>

<li>Clase B: El primer byte de una dirección de Clase B está en el rango de 128 a 191. Los primeros dos bytes representan el número de red y los últimos dos bytes representan el número de host.</li>

<br>

<li>Clase C: El primer byte de una dirección de Clase C está en el rango de 192 a 223. Los primeros tres bytes representan el número de red y el último byte representa el número de host.</li>

<br>

<li>Clase D: El primer byte de una dirección de Clase D está en el rango de 224 a 239. Las direcciones de Clase D se utilizan para multicast.</li>

<br>

<li>Clase E: El primer byte de una dirección de Clase E está en el rango de 240 a 255. Las direcciones de Clase E se reservan para uso experimental y no se utilizan para la comunicación en Internet.</li>

<p>Los rangos de direcciones IPv4 son cada vez más escasos, debido al aumento constante del número de dispositivos conectados a Internet. Se está trabajando en una transición a IPv6, que utiliza direcciones más largas y ofrece un rango de direcciones mucho mayor.</p>

<p><b>2. Determina el rango de direcciones privadas existentes.</b></p>

<p>Las direcciones IP privadas son direcciones que no están asignadas a dispositivos conectados directamente a Internet, sino que se utilizan en redes privadas, como redes domésticas o de oficina. Estas direcciones se definen en el RFC 1918 de la IETF y se pueden utilizar en cualquier red local sin necesidad de registro o pago a una autoridad central. Los rangos de direcciones IP privadas son los siguientes:</p>

<li>10.0.0.0 a 10.255.255.255 (rango de Clase A)</li>

<li>172.16.0.0 a 172.31.255.255 (rango de Clase B)</li>

<li>192.168.0.0 a 192.168.255.255 (rango de Clase C)</li>

<p>Las direcciones IP privadas no son enrutables a través de Internet y que deben utilizarse en combinación con un enrutador NAT (traducción de direcciones de red) para permitir que los dispositivos en la red privada se comuniquen con dispositivos en Internet.</p>

<p><b>3. </b></p>