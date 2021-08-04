# Title #
Cómo instalar un cambiador de agente de usuario en Firefox - Random User Agent

# Summary #
Esta guía te mostrará cómo instalar la extensión Random User Agent en Firefox a fin de cambiar periódicamente el agente de usuario de tu navegador, lo que dificulta que los rastreadores obtengan tu huella digital en internet.

# Body #
Cuando accedes a un sitio web, tu navegador envía una cadena llamada *agente de usuario* que recoge el nombre de tu navegador, el sistema operativo y otros metadatos técnicos de tu dispositivo. Desafortunadamente, los rastreadores suelen abusar de estos metadatos para crear una *huella digital* de tu sistema e identificarte con precisión en toda la web. Para limitar la capacidad de obtener tu huella digital, puedes instalar un conmutador de agente de usuario para cambiar periódicamente el agente de usuario de tu navegador y así dificultar que seas identificado con precisión.

> **Atención**: Usar un conmutador de agente puede hacer que algunas páginas no se puedan visualizar o se visualicen con errores. Para evitar este comportamiento, mostramos cómo desactivar la extensión en estos casos.

### Instalación ###
Al igual que cualquier otra extensión, para instalar Random User Agent debes visitar la [página de extensiones de Mozilla Firefox][1] y hacer clic en **Agregar a Firefox** (Fig. 1) y, a continuación, hacer clic en **Añadir** (Fig. 2).

![Fig. 1: Descargar Random User Agent: Agregar a Firefox (*Add to Firefox*)](../../images/Firefox/agent-add.png?raw=true)

![Fig. 2: Añadir Random User Agent a Firefox: Añadir (*Add*)](../../images/Firefox/agent-prompt.png?raw=true)

Una vez instalada correctamente la extensión, verás una notificación de instalación exitosa en la esquina superior derecha y el ícono de Random User Agent aparecerá en la barra de herramientas (Fig. 3). 

![Fig. 3: Notificación de instalación exitosa](../../images/Firefox/agent-notify.png?raw=true)

Para comprobar el agente de usuario asignado actualmente, haz clic en el ícono (Fig. 4). Si llegas a una página que no funciona cuando tienes activado Random User Agent, puedes desactivar la extensión para ese dominio haciendo clic en **Enabled on this domain** (activado para este dominio) o pausar el conmutador temporalmente, haciendo clic en **Pause Switcher** (pausar conmutador).

![Fig. 4: Interfaz emergente de Random User Agent: *Enabled on this domain* (activado en este dominio), *Pause Switcher* (pausar conmutador)](../../images/Firefox/agent-test.png?raw=true)

Por defecto, Random User Agent ha sido configurado para cambiar el agente de usuario cada 10 minutos, aunque se puede configurar en la página de *general settings* (configuraciones generales) (Fig. 5).

![Fig. 5: Página de configuraciones de Random User Agent: *Time (in minutes) to automatically update the user agent* (Tiempo (en minutos) para actualizar automáticamente el agente de usuario)](../../images/Firefox/agent-settings.png?raw=true)

[1]: https://addons.mozilla.org/en-US/firefox/addon/random_user_agent/
