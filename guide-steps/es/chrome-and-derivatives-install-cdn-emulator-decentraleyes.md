# Title  #
Cómo instalar un emulador de CDN (red de entrega de contenidos o *content delivery network*, en inglés) en Chrome (y derivados) - Decentraleyes

# Summary #
Decentraleyes es una extensión para el navegador que sirve para emular una red local de entrega de contenido (CDN), lo que protege tu privacidad al evadir las grandes CDN (por ejemplo, Google Hosted Libraries). Con esta guía, aprenderás a instalar Decentraleyes en Chrome (y sus derivados) para evitar que las CDN rastreen tu actividad en línea.

# Body #
Las redes de distribución de contenidos (CDN) son redes geográficamente distribuidas de servidores proxy que buscan ofrecer funciones como mejorar la disponibilidad y el rendimiento de los sitios web. Aunque el objetivo es loable, también implica que los proveedores de CDN reciben metadatos vinculados con los sitios web que visitas (donde están configurados). Por ello, quizá sea conveniente sacrificar estas ventajas adicionales y prescindir de los grandes proveedores de CDN (como Google y Cloudfare) para evitar que puedan obtener datos conectados a tu navegación en la red.

Esta guía explicará cómo instalar Decentraleyes en Chrome (y sus derivados).

### Instalación ###

Al igual que todas las demás extensiones, para instalar Decentraleyes se debe visitar la [Chrome Web Store][1] y hacer clic en **Añadir a Chrome** (Fig. 1) y luego en **Agregar extensión** (Fig. 2).

![Fig. 1: Descarga Decentraleyes: Añadir a Chrome (*Add to Chrome*)](../../images/Chrome/decentraleyes-add.png?raw=true)

![Fig. 2: Agregar extensión (*Add extension*)](../../images/Chrome/decentraleyes-prompt.png?raw=true)

![Fig. 3: Notificación de instalación exitosa](../../images/Chrome/decentraleyes-notify.png?raw=true)

Una vez instalada correctamente la extensión, aparecerá una notificación en la esquina superior derecha y el ícono de Decentraleyes aparecerá en el menú de extensiones de la barra de herramientas (Fig. 3). Para anclar el ícono a la barra de herramientas, haz clic en el menú de extensiones y luego en la chincheta junto al ícono de Decentraleyes. Cuando visites un sitio web, Decentraleyes bloqueará automáticamente las conexiones a las CDN de terceros e inyectará los activos localmente; para comprobarlo haz clic en el ícono (Fig. 4).

![Fig. 4: Interfaz emergente de Decentraleyes: Contador de recursos inyectados localmente
(*Counter for locally injected sources*)](../../images/Chrome/decentraleyes-test.png?raw=true)

Puedes comprobar la extensión visitando la [utilidad de pruebas de Decentraleyes][2]. Si estás interesado en usos más avanzados, puedes visitar la [página de documentación oficial][3].

[1]: https://chrome.google.com/webstore/detail/decentraleyes/ldpochfccmkkmhdbclfhpagapcfdljkj

[2]: https://decentraleyes.org/test/

[3]: https://git.synz.io/Synzvato/decentraleyes/-/wikis/
