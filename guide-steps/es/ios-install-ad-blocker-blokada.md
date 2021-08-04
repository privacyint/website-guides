# Title #
Cómo instalar un bloqueador de anuncios en iOS - Blokada

# Summary #
Blokada es una aplicación móvil gratuita y de código abierto que utiliza servidores DNS para bloquear anuncios y rastreadores en tu dispositivo con el objetivo de mejorar tu privacidad. Con esta guía aprenderás a instalar Blokada en tu dispositivo iOS.

# Body #
Blokada es un bloqueador de anuncios que actúa como una VPN para bloquear el tráfico no deseado con base en hostnames (urls). Esto evita que las aplicaciones ejecutándose en tu dispositivo carguen anuncios y datos maliciosos.

### Instalación ###

Para instalar Blokada, visita su página en la [App Store de Apple][1], haz clic en **Obtener** (Fig. 1), y confirma haciendo clic en **Instalar** (Fig. 2).

![Fig. 1: Página de Blokada en la App Store](../../images/ios/blockada-app-store.jpg?raw=true)

![Fig. 2: Instalar Blokada](../../images/ios/blockada-install.png?raw=true)

### Configuración ###
Una vez instalado Blokada, puedes abrir la aplicación pulsando el ícono. Por defecto, Blokada está desactivada. Para activarla, haz clic en el botón grande (Fig. 3).

![Fig. 3: Activar Blokada](../../images/ios/blockada-enable.jpg?raw=true)

Blokada solicitará permiso para configurar una VPN, lo cual es necesario para bloquear los anuncios. Blokada dice que configura una VPN dividida, que sólo enruta el tráfico en el puerto 53, que se utiliza para comunicarse con resolutores DNS externos. Esto significa que todo el tráfico (por ejemplo, si intentas abrir privacyinternational.org en tu navegador) se dirigirá a través de Blokada y se cotejará con un archivo DNS local. Si el hostname está en la lista (por ejemplo, un servidor de anuncios), el recurso no cargará. Esto impde que se acceda y, además, muestren anuncios y rastreadores maliciosos.

Blokada afirma que **no** vigila ni filtra el tráfico habitual de la red. Como es de código abierto y el código es visible públicamente, esta afirmación puede verificarse periódicamente.

Haz clic en **Permitir** para continuar con la configuración (Fig. 4). 

![Fig. 4: Pmitir que Blokada establezca una VPN](../../images/ios/blockada-vpn.jpg?raw=true)

Blokada ya debería estar activada. Para seleccionar una lista de bloqueo (*blocklist*), haz clic en la ficha **Advanced** (Avanzado) (Fig. 5), y luego selecciona una (o más) de la lista. Tal vez quieras utilizar la misma lista que sugerimos en nuestras guías DNS, la lista de hosts de Steven Black o [Energized](https://github.com/EnergizedProtection/block), que también se actualiza con frecuencia. 

![Fig. 5: Selecciona una lista de bloqueo](../../images/ios/blockada-lists.jpg?raw=true)

Después de seleccionar la lista de bloqueo, tu dispositivo debería empezar a bloquear los anuncios de inmediato. Para más información sobre Blokada y sus funciones avanzadas, puedes visitar su [sitio web oficial][2].

[1]: https://apps.apple.com/us/app/blokada/id1508341781

[2]: https://blokada.org/
