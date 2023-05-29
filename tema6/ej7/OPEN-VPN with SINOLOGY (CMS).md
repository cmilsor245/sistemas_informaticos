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

<h1>TASK 7 - OPEN-VPN with SINOLOGY</h1>

<h4>CHRISTIAN MILLÁN SORIA</h4>

<h4>1º DAW TARDE</h4>

<hr>

<p><b>1. Explica qué es OPEN-VPN y todo lo necesario para configurar un servidor OPEN-VPN en un NAS Synology, así como las acciones a tomar en la puerta de enlace de la red local para realizar el reenvío de puertos a este servidor OPEN-VPN.</b></p>

<p>OPEN-VPN es un software de código abierto que proporciona una conexión segura y privada a través de una red pública, utilizando el protocolo VPN (Virtual Private Network). Permite a los usuarios acceder a recursos de red de forma remota y proteger su conexión de posibles amenazas.</p>

<p>Para configurar un servidor OPEN-VPN en un NAS Synology, es necesario realizar los siguientes pasos:</p>

<li>Asegurarse de tener un NAS Synology compatible con la funcionalidad de servidor VPN. No todos los modelos lo admiten.</li>

<li>Instalar el paquete VPN Server en el NAS Synology. Esto se puede hacer a través del centro de paquetes en la interfaz de administración del NAS.</li>

<li>Configurar los ajustes básicos del servidor VPN, como el nombre del servidor, el rango de direcciones IP para los clientes VPN, los protocolos de seguridad, etc.</li>

<li>Generar certificados y claves de seguridad para el servidor y los clientes VPN. Esto se puede hacer utilizando las herramientas integradas en el paquete VPN Server.</li>

<li>Configurar los ajustes de autenticación y cifrado según las preferencias de seguridad.</li>

<li>Abrir el puerto en el enrutador (gateway) para permitir el acceso externo al servidor OPEN-VPN en el NAS Synology. Esto se conoce como reenvío de puertos (port forwarding).</li>

<li>Configurar las reglas de reenvío de puertos en el enrutador para redirigir el tráfico entrante en el puerto seleccionado hacia la dirección IP interna del NAS Synology.</li>

<li>Verificar que el servidor OPEN-VPN esté funcionando correctamente y realizar las pruebas necesarias para conectarse a él de forma remota.</li>

<p><b>2. Exporta el archivo de configuración de OpenVPN al cliente de OpenVPN para Windows y prueba la conexión y el acceso a las carpetas compartidas del NAS.</b></p>

<p>He utilizado el simulador que aparece en el PDF de la práctica para realizar esta tarea.</p>

<p>Al entrar en <a href="https://demo.synology.com/es-es/dsm">este enlace</a> elegí la opción "Pruebe DSM 7.2", el cual es un simulador preparado para poder realizar esta tarea.</p>

<p>Una vez dentro de la máquina (tarda en cargar un poco), me encuentro con el escritorio del NAS en el que trabajaré.</p>

<img src="img/1.png">