# Title #
Cómo ajustar la configuración de Chrome para mejorar tu privacidad en línea

# Summary #
Esta guía te mostrará cómo ajustar la configuración de tu navegador Chrome a fin de reforzar tu privacidad en línea.


# Body #

> **Atención:** Chrome es un producto de Google y, como tal, incorpora muchos mecanismos que posiblemente estén compartiendo datos con Google. Uno de estos mecanismos vincula automáticamente tu navegador a tu cuenta de Google cuando inicias una sesión en cualquier servicio de Google (por ejemplo, Gmail). Para evitar que esto suceda, considera usar Firefox o una alternativa basada en Chrome (por ejemplo, Vivaldi, Opera, Brave...). Otra posibilidad es seguir las indicaciones de esta guía para desactivar algunos de estos comportamientos en las configuraciones.

### Cómo cambiar las configuraciones en el menú de Chrome ###
Para acceder a las configuraciones, haz clic en el menú de tres puntos de la parte superior derecha y pulsa **Configuración** (Fig. 1), o escribe <chrome://settings/> en la barra de direcciones URL y haz clic en Intro.

![Fig. 1: Menú de configuraciones de Chrome](../../../images/Chrome/settings-menu.png?raw=true)

#### Tú y Google ####

Chrome incluye varias funciones que buscan mejorar tu experiencia de navegación y que requieren que compartas datos con Google. Para desactivar estas opciones, ve a la página de Configuración y haz clic en **Tú y Google** > **Sincronización y servicios de Google**. Otra cosa que puedes hacer es desactivar **Autocompletar búsquedas y URLs**, **Mejorar las búsquedas y la navegación** y **Permitir el acceso a Chrome** para evitar que estos datos sean enviados a los servidores de Google (Fig. 2).

![Fig. 2: Configuraciones de sincronización y servicios: Autocompletar búsquedas y URLs (*Autocomplete searches and URLs*), Mejorar las búsquedas y la navegación (*Make searches and browsing better*), Permitir el acceso a Chrome (*Allow Chromium sign-in*) 
](../../../images/Chrome/settings-sync.png?raw=true)

#### Privacidad y seguridad ####
En la página de Configuración, haz clic en **Privacidad y seguridad**. En esta página puedes cambiar algunas de las configuraciones para protegerte de los *web trackers*.

##### Cookies y otros datos de los sitios web #####
No realizar seguimiento (DNT o *Do Not Track*) es una señal que tu navegador envía a los sitios web cuando navegas por la red para indicarles que no quieres que te rastreen. Aunque no todos los sitios web respetan esta señal, podría ser conveniente activarla. Para protección adicional, consulta nuestra [guía sobre cómo instalar un bloqueador de anuncios](chrome-ublock-origin.md). 

Para habilitar DNT, activa **Enviar solicitud de "No realizar seguimiento" con el tráfico de navegación**, y desactiva **"Precargar las páginas para acelerar la navegación y las búsquedas"**.

##### Seguridad #####
Activa **Protección estándar** en la configuración Navegación segura (puedes escoger Protección mejorada, pero ten en cuenta que esto requiere el envío de datos adicionales a Google). A continuación, haz clic en la flecha de la derecha para abrir el panel de configuraciones avanzadas. Para evitar el envío de datos adicionales a Google, desactiva **Ayudar a mejorar la seguridad en la web para todos los usuarios** (Fig. 3). 

![Fig. 3: Configuraciones de seguridad: Protección estándar (*Standard protection*), Protección mejorada (*Enhanced protection*), Ayudar a mejorar la seguridad en la web para todos los usuarios (*Help improve security on the web for everyone*)](../../../images/Chrome/settings-security.png?raw=true)

##### Configuración de los sitios #####
En la sección de permisos, puedes habilitar **Preguntar antes de acceder** para **todos** los permisos para asegurarte de que los sitios web no accedan a tu micrófono o ubicación sin que tú lo sepas. Si quieres que los sitios no puedan enviar y recibir datos después de que hayas cerrado una pestaña o ventana, desactiva **Sincronización en segundo plano** (ten en cuenta que esto puede afectar tu navegación). 

Por último, puedes desplazarte hasta el final de la página y hacer clic en **Configuración adicional de contenido**. Aquí verás una opción para desactivar los **anuncios** que Google considera son invasivos o engañosos. Aunque es una opción sencilla de activar, sugerimos que consideres un bloqueador de anuncios de terceros, como uBlock Origin o Privacy Badger, para evitar que Google sea quien decida qué anuncios son problemáticos y bloquee todos los anuncios.

![Fig. 4: Configuración de los permisos](../../../images/Chrome/settings-permissions.png?raw=true)
