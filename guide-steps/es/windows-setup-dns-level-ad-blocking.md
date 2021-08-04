# Title #
Cómo configurar el bloqueo de anuncios a nivel del DNS en Windows

# Summary #
Con esta guía aprenderás a insertar manualmente registros DNS para ciertos tipos de hosts conocidos (por ejemplo, servidores de anuncios, rastreadores, sitios web de malware) y dirigirlos a una dirección vacía, de modo que esas solicitudes quedarán bloqueadas en tu dispositivo. A diferencia de las extensiones del navegador, el bloqueo de anuncios a nivel del DNS funciona en *cualquier* aplicación o servicio que se ejecute en tu dispositivo, no solamente en tu navegador. 

# Body #

### Configuración ###
En internet, las solicitudes de acceso a sitios web se dirigen a direcciones IP. Dado que las direcciones IP son difíciles de recordar, solemos dirigirnos a los hosts por su nombre (por ejemplo, privacyinternational.org). Por eso, y porque las direcciones IP pueden cambiar con frecuencia, cuando tu computador quiere acceder a un servidor por el nombre del host, le pregunta a un servidor DNS cuál es la dirección IP de ese nombre de host, para poder enrutar la solicitud. Normalmente, tu sistema operativo primero revisa el *archivo hosts* de tu sistema en busca de una dirección para el nombre del host. Si el nombre del host no está en el archivo, el sistema operativo le pide a un servidor DNS externo que lo resuelva.

Para configurar el bloqueo de anuncios a nivel DNS, añadiremos una lista de servidores de anuncios y rastreadores conocidos al archivo hosts y los remitiremos a una dirección vacía (`0.0.0.0`) con el fin de asegurar el bloqueo de las solicitudes. Las listas de servidores de anuncios y rastreadores son aportadas y mantenidas por la comunidad online, y puedes elegir varias listas para bloquear diferentes tipos de servicios (por ejemplo, anuncios, rastreadores, noticias falsas, redes sociales, etc.). En esta guía, te sugerimos que utilices la [lista de hosts MVPS][1] para bloquear los anuncios y los rastreadores. Recomendamos este archivo en lugar del archivo Steven Black porque el formato del archivo de hosts en Windows es diferente al de Linux y MacOS, lo que hace que el archivo Steven Black sea incompatible con Windows.

Para empezar, descarga el archivo `hosts.zip` de la página web y ábrelo en una ventana de Explorer. A continuación, selecciona el archivo que descargaste y haz clic en **Extraer todo** (Fig. 1).

![Fig. 1: Extrae el archivo hosts.zip](../../images/Windows/hosts-extract.png?raw=true)

Una vez extraídos los archivos, conviene comprobar la integridad del archivo de hosts para evitar cualquier manipulación. Para ello, abre una ventana de terminal y escribe

```CertUtil -hashfile C:\Users\YourUserName\pathToExtractedFile\HOSTS MD5```

La salida de este comando debe coincidir con la del sitio web de MVPS (5B269EA131819DEFF186B33189C7AAD6 a la fecha 11/12/2020). Si la suma de comprobación (*sumcheck*) concuerda, haz clic con el botón derecho del ratón en el archivo `mvps.bat` y selecciona **Ejecutar como administrador** (Fig. 2).

![Fig. 2: Ejecutar el instalador como administrador (*Run as administrator*)](../../images/Windows/hosts-admin.png?raw=true)

Si el instalador se ejecuta con éxito, debería aparecer un mensaje que diga **El archivo de hosts de MVPS ha sido actualizado** (Fig. 3).

![Fig. 3: Notificación de instalación: El archivo de hosts de MVPS ha sido actualizado (*The MVPS hosts file is now updated*)](../../images/Windows/hosts-bat.png?raw=true)

Para que los cambios tengan efecto, es necesario reiniciar el servicio de red o reiniciar la máquina. De ahora en adelante, tu sistema operativo bloqueará cualquier solicitud a los servidores de anuncios y los rastreadores que figuren en tu archivo hosts. Para mantener el archivo hosts actualizado, repite periódicamente los pasos de esta guía. Para información adicional sobre cómo administrar tu archivo de hosts, revisa la [documentación][2] de MVPS.

[1]: https://winhelp2002.mvps.org/hosts.htm

[2]: https://winhelp2002.mvps.org/hostswin8.htm
