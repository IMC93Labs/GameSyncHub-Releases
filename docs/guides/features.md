# Game Sync Hub — Features / Funciones

[English](#english) · [Español](#español)

---

<a id="english"></a>
## English

Game Sync Hub is a portable Windows application for organizing local PC games, protecting their save data and keeping selected game information synchronized through Google Drive. It also includes a controller-first console mode so the library can be used from a TV or couch setup.

### Game library and metadata

- Add local games from their executable or launcher.
- Keep each game identified independently even when paths change between PCs.
- Search public metadata candidates while adding a game.
- Retrieve and apply available **cover art, horizontal backgrounds, icons and descriptions**.
- Manually replace cover, background or icon when desired.
- Keep game-specific media so the same artwork can be restored on another PC when the library is recovered.
- Track play time, number of sessions and last-played information.

### Save-path assistance and save protection

- Configure the local folder where each game stores its saves.
- Suggest known save locations for supported/recognized games while still allowing manual selection.
- Protect the configured save location through Game Sync Hub's local save-protection system.
- Validate the save setup before launching a game.
- Keep a verified recovery history with **Current** and **Previous** states.
- Provide manual emergency recovery material in addition to the internal protected format.
- Avoid silently replacing an unknown or divergent local save with a cloud copy.

### Google Drive synchronization

- Connect a Google Drive account through the application.
- Synchronize protected save data together with the information required to recover the Game Sync Hub library.
- Preserve game identity, metadata, artwork, known portable save paths and play statistics in the cloud structure used by Game Sync Hub.
- Continue working locally when the network is unavailable and resume pending synchronization after connectivity returns.
- Show real synchronization work through the **Transfer Center**, without blocking the rest of the interface.

### Multi-PC and recovery

- Use the same Game Sync Hub library across more than one PC.
- Detect potentially divergent save histories instead of deciding solely from file timestamps.
- Keep play statistics from different PCs and merge sessions by their session identity.
- Recover the library on a new/clean PC from the information already stored in Google Drive.
- Re-link a reinstalled game to its new executable and local save path without changing its game identity.
- Recover a verified save from Drive when needed, with validation before the restored folder becomes the active game save.

### Console mode

Console mode is designed for controller use on a TV or couch setup.

- Start Game Sync Hub directly in Console Mode if desired.
- Optionally **enter Console Mode automatically when a controller is connected**.
- Navigate the game carousel, menus, backups and search without needing the mouse for normal console use.
- Use each game's real cover/logo/background when available.
- Use dynamic game backgrounds, a fallback background when artwork is missing, themes and interface scaling.
- Configure background intensity/blur and reduce animations or transparency when preferred.
- Remember the last screen and last selected game.
- Show recent games, favourites, play time, last session and save status according to the selected options.
- Optional ambient audio and notification sounds can be configured for the console experience.

### Controller support

Game Sync Hub includes an abstraction layer for different controller families:

- **Xbox / XInput**
- **PlayStation**
- **Nintendo**
- **Generic HID controllers**

The application can adapt button glyphs, choose a preferred controller, filter unwanted stick movement with a dead zone and handle controller reconnection. Exact behaviour can vary with the device and Windows driver.

### Optional performance-overlay shortcut

For users who already use **MSI Afterburner + RivaTuner Statistics Server (RTSS)**, Game Sync Hub can expose a controller shortcut for the existing performance overlay.

- During a game, the shortcut uses **Menu/Start + View/Select**.
- Game Sync Hub reuses the **Toggle On-Screen Display** hotkey configured in MSI Afterburner.
- It can detect Afterburner/RTSS and use the configured toggle key when available.
- Game Sync Hub does **not** install Afterburner or RTSS and does not create the overlay itself; those applications remain optional third-party tools.

### Optional Anti-UAC launch rules

For trusted games or launchers that normally request elevation every time they start, Game Sync Hub can configure an optional Anti-UAC launch rule.

- Rules are associated with the relevant game/launcher instead of disabling UAC globally.
- The feature is intended only for software the user already trusts.
- Removing or changing a game can invalidate/clean the corresponding rule when appropriate.

### Built-in updates

Game Sync Hub v1.0.0 includes the updater used for future stable releases published in this repository.

- Check for updates automatically in the background or manually from the application.
- Stable mode ignores draft and pre-release builds.
- Ask for confirmation before installing an update.
- Download the fixed official `GameSyncHub.exe` asset and verify its SHA-256 against the release manifest.
- Replace the application executable only when Game Sync Hub is in a safe state.
- Use a temporary updater helper, startup handshake and rollback protection if the new executable cannot start correctly.
- Updating the application does not intentionally replace the user's saves, Google Drive library data, SaveCache, junction configuration or local settings.

### Portable distribution

The public Windows build is distributed as a **single self-contained `GameSyncHub.exe`**. No mandatory installer is required.

### Visual guides

- [Visual documentation](visual-documentation-es.md)
- [Quick-start image](../media/quick-start-es.png)
- [Recovery image](../media/recovery-es.png)

---

<a id="español"></a>
## Español

Game Sync Hub es una aplicación portable para Windows pensada para organizar juegos locales de PC, proteger sus partidas guardadas y mantener sincronizada mediante Google Drive la información necesaria para recuperarlas. También incluye un Modo consola orientado a mando para utilizar la biblioteca desde un televisor o desde el sofá.

### Biblioteca de juegos y metadatos

- Añadir juegos locales a partir de su ejecutable o launcher.
- Mantener cada juego identificado de forma independiente aunque sus rutas cambien entre ordenadores.
- Buscar candidatos de metadatos públicos al añadir un juego.
- Obtener y aplicar, cuando están disponibles, **portada, fondo horizontal, icono y descripción**.
- Cambiar manualmente portada, fondo o icono si se desea.
- Conservar la multimedia del juego para poder recuperarla también al reconstruir la biblioteca en otro PC.
- Registrar tiempo jugado, número de sesiones y última vez jugado.

### Ayuda con la ruta de partidas y protección del save

- Configurar la carpeta local donde cada juego guarda sus partidas.
- Sugerir rutas conocidas para juegos reconocidos, manteniendo siempre la posibilidad de elegir una ruta manualmente.
- Proteger la ruta configurada mediante el sistema local de protección de partidas de Game Sync Hub.
- Validar el estado de la partida antes de iniciar el juego.
- Mantener historial verificado de recuperación con estados **Current** y **Previous**.
- Generar material de recuperación manual para emergencias además del formato protegido interno.
- Evitar sustituir silenciosamente una partida local desconocida o divergente por una copia de la nube.

### Sincronización con Google Drive

- Conectar una cuenta de Google Drive desde la aplicación.
- Sincronizar las partidas protegidas junto con la información necesaria para reconstruir la biblioteca de Game Sync Hub.
- Conservar identidad del juego, metadatos, multimedia, rutas portables conocidas y estadísticas de uso dentro de la estructura de Game Sync Hub en la nube.
- Seguir trabajando localmente cuando no hay conexión y reanudar los cambios pendientes cuando vuelve la red.
- Mostrar el trabajo real de sincronización mediante el **Centro de transferencias** sin bloquear el resto de la interfaz.

### Varios PCs y recuperación

- Utilizar la misma biblioteca de Game Sync Hub en más de un ordenador.
- Detectar posibles historiales divergentes de partidas sin decidir únicamente por la fecha de los archivos.
- Conservar las estadísticas de distintos PCs y fusionar las sesiones mediante su identidad de sesión.
- Recuperar la biblioteca en un PC nuevo/limpio utilizando la información ya guardada en Google Drive.
- Volver a vincular un juego reinstalado con su nuevo ejecutable y su nueva ruta local de partidas sin cambiar la identidad del juego.
- Recuperar una partida verificada desde Drive cuando sea necesario, validándola antes de convertir la carpeta restaurada en la partida activa.

### Modo consola

El Modo consola está diseñado para utilizar Game Sync Hub con mando desde un televisor o desde el sofá.

- Iniciar Game Sync Hub directamente en Modo consola si se desea.
- Opcionalmente **entrar automáticamente en Modo consola al conectar un mando**.
- Navegar por el carrusel de juegos, menús, copias y búsqueda sin necesitar el ratón durante el uso normal del modo consola.
- Utilizar portada/logo/fondo real de cada juego cuando está disponible.
- Fondos dinámicos por juego, fondo alternativo cuando falta arte, temas y escala de interfaz.
- Configurar intensidad/desenfoque del fondo y reducir animaciones o transparencias si se prefiere.
- Recordar la última pantalla y el último juego seleccionado.
- Mostrar recientes, favoritos, tiempo jugado, última sesión y estado de la partida según las opciones elegidas.
- Configurar sonido ambiente y sonidos de notificación para la experiencia de consola.

### Soporte de mandos

Game Sync Hub incluye una capa de abstracción para distintas familias de mando:

- **Xbox / XInput**
- **PlayStation**
- **Nintendo**
- **Mandos HID genéricos**

La aplicación puede adaptar los iconos de botones, elegir mando preferido, filtrar movimientos involuntarios mediante zona muerta y gestionar reconexiones. El comportamiento exacto puede variar según el dispositivo y el controlador de Windows.

### Atajo opcional para overlay de rendimiento

Para quien ya utilice **MSI Afterburner + RivaTuner Statistics Server (RTSS)**, Game Sync Hub puede ofrecer un atajo de mando para controlar el overlay de rendimiento existente.

- Durante un juego, el atajo utiliza **Menu/Start + View/Select**.
- Game Sync Hub reutiliza la tecla **Toggle On-Screen Display** configurada en MSI Afterburner.
- Puede detectar Afterburner/RTSS y utilizar la tecla configurada cuando está disponible.
- Game Sync Hub **no instala** Afterburner ni RTSS y no genera por sí mismo el overlay; siguen siendo herramientas externas opcionales.

### Reglas Anti-UAC opcionales

Para juegos o launchers de confianza que solicitan elevación cada vez que se ejecutan, Game Sync Hub permite configurar una regla Anti-UAC opcional.

- Las reglas se asocian al juego/launcher correspondiente en lugar de desactivar UAC globalmente.
- La función está pensada únicamente para programas en los que el usuario ya confía.
- Al eliminar o cambiar un juego, la regla correspondiente puede invalidarse/limpiarse cuando proceda.

### Actualizaciones integradas

Game Sync Hub v1.0.0 incluye el actualizador que se utilizará para las siguientes versiones estables publicadas en este repositorio.

- Comprobar actualizaciones automáticamente en segundo plano o manualmente desde la aplicación.
- El canal estable ignora borradores y versiones pre-release.
- Pedir confirmación antes de instalar.
- Descargar el asset oficial fijo `GameSyncHub.exe` y verificar su SHA-256 frente al manifiesto de la Release.
- Sustituir el ejecutable únicamente cuando Game Sync Hub se encuentra en un estado seguro.
- Utilizar helper temporal, confirmación de arranque y rollback si el nuevo ejecutable no puede arrancar correctamente.
- La actualización de la aplicación no está diseñada para sustituir las partidas, datos de biblioteca en Drive, SaveCache, configuración de junctions ni ajustes locales del usuario.

### Distribución portable

La versión pública para Windows se distribuye como **un único `GameSyncHub.exe` self-contained**. No necesita instalador obligatorio.

### Guías visuales

- [Documentación visual](visual-documentation-es.md)
- [Imagen de inicio rápido](../media/quick-start-es.png)
- [Imagen de recuperación](../media/recovery-es.png)
