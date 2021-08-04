# Title  #
Cómo instalar un emulador de CDN (red de entrega de contenidos o *content delivery network*, en inglés) en Firefox - Decentraleyes

# Summary #
Decentraleyes es una extensión para el navegador que se usa para emular una red local de entrega de contenido (CDN), lo que protege tu privacidad al evadir las grandes CDN (por ejemplo, Google Hosted Libraries). Con esta guía, aprenderás a instalar Decentraleyes en Firefox para evitar que las CDNs rastreen tu actividad en línea.

# Body #
Las redes de distribución de contenidos (CDN) son redes geográficamente distribuidas de servidores proxy que buscan ofrecer funciones como mejorar la disponibilidad y el rendimiento de los sitios web. Aunque el objetivo es loable, también implica que los proveedores de CDN reciben metadatos vinculados con los sitios web que visitas (donde están instalados). Sabiendo esto, quizá sea conveniente sacrificar estas ventajas adicionales y prescindir de los grandes proveedores de CDN (como Google y Cloudfare) para evitar que puedan obtener datos relacionados con tu navegación en línea.

Esta guía explicará cómo instalar Decentraleyes en Firefox para lograr este resultado.

### Instalación ###
Al igual que todas las demás extensiones, para instalar Privacy Badger debes visitar la [Mozilla Firefox Add-ons page][1] y hacer clic en **Agregar a Firefox** (Fig. 1) y, a continuación, hacer clic en **Añadir** en la ventana de diálogo (Fig. 2).

![Fig. 1: Descargar Decentraleyes: Agregar a Firefox (*Add to Firefox*)](../../images/Firefox/decentraleyes-add.png?raw=true)

![Fig. 2: Añadir Decentraleyes a Firefox: Añadir (*Add*)](../../images/Firefox/decentraleyes-prompt.png?raw=true)

![Fig. 3: Notificación de instalación exitosa](../../images/Firefox/decentraleyes-notify.png?raw=true)

Una vez instalada exitosamente la extensión, aparecerá una notificación en la esquina superior derecha y el ícono de Decentraleyes aparecerá en el menú de la barra de herramientas (Fig. 3). Cuando visites un sitio web, Decentraleyes bloqueará automáticamente las conexiones a las CDN de terceros e inyectará los activos localmente; para constatarlo haz clic en el ícono (Fig. 4).

![Fig. 4: Interfaz emergente de Decentraleyes: Contador de recursos inyectados localmente
(*Counter for locally injected sources*)](../../images/Firefox/decentraleyes-test.png?raw=true)

Puedes comprobar la extensión visitando la [utilidad de pruebas de Decentraleyes][2]. Si estás interesado en usos más avanzados, puedes visitar la [página de documentación oficial][3].


[1]: https://addons.mozilla.org/en-US/firefox/addon/decentraleyes/

[2]: https://decentraleyes.org/test/

[3]: https://git.synz.io/Synzvato/decentraleyes/-/wikis/
