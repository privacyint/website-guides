# Title  #
Cómo instalar un bloqueador de anuncios en Chrome (y derivados) - uBlock Origin

# Summary #
uBlock Origin es un bloqueador de uso general para navegadores web que por defecto bloquea anuncios, rastreadores y sitios de malware. Esta guía te mostrará cómo instalar uBlock Origin en Chrome y sus derivados (Opera, Chromium, Brave...)

# Body #
uBlock Origin (que no debe confundirse con uBlock, que es un proyecto diferente) es un bloqueador de anuncios independiente y de código abierto que utiliza una lista depurada de servidores y evita que tu navegador se conecte a estos servidores y evita que tu navegador se conecte a estos servidores con el propósito mostrarte anuncios. 

> Nota: En el mercado hay muchos bloqueadores de anuncios y puedes ensayar alternativas. Al utilizar un bloqueador de anuncios independiente, de código abierto y gratuito, es más probable que evites usar productos con conflictos de interés, spywares o que tengan programas de "anuncios aceptables". En teoría, cualquier bloqueador de anuncios con listas negras y blancas abiertas que el usuario pueda editar debería ofrecer resultados similares 

> **Atención**: A veces usar un bloqueador de anuncios puede hacer que algunas páginas no se vean correctamente o no se vean en absoluto. Para evitar este comportamiento, mostramos cómo desactivar la extensión en estos casos.

### Instalación ###
Como cualquier otra extensión, para instalar uBlock Origin visita la [Chrome Web Store][1] y haz clic en **Añadir a Chrome** (Fig. 1) y luego en **Agregar extensión** (Fig. 2).

![Fig. 1: Descarga uBlock Origin: Añadir a Chrome (*Add to Chrome*)](../../images/Chrome/ublock-add.png?raw=true)

![Fig. 2: Agregar extensión (*Add extension*)](../../images/Chrome/ublock-prompt.png?raw=true)

![Fig. 3: Notificación de instalación exitosa](../../images/Chrome/ublock-notify.png?raw=true)

Una vez instalada correctamente la extensión, aparecerá una notificación en la esquina superior derecha y el ícono de uBlock Origin aparecerá en el menú de extensiones de la barra de herramientas (Fig. 3). Para anclar el ícono a la barra de herramientas, haz clic en el menú de extensiones y luego en la chincheta junto al ícono de uBlock Origin. 

Cuando visites un sitio web, uBlock Origin bloqueará automáticamente los rastreadores y anuncios maliciosos; para comprobarlo haz clic en el ícono (Fig. 4).

![Fig. 4: Interfaz emergente de uBlock Origin](../../images/Chrome/ublock-test.png?raw=true)

### Listas blancas
Algunas páginas web funcionan mal o no cargan cuando uBlock Origin está activado. En estos casos, puedes desactivar uBlock Origin para sitios web específicos haciendo clic en el ícono y luego en el botón de encendido grande (Fig. 4). Para recargar la página, simplemente pulsas el ícono de recarga en uBlock Origin (Fig. 5) o actualizas la página en tu navegador.

Ten presente que usar Ctrl+clic desactivará uBlock Origin tan solo temporalmente y no total e indefinidamente para ese sitio.

![Fig. 5: Recargar la lista blanca de dominios de uBlock Origin](../../images/Chrome/ublock-whitelist.png?raw=true)

uBlock Origin es una herramienta potente y altamente configurable para bloquear cualquier solicitud de la red en tu navegador. Si estás interesado en usos más avanzados, visita la [página de documentación oficial][2].

[1]: https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm

[2]: https://github.com/gorhill/uBlock/wiki
