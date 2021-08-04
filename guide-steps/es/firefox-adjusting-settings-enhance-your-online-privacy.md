# Title #
Cómo ajustar la configuración de Firefox para mejorar tu privacidad en línea

# Summary #
'Firefox te ofrece varios mecanismos para proteger tu privacidad. Sin embargo, algunos de ellos no vienen activados por defecto. Esta guía te mostrará cómo configurar las opciones de tu navegador Firefox para reforzar tu privacidad en línea.


# Body #

### Cómo cambiar la configuración en el menú de Firefox ###

Para cambiar la configuración básica de privacidad en Firefox, accede al menú de preferencias haciendo clic en **Edición > Preferencias** en la barra de menús, o escribiendo `about:preferences` en la barra de URL, y luego haciendo clic en **Privacidad y seguridad** (Fig. 1)


![Fig. 1: Página de configuración de privacidad de Firefox](../../images/Firefox/settings-page.png?raw=true)

#### Cómo activar el bloqueo de contenidos ####
El bloqueo de contenidos debería ser activado por defecto cuando instales Firefox. Sin embargo, si no ha sido activada por defecto, busca la configuración **Protección antirrastreo mejorada** y selecciona **Estándar** (Fig. 2). Si quieres una protección más fuerte, selecciona **Estricto**, pero ten en cuenta que esto puede interferir con la visualización de algunas páginas. 

![Fig. 2: Configuración antirrastreo de Firefox: Estándar (*Standard*) o Estricto (*Strict*)](../../images/Firefox/settings-tracking.png?raw=true)

#### Cómo activar la función "No rastrear" ####
Al navegar por la red, tu navegador puede indicarle a los sitios web que no quieres que te rastreen. ¡Ten en cuenta que no todos los sitios web lo respetan! Para protegerte mejor, consulta [nuestra guía sobre cómo instalar un bloqueador de anuncios] (firefox-ublock-origin.md). Aun así, es mejor que esta opción esté activada. Desplázate hacia abajo hasta que veas la opción **Enviar a los sitios web una señal de "No rastrear", significa que no quieres ser rastreado** y luego haz clic en **Siempre** (Fig. 3).

![Fig. 3: Configuración de "No rastrear" en Firefox: Siempre (*Always*)](../../images/Firefox/settings-dnt.png?raw=true)

#### Cómo desactivar los servicios de telemetría ###
Para mejorar sus servicios, Firefox recopila datos técnicos y de interacción que posteriormente envía a Mozilla para su tratamiento. Esto también incluye la posibilidad de instalar extensiones en tu navegador de forma remota, lo que supone un grave riesgo para la privacidad. Para desactivar los servicios de telemetría, busca la sección titulada **Recolección de datos y uso de Firefox** y asegúrate de desactivar todas las casillas (Fig. 4).

![Fig. 4: Desactivar telemetría en Firefox: Recolección de datos y uso de Firefox (*Firefox Data Collection and Use*)](../../images/Firefox/settings-telemetry.png?raw=true)

### Cómo cambiar configuraciones en la página `about:config` ###
Para configurar las opciones avanzadas de privacidad, escribe `about:config` en la barra de URL y pulsa intro. A continuación, aparecerá un mensaje de advertencia indicando que algunas configuraciones pueden afectar al rendimiento y la seguridad de Firefox (Fig. 5). Haz clic en **Aceptar el riesgo y continuar** para entrar en la página de configuración.

> **Atención**: Esta página de configuración permite acceder a funciones avanzadas que podrían interferir con el buen funcionamiento de Firefox. Asegúrate de entender lo que haces. Todos los cambios son reversibles.

![Fig. 5: Página de configuración avanzada de Firefox](../../images/Firefox/settings-config-warning.png?raw=true)

La Tabla 1 muestra algunas de las opciones avanzadas que puedes cambiar para mejorar la protección de tu privacidad en línea. Junto a cada opción se encuentra el valor que debe aplicarse, así como un breve resumen sobre los efectos de la misma. Para ajustar las opciones, escribe su nombre en la barra de búsqueda y luego haz doble clic para cambiar el valor. Al hacerlo, el valor actualizado se resalta en negrita y es guardado automáticamente (Fig. 6).

![Fig. 6: Establecer las opciones avanzadas de configuración en Firefox](../../images/Firefox/settings-config-change.png?raw=true)

| Opción                                             | Valor   | Porqué                                                                                               |
| :--                                                 | :--     | :--                                                                                               |
| `media.navigator.enabled`                           | `false` | Evita que los sitios web revisen el estado de tu micrófono y tu cámara                           |
| `privacy.firstparty.isolate`                        | `true`  | Aísla las cookies de origen del dominio para reducir el rastreo a lo largo de varios sitios web                   |
| `privacy.trackingprotection.cryptomining.enabled`   | `true`  | Impide que los sitios web ejecuten mineros de criptomonedas en tu navegador                                     |
| `privacy.trackingprotection.fingerprinting.enabled` | `true`  | Intenta disminuir tu huella digital en internet                                                         |
| `geo.enabled`                                       | `false` | Desactiva los servicios de localización, ya que pasan por los servidores de Google                               |
| `network.prefetch-next`                             | `false` | Desactiva la precarga (*prefetch*) de páginas web, porque puede suponer un riesgo para la privacidad                             |
| `network.websocket.enabled`                         | `false` | Si utilizas una VPN, el uso de WebSockets puede filtrar tu dirección IP verdadera                            |
| `dom.event.clipboardevents.enabled`                 | `false` | Impide que los sitios web reciban una notificación cuando copias, cortas o pegas algo de la página |
| `media.peerconnection.enabled`                      | `false` | Si utilizas una VPN, el uso de WebRTC puede filtrar tu dirección IP verdadera                                   |
| `dom.battery.enabled`                               | `false` | Impide que los sitios web puedan leer el nivel de tu batería                                                  |
| `browser.send_pings`                                | `false` | Impide que los sitios web rastreen tus clics en las páginas                                                |
| `browser.send_pings.require_same_host`              | `true`  | Permite el rastreo de clics si el host de envío y el de recepción coinciden                                             |
| `extensions.pocket.enabled`                         | `false` | Desactiva la integración de Pocket                                                                        |

Tabla 1: Configuraciones recomendadas para reforzar la privacidad de tu navegador
