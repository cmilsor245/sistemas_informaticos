<style>
  h1{
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

<h1>AWS VPC EX1</h1>

<hr>

<h2><b>Preguntas qye hemos de saber responder:</b></h2>

<p><b>Dada la IPv4 172.31.15.6/20...</b></p>

<li><b>¿A qué red pertenece? ¿Cuál es su máscara?</b></li>

<li><b>¿Cuál es el nº de hosts que puede soportar?</b></li>

<li><b>¿Cuál es la primera IP asignable?</b></li>

<li><b>¿Cuál es la dirección de broadcast?</b></li>

<li><b>¿Cuál sería la última IP asignable?</b></li>

<hr>

<p><b>3. Vamos a crear un VPC con las siguientes condiciones:</b></p>

<p><b>Se trata de montar una infraestructura para una empresa que va a tener dos subredes: una pública y otra privada. Cada una de las subredes estará dispersa en dos zonas de disponibilidad de la región para más disponibilidad y seguridad.</b></p>

<p><b>La zona pública deberá tener salida a Internet a través de una gateway propio creado ad-hoc para el VPC.</b></p>

<p><b>El rango de direcciones del VPC será el CIDR 10.0.0.0/16 y cada una de las dos subredes pública y privada tendrán los CIDR 10.0.1.0/24 y 10.0.2.0/24 respectivamente.</b></p>

<p><b>Las subredes públicas se llamarán "publica_vpc" y "privada_vpc".</b></p>

<p><b>Se creará una tabla de enrutamiento que permita salida a Internet a la subred pública, pero no a la privada.</b></p>