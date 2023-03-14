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

<p>Una vez dentro del panel de control, buscamos "vpc" en la barra de búsqueda y clicamos en la opción que nos llevará al menú principal para poder trabajar con las VPC.</p>

<img src="img/2.png">

<p>Entre las opciones que ofrece este panel de control, debemos elegir primero la de crear una nueva VPC.</p>

<img src="img/3.png">

<p>Nos encontramos con una serie de ajustes que podemos cambiar o dejar de forma predeterminada. Para empezar, marcamos la opción "VPC only" de la izquierda, ya que por ahora solo queremos crear una VPC básica.</p>

<p>Se le asigna un nombre ("vpc_< tusiniciales >"). Se establece el CIDR que nos pide el ejercicio y, por último, añadimos una etiqueta "AWSEvaluation" con valor "1daw" (esto es solo un ejemplo, la etiqueta puede ser cualquiera, simplemente debe ser identificable).</p>

<img src="img/4.png">

<p>Esto último lo haremos siempre que se presente la opción de añadir una nueva etiqueta para poder encontrar los elementos de forma más sencilla en caso de ser necesario.</p>

<img src="img/5.png">

<p>Hacemos clic en el botón "Create VPC" y podemos ver cómo la VPC se ha creado correctamente con los ajustes definidos.</p>

<img src="img/6.png">

<p>El siguiente paso es dirigirse al panel lateral de la izquierda para entrar en el apartado "Subnets".</p>

<img src="img/7.png">

<p>Una vez dentro, localizamos la opción "Create subnet", en la esquina superior derecha del menú. Hacemos clic en ella.</p>

<p>Se nos presenta un menú de creación similar al anterior para crear la subred nueva.</p>

<p>En el desplegable que aparece en el primer cuadro se debe seleccionar la VPC que creamos anteriormente:</p>

<img src="img/8.png">

<p>De esta forma hemos vinculado la nueva subred que vamos a crear a la VPC con la que trabajaremos en este ejercicio.</p>

<p>En el siguiente cuadro aparecen nuevos ajustes. Debemos establecer un nombre para la nueva subred (tendremos que crear dos subredes, por lo que esta primera se llamará "vpc_publica_test").</p>

<p>Es importante que la zona de disponibilidad sea "US East (N. Virginia) / ...", ya que es donde se localiza la versión de AWS que tenemos disponible con nuestro correo corporativo.</p>