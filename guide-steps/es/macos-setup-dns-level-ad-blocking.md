# Title #
Cómo configurar el bloqueo de anuncios a nivel del DNS en macOS

# Summary #
Con esta guía aprenderás a insertar manualmente registros DNS para ciertos tipos de hosts conocidos (por ejemplo, servidores de anuncios, rastreadores, sitios web de malware) y dirigirlos a una dirección vacía, de modo que esas solicitudes queden bloqueadas en tu dispositivo. A diferencia de las extensiones del navegador, el bloqueo de anuncios a nivel del DNS funciona en *cualquier* aplicación o servicio que se ejecute en tu dispositivo, no solamente en tu navegador. 

# Body #

### Configuración ###
En internet, las solicitudes de acceso a sitios web se dirigen a direcciones IP. Dado que las direcciones IP son difíciles de recordar, solemos dirigirnos a los hosts por su nombre (por ejemplo, privacyinternational.org). Por eso, y porque las direcciones IP pueden cambiar con frecuencia, cuando tu computador quiere acceder a un servidor por el nombre del host, le pregunta a un servidor DNS cuál es la dirección IP de ese nombre del host, para poder enrutar la solicitud. Normalmente, tu sistema operativo primero revisa el *archivo hosts* de tu sistema en busca de una dirección para el nombre del host. Si el nombre del host no está en el archivo, el sistema operativo le pide a un servidor DNS externo que lo resuelva.

Para configurar el bloqueo de anuncios a nivel DNS, añadiremos al archivo hosts una lista de servidores de anuncios y rastreadores conocidos y los remitiremos a una dirección vacía (`0.0.0.0`) con el fin de asegurar el bloqueo de las solicitudes. Las listas de servidores de anuncios y rastreadores son aportadas y mantenidas por la comunidad online, y puedes elegir varias listas para bloquear diferentes tipos de servicios (por ejemplo, anuncios, rastreadores, noticias falsas, redes sociales, etc.). En esta guía, te sugerimos que utilices la [lista unificada de hosts][1] de Steven Black para bloquear anuncios y rastreadores, puesto que se actualiza con frecuencia.

Empieza por abrir una ventana del Finder y ve a la carpeta **Aplicaciones > Utilidades** y abre la aplicación **Terminal**. A continuación, escribe el siguiente comando en la ventana:

```bash wget https://raw.githubusercontent.com/StevenBlack/hosts/master/hosts -O hosts ```

y luego pulsa intro. La lista de Steven Black se descargará en el directorio actual. Aunque es poco probable, es importante examinar el contenido del archivo, para asegurarse de que no contiene entradas maliciosas (por ejemplo, paypal.com apuntando a una dirección de phishing que roba la información de tu tarjeta de crédito). Para ello, puedes utilizar `grep`. En la misma ventana de terminal, escribe el siguiente comando:

```bash grep -E '^(\s*)[1-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\s*.*\..*' hosts ```

y luego pulsa intro. Si hay alguna salida (por ejemplo: el comando devuelve texto), es posible que el archivo haya sido manipulado. Bórralo y elige otro archivo hosts, por ejemplo, [de esta lista](https://github.com/EnergizedProtection/block#formats).  Cuando tengas la URL de esta nueva lista (por ejemplo, la URL de la lista blu es https://block.energized.pro/blu/formats/hosts.txt), sustituye la URL de StevenBlack en el comando anterior por esta nueva URL. Repite el segundo comando para asegurarte de que este archivo no haya sido manipulado.

Si el archivo hosts está bien, puedes moverlo a la ubicación correcta con el comando que aparace abajo. En los macOS suele ser `/etc/hosts`, pero asegúrate de consultar el manual de distribuciones. Por favor, ten en cuenta que si en el pasado ya has modificado tu archivo de hosts con entradas personalizadas, debes fusionar manualmente ambos archivos (abre ambos archivos en tu editor de texto y copia y pega). En la misma ventana de terminal, escribe el siguiente comando:

```bash sudo mv hosts /etc ```

Pulsa intro y se te solicitará que ingreses tu contraseña. Escribe tu contraseña (no aparecerá mientras tecleas, eso es lo previsto) y vuelve a pulsar intro. Para que los cambios tengan efecto, es necesario reiniciar el servicio de red (consulta las instrucciones sobre cómo hacerlo en el manual de distribuciones) o reiniciar la máquina.

De aquí en adelante, tu sistema operativo bloqueará cualquier solicitud a los servidores de anuncios y los rastreadores que figuren en tu archivo hosts. Para mantener el archivo hosts actualizado, repite periódicamente los pasos de esta guía.

[1]: https://raw.githubusercontent.com/StevenBlack/hosts/master/hosts
