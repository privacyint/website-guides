# Title #
Cómo instalar un cambiador de agente de usuario en Chrome (y derivados) - Random User Agent

# Summary #
Esta guía te mostrará cómo instalar la extensión Random User Agent en Chrome (y derivados) a fin de cambiar periódicamente el agente de usuario de tu navegador, lo que dificulta que los rastreadores obtengan tu huella digital en internet.

# Body #
Cuando accedes a un sitio web, tu navegador envía una cadena llamada *agente de usuario* que recoge el nombre de tu navegador, el sistema operativo y otros metadatos técnicos de tu dispositivo. Desafortunadamente, los rastreadores suelen abusar de estos metadatos para crear una *huella digital* de tu sistema e identificarte con precisión en toda la web. Para limitar la capacidad de obtener tu huella digital, puedes instalar un conmutador de agente de usuario para cambiar periódicamente el agente de usuario de tu navegador y así dificultar que seas identificado con precisión.

> **Atención**: Usar un conmutador de agente puede hacer que algunas páginas no se puedan visualizar o se visualicen con errores. Para evitar este comportamiento, mostramos cómo desactivar la extensión en estos casos.

### Instalación ###
Al igual que todas las demás extensiones, para instalar Random User Agent se debe visitar la [Chrome Web Store][1] y hacer clic en **Añadir a Chrome** (Fig. 1) y luego en **Agregar extensión** (Fig. 2).

![Fig. 1: Descargar Random User Agent: Añadir a Chrome (*Add to Chrome*)](../../images/Chrome/agent-add.png?raw=true)

![Fig. 2: Agregar User Agent a Chrome: Agregar extensión (*Add extension*)](../../images/Chrome/agent-prompt.png?raw=true)

Una vez instalada correctamente la extensión, verás una notificación en la esquina superior derecha y el ícono de Random User Agent aparecerá en la barra de herramientas (Fig. 3).

![Fig. 3: Notificación de instalación exitosa](../../images/Chrome/agent-notify.png?raw=true)

Para comprobar el agente de usuario asignado actualmente, haz clic en el ícono (Fig. 4). Si llegas a una página que no funciona cuando tienes activado Random User Agent, puedes desactivar la extensión para ese dominio haciendo clic en **Enabled on this domain** (activado para este dominio) o pausar el conmutador temporalmente, haciendo clic en **Pause Switcher** (pausar conmutador).

![Fig. 4: Interfaz emergente de Random User Agent: *Enabled on this domain* (activado en este dominio), *Pause Switcher* (pausar conmutador)](../../images/Chrome/agent-test.png?raw=true)

Por defecto, Random User Agent ha sido configurado para cambiar el agente de usuario cada 10 minutos, aunque se puede configurar en la página de *general settings* (configuraciones generales) (Fig. 5).

![Fig. 5: Página de configuraciones de Random User Agent: *Time (in minutes) to automatically update the user agent* (Tiempo (en minutos) para actualizar automáticamente el agente de usuario)](../../images/Chrome/agent-settings.png?raw=true)

[1]: https://chrome.google.com/webstore/detail/random-user-agent/einpaelgookohagofgnnkcfjbkkgepnp
