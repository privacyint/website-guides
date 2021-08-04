# Title  #
Cómo instalar un bloqueador de anuncios en Microsoft Edge - uBlock Origin

# Summary #
uBlock Origin es un bloqueador de uso general para navegadores web que por defecto bloquea anuncios, rastreadores y sitios de malware. Con esta guía aprenderás a instalar uBlock Origin en Microsoft Edge.

# Body #
uBlock Origin (que no debe confundirse con uBlock, que es un proyecto diferente) es un bloqueador de anuncios independiente y de código abierto que utiliza una lista depurada de servidores, y evita que tu navegador se conecte a estos servidores para mostrarte anuncios. 

> Nota: En el mercado hay muchos bloqueadores de anuncios y puedes ensayar alternativas. Al utilizar un bloqueador de anuncios independiente, de código abierto y gratuito, es más probable que evites usar productos con conflictos de interés, spywares o que tengan programas de "anuncios aceptables". En teoría, cualquier bloqueador de anuncios que tenga listas negras y blancas abiertas que el usuario pueda editar debería ofrecer resultados similares 

> **Atención**: A veces usar un bloqueador de anuncios puede hacer que algunas páginas no se vean correctamente o no se vean en absoluto. Para evitar este comportamiento, mostramos cómo desactivar la extensión en estos casos.

### Instalación ###
Como cualquier otra extensión, para instalar UBlock Origin se debe visitar la [tienda de complementos de Microsoft Edge][1] y hacer clic en **Obtener** (Fig. 1) y, a continuación, hacer clic en **Agregar extensión** en la ventana de diálogo (Fig. 2).

![Fig. 1: Descargar uBlock Origin: Obtener (*Get*)](../../images/Edge/ublock-add.png?raw=true)

![Fig. 2: Agregar uBlock Origin a Edge: Agregar extensión (*Add extension*)](../../images/Edge/ublock-prompt.png?raw=true)

![Fig. 3: Notificación de instalación exitosa](../../images/Edge/ublock-notify.png?raw=true)

Una vez instalada correctamente la extensión, se abrirá una página de notificación y el ícono de uBlock Origin aparecerá en el menú de la barra de herramientas (Fig. 3). Para anclar el ícono en la barra de herramientas, haz clic en el menú de extensiones y, a continuación, haz clic en la chincheta situada junto al ícono de uBlock Origin. 

Cuando visites un sitio web, uBlock Origin bloqueará automáticamente los rastreadores y anuncios maliciosos; para comprobarlo haz clic en el ícono (Fig. 4).

![Fig. 4: Interfaz emergente de uBlock Origin](../../images/Edge/ublock-test.png?raw=true)

### Listas blancas
Algunas páginas web funcionan mal o no cargan si uBlock Origin está activado. En estos casos, puedes desactivar uBlock Origin para un sitio web específico haciendo clic en el ícono y luego en el botón de encendido grande (Fig. 4). Para recargar la página, simplemente pulsas el ícono de recarga en uBlock Origin (Fig. 5) o actualizas la página en tu navegador.

Ten presente que usar Ctrl+clic desactivará uBlock Origin solo temporalmente y no total e indefinidamente para ese sitio.

![Fig. 5: Recargar la lista blanca de dominios de uBlock Origin](../../images/Edge/ublock-whitelist.png?raw=true)

uBlock Origin es una herramienta potente y altamente configurable para bloquear cualquier solicitud de la red en tu navegador. Si estás interesado en usos más avanzados, visita la [página de documentación oficial][2].

[1]: https://microsoftedge.microsoft.com/addons/detail/ublock-origin/odfafepnkmbhccpbejgmiehpchacaeak

[2]: https://github.com/gorhill/uBlock/wiki
