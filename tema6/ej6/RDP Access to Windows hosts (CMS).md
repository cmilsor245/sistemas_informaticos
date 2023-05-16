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

<h1>TASK 6 - RDP ACCESS TO WINDOWS HOSTS</h1>

<h4>CHRISTIAN MILLÁN SORIA</h4>

<h4>1º DAW TARDE</h4>

<hr>

<p><b>1. Servidor remoto. ¿Qué es necesario configurar en el host de Windows al que queremos acceder?</b></p>

<p>Para configurar el acceso remoto en un host de Windows al que deseas acceder, debes seguir los siguientes pasos:</p>

<li>1. Verifica la edición de Windows: Asegúrate de que el host de Windows tenga una edición compatible con el acceso remoto. En general, las ediciones profesionales, como Windows 10 Pro o Windows Server, admiten la función de Escritorio remoto, mientras que las ediciones domésticas, como Windows 10 Home, pueden tener limitaciones o requerir soluciones alternativas.</li>

<li>2. Habilita la función de Escritorio remoto: Para habilitar el acceso remoto, haz lo siguiente:</li>

<li>Haz clic derecho en el menú "Inicio" y selecciona "Sistema".</li>

<li>En la ventana de Configuración del sistema, selecciona "Configuración avanzada del sistema".</li>

<li>En la pestaña "Remoto", marca la opción "Permitir que los usuarios se conecten de forma remota a este equipo".</li>

<li>Opcionalmente, puedes hacer clic en "Seleccionar usuarios" para especificar qué usuarios o grupos tienen permiso para acceder de forma remota.</li>

<li>3. Configura el enrutamiento y acceso remoto (opcional): Si deseas permitir el acceso remoto desde fuera de tu red local, es posible que necesites configurar el enrutamiento y acceso remoto en tu enrutador o firewall para redirigir los puertos necesarios al host de Windows.</li>

<li>4. Configura la red y la seguridad: Asegúrate de que el host de Windows esté correctamente conectado a la red y tenga una dirección IP válida. Además, considera configurar las medidas de seguridad apropiadas, como cortafuegos y software antivirus, para proteger el host de accesos no autorizados.</li>

<p>Una vez que hayas completado estos pasos, podrás acceder al host de Windows de forma remota utilizando una herramienta de acceso remoto como el Escritorio remoto de Windows, ingresando la dirección IP o el nombre de host del equipo al que deseas conectarte.</p>