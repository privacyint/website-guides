# Title #
Cómo aislar tu actividad en línea - Firefox Multi-Account Containers

# Summary #
Una manera de minimizar el rastreo y mejorar tu privacidad en línea es almacenar la menor cantidad posible de cookies de navegación en tu dispositivo. Sin embargo, algunas es práctico tener cookies almacenadas en sitios web como tu cliente de correo electrónico o tu aplicación web para tomar notas, para que no tengas que iniciar una sesión cada vez que visites el sitio. Esta guía explicará cómo instalar y configurar los contenedores de Firefox Multi-Account Containers para mantener diferentes partes de tu actividad en línea aisladas entre sí, reduciendo así tu huella digital.

# Body #

### Instalación ###

Al igual que para las demás extensiones, para instalar Firefox Multi-Account Containers debes visitar la [página de extensiones de Mozilla Firefox][1] y hacer clic en **Agregar a Firefox** (Fig. 1) y, a continuación, hacer clic en **Añadir** (Fig. 2).

![Fig. 1: Descargar Firefox Multi-Account Containers: Agregar a Firefox (*Add to Firefox*)](../../images/Firefox/containers-add.png?raw=true)

![Fig. 2: Añadir Firefox Multi-Account Containers a Firefox: Añadir (*Add*)](../../images/Firefox/containers-prompt.png?raw=true)

Una vez instalada correctamente la extensión, verás una notificación de instalación exitosa en la esquina superior derecha y el ícono de Firefox Multi-Account Containers aparecerá en la barra de herramientas (Fig. 3). La primera vez que hagas clic en el ícono verás una guía para entender mejor cómo funciona la extensión (Fig. 4).

![Fig. 3: Notificación de instalación exitosa](../../images/Firefox/containers-notify.png?raw=true)

![Fig. 4: Guía de inicio de Firefox Multi-Account Containers](../../images/Firefox/containers-test.png?raw=true)

### Cómo configurar un contenedor ###

Puedes crear un contenedor para cualquier sitio web y puedes asignar un sitio web a varios contenedores. En esta sección, aprenderás a configurar un contenedor para Twitter, pero los pasos son similares para otros sitios web. Primero, crea el contenedor haciendo clic en el ícono y luego ve a **Manage containers > New container** (Gestión de contenedores > Nuevo contenedor). Escribe el nombre de tu contenedor y pulsa OK (Fig. 5).

![Fig. 5: Creación de un contenedor para Twitter: Escribe el nombre del contenedor y haz clic en "OK"](../../images/Firefox/containers-twitter-create.png?raw=true)

A continuación, navega al sitio web de Twitter, haz clic en el ícono de la barra de herramientas y luego haz clic en **Always Open This Site in...** (Abrir siempre este sitio en...) y selecciona el contenedor que acabas de crear (Fig. 6).

![Fig. 6: Abrir siempre los enlaces de Twitter en su contenedor](../../images/Firefox/containers-twitter-open.png?raw=true)

Después de completar este paso, los enlaces de Twitter se abrirán en su contenedor, lo que es constatado por la pestaña subrayada y el símbolo en la barra de direcciones (Fig. 7).

![Fig. 7: Notificación de contenedor](../../images/Firefox/containers-twitter-notification.png?raw=true)

Cuando estés navegando en otro contenedor y navegues hasta un enlace de Twitter, la extensión te ubicará automáticamente en el contenedor de Twitter. La primera vez que ocurra, te preguntará si quieres abrir el enlace en el contenedor asignado (Fig. 8); si deseas que lo haga automáticamente, pulsa el botón **Remember my decision for this site** (Recordar mi decisión para este sitio) y luego haz clic en **Open in Twitter Container** (abrir en el contenedor de Twitter).

![Fig. 8: Redireccionar siempre los enlaces al contenedor ](../../images/Firefox/containers-twitter-prompt.png?raw=true)

Para más detalles sobre cómo utilizar los contenedores multicuenta de Firefox Multi-Account, puedes consultar la [documentación oficial][2].

[1]: https://addons.mozilla.org/en-US/firefox/addon/multi-account-containers/

[2]: https://blog.mozilla.org/firefox/introducing-firefox-multi-account-containers/
