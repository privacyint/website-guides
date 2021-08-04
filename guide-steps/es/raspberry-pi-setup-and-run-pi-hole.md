# Title #
Cómo configurar y ejecutar Pi-hole en Raspberry Pi

# Summary #
Normalmente, Bloquear los anuncios y los rastreadores en tus dispositivos implica realizar tareas manuales en cada uno de ellos (por ejemplo, instalar un bloqueador de anuncios en tu navegador, otro en tu teléfono y otro en tu tableta). Esta guía te mostrará cómo instalar y configurar Pi-hole, un bloqueador de anuncios de uso general para toda la red, en una Raspberry Pi, para bloquear los anuncios en cualquier dispositivo conectado a tu red doméstica.

# Body #

## Introducción ##

Pi-hole es un bloqueador de anuncios de uso general que cubre toda la red y la protege de los anuncios y los rastreadores sin que sea necesario configurar cada uno de los dispositivos. Tiene la capacidad de bloquear anuncios en cualquier dispositivo de la red (por ejemplo, electrodomésticos inteligentes) y, a diferencia de las extensiones del navegador, Pi-hole bloquea los anuncios en cualquier tipo de software.

La configuración general funciona de la siguiente manera (Fig. 1). Instalas Pi-hole en tu servidor (en este caso, estamos usando una Raspberry Pi) y le asignas una dirección IP estática. En tu router, configuras el servidor primario de DNS a la dirección IP de Pi-hole. Cuando un dispositivo se conecta a tu red doméstica, obtiene de tu router la dirección IP de Pi-hole como su servidor DNS principal. Cuando el dispositivo busca la dirección del nombre host, contacta a Pi-hole. Si el host es un anuncio o un rastreador y está incluido en la lista en uso, la solicitud se bloquea al instante. En caso contrario, la búsqueda se realiza en un servidor upstream que tú elijas (por ejemplo, OpenDNS, Cloudflare, GoogleDNS, tu ISP).

![Fig. 1: Configuración general de Pi-hole](../../images/Pihole/overview.png?raw=true)

## Prerrequisitos ##
Para desplegar Pi-hole en tu red doméstica, asegúrate de contar con todos los siguientes elementos:

- Una Raspberry Pi con mínimo 512MB de RAM (todas las versiones de Raspberry Pi cumplen este requisito) y con Raspbian instalado.
- Una tarjeta SD con mínimo 2GB de espacio libre.
- Conexión a internet en tu Raspberry Pi. Ya sea a través de Wi-Fi (si está disponible) o a través de un cable Ethernet.
- Acceso al panel de administración de tu router[^1].

[^1]: Usualmente tendrás acceso en las redes domésticas. Consulta la documentación de tu router para ver las instrucciones y las credenciales.

## Instalación ##

> **Advertencia:** Esta guía está basada en la documentación oficial de Pi-hole, pero es posible que no esté al día. El objetivo principal de esta guía es dar una idea de qué hace Pi-hole y cómo se puede configurar, y no tanto ser una guía paso a paso precisa. Para consultar instrucciones actualizadas sobre cómo hacer la instalación y cualquier problema específico, por favor lea la [documentación oficial][3].

Si vas a utilizar una Raspberry Pi nueva, empieza por instalar Raspbian de acuerdo con la [documentación de Raspberry Pi][1]. Luego, asegúrate de instalar `git` con el siguiente comando:

```bash sudo apt install git ```

Para instalar Pi-hole, deberás clonar su repositorio git y ejecutar el script de instalación.

```bash git clone --depth 1 https://github.com/pi-hole/pi-hole.git Pi-hole cd "Pi-hole/automated install/" sudo bash basic-install.sh ```

El script te guiará por los pasos de la instalación y te pedirá indicaciones para configurar los ajustes básicos. Cualquier configuración realizada durante la instalación puede ser actualizada después. Durante el proceso, se te solicitará que selecciones un proveedor de DNS upstream (Fig. 2). Este es el servidor en el que se realizarán las búsquedas de nombres de host no bloqueados.

![Fig. 2: Selecciona DNS upstream](../../images/Pihole/dns.png?raw=true)

A continuación, se te pedirá que selecciones un par de listas de anuncios (*adlists*). Te sugerimos que dejes las dos opciones activadas, que es como viene la configuración predeterminada (Fig. 3). Más adelante, podrás añadir listas personalizadas si lo deseas.

![Fig. 3: Selección de *adlist* en Pi-hole](../../images/Pihole/adlists.png?raw=true)

Pi-hole puede bloquear anuncios en IPv4 e IPv6. Salvo que tengas una razón específica para desactivar alguno de esos protocolos, puedes dejarlos ambos activados (Fig. 4).

![Fig. 4: Selección de protocolos en Pi-hole](../../images/Pihole/protocols.png?raw=true)

También incluye una interfaz web que puedes acceder para gestionar tu instancia de Pi-hole. Si te sientes cómodo con el uso de la línea de comandos, puedes omitir la instalación de la interfaz web (y del servidor). De lo contrario, te sugerimos que la instales (Fig. 5), al igual que el servidor web correspondiente (Fig. 6).


![Fig. 5: Instalación de la interfaz web](../../images/Pihole/webinterface.png?raw=true)

![Fig. 6: Instalación del servidor web](../../images/Pihole/webserver.png?raw=true)

Puedes escoger que se elabore un registro de las consultas que responda tu Pi-hole (Fig. 7), y elegir un nivel de privacidad que determine qué tipo de registros serán almacenados (Fig. 8). Si compartes tu instancia de Pi-hole con otras personas, ten en cuenta que los registros pueden filtrar información privada (que tú podrás ver), así que elige los niveles de privacidad adecuados.

![Fig. 7: Configuración de los registros de consultas](../../images/Pihole/logs.png?raw=true)

![Fig. 8: Establece el nivel de privacidad de los registros](../../images/Pihole/privacy.png?raw=true)

Cuando finalice la instalación, recibirás un mensaje resumiendo las direcciones IP de tu Pi-hole y una contraseña de administrador generada al azar (Fig. 9). Asegúrate de guardar esto en algún lugar (ya sea con una captura de pantalla o anotada en un papel), porque necesitarás la información más adelante.

![Fig. 9: Resumen de la instalación de Pi-hole ](../../images/Pihole/summary.png?raw=true)

Haz clic en OK para concluir la instalación. Para comprobar que la instalación se realizó correctamente, abre un navegador web y ve a <http://IP_ADDRESS/admin>, donde `IP_ADDRESS` es la dirección IPv4 de tu dispositivo Pi-hole (Fig. 9). Ten presente que <http://pihole/admin> sólo funciona **después** de que configures tu dispositivo para utilizar el servidor DNS de Pi-hole. Haz clic en el botón de inicio de sesión e introduce tu contraseña (generada al azar). Ahora deberías estar en el panel de administración de Pi-hole (Fig. 10).

![Fig. 10: Panel de control de Pi-hole](../../images/Pihole/admin.png?raw=true)

## Configuración ##
Ahora que tienes instalado Pi-hole, el paso final es configurar tu red para que use Pi-hole como su servidor DNS.

Para hacer esto, el mejor método es cambiar el servidor DNS de tu router y dirgirlo a la dirección IP de Pi-hole, para garantizar que cualquier cliente que se conecte a tu red reciba a Pi-hole como su servidor DNS. Usualmente, esto requiere que accedas al panel de control del router. Allí deberías encontrar un campo para establecer los servidores DNS primario y secundario. Fija la dirección primaria a la dirección IP del Pi-hole, y reinicia cualquier conexión de red abierta que pudieras tener en tus dispositivos. Ahora, cuando te conectes a tu red doméstica, debería aparecer Pi-hole como servidor DNS.

Sin embargo, algunos routers no permiten cambiar la configuración del DNS. En este caso, puedes definir Pi-hole como tu servidor DHCP (y al hacerlo, necesitas desactivar el propio servidor DHCP de tu router). Consulta la [documentación oficial de Pi-hole][2] para saber cómo hacerlo.

[1]: https://www.raspberrypi.org/software/

[2]: https://discourse.pi-hole.net/t/how-do-i-use-pi-holes-built-in-dhcp-server-and-why-would-i-want-to/3026

[3]: https://docs.pi-hole.net/
