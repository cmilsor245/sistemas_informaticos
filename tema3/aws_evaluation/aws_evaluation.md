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

  #ex{
    border: none;
  }
</style>

<h1>AWS EVALUATION</h1>

<hr>

<p><b>1. AWS Academy Cloud Foundations (Theory)</b></p>

<img src="img/modules_done.png">

<hr>

<p><b>2.a. Creación de una VPC donde instalar las instancias que vamos a usar.</b></p>

<p><b>Crear una VPC con las siguientes condiciones:</b></p>

<li><b>Se trata de montar una infraestructura para una empresa que va a tener dos subredes, una pública y otra privada. Cada una de las subredes estará dispersa en dos zonas de disponibilidad de la región para más disponibilidad y seguridad.</b></li>

<li><b>La zona pública deberá tener salida a Internet a través de un gateway propio creado para la VPC.</b></li>

<li><b>El rango de direcciones de la VPC será el CIDR 10.0.0.0/16 y cada una de las dos subredes tendrá los CIDR 10.0.1.0/24 y 10.0.2.0/24 respectivamente.</b></li>

<li><b>La subred pública se llamará "vpc_publica_test" y la privada "vpc_privada_test".</b></li>

<li><b>Se creará una tabla de enrutamiento que permita salida a Internet a la subred pública, pero no a la privada.</b></li>

<p><b>Ficha técnica:</b></p>

<li><b>Nombre VPC: vpc_< tusiniciales ></b></li>

<li><b>Subred pública: vpc_publica_test</b></li>

<li><b>Subred privada: vpc_privada_test</b></li>

<li><b>CIDR VPC: 10.0.0.0/16</b></li>

<li><b>CIDR público: 10.0.1.0/24</b></li>

<li><b>CIDR privado: 10.0.2.0/24</b></li>

<p><b>Salida a Internet (subred pública):</b></p>

<img src="img/salida_publica.png">

<p>Lo primero es iniciar el Learner Lab del entorno de AWS.</p>

<img src="img/1.png">