# Game Sync Hub — Features / Funciones

[English](#english) · [Español](#español)

---

<a id="english"></a>
## English

Game Sync Hub is a portable Windows application for organizing local PC games, protecting their save data and keeping the information required for recovery synchronized through Google Drive. It also includes a controller-first Console Mode for TV/couch use.

### Game library and metadata

- Add local games from their executable or launcher.
- Keep each game identified independently even when local paths change between PCs.
- Search public metadata candidates while adding a game.
- Retrieve and apply available **cover art, horizontal backgrounds, icons and descriptions**.
- Manually replace cover, background or icon when desired.
- Preserve game-specific media so it can be restored on another PC.
- Track play time, sessions and last-played information.

### Save-path assistance and local protection

- Configure the local folder where each game stores its saves.
- Suggest known save locations for recognized games while still allowing manual selection.
- Detect unsafe overlapping save-path selections before changing protection.
- Protect the configured save location through Game Sync Hub's local save-protection system.
- Validate the local save state before launching a game.
- Keep verified recovery history with **Current** and **Previous** states.
- Generate manual emergency recovery material in addition to the internal protected package.
- Avoid silently replacing an unknown or divergent local save with a cloud copy.
- Preserve game identity when a protected save path has to be safely migrated on the current PC.

### Local-first behaviour

Google Drive adds redundancy, but it is not intended to become a requirement for playing.

- A healthy local protected save remains usable when Internet connectivity is unavailable.
- Drive outages, DNS failures or temporary network errors can leave synchronization pending without blocking the game.
- New local save progress remains protected first and can be uploaded when connectivity returns.
- Launch is blocked only when there is a genuine save-safety risk, such as an unresolved conflict, unsafe local protection state or critical restore/write operation.
- Permanent remote errors are stabilized or surfaced for repair instead of being retried forever.

### Google Drive synchronization

- Connect a Google Drive account through the application.
- Synchronize protected saves together with the information required to recover the Game Sync Hub library.
- Preserve game identity, metadata, artwork, portable save-path knowledge and play statistics in the managed cloud structure.
- Use canonical managed folders for each game's information, media and save data.
- Reconcile stale/missing managed Drive resource references when they can be repaired safely.
- Avoid selecting between two conflicting content-bearing resources solely by date or filename.
- Use deterministic recovery staging so retries can resume the same logical work instead of creating duplicate staging identities.
- Reuse verified unchanged manual-recovery files when possible instead of uploading an identical recovery tree again.
- Show synchronization work through the **Transfer Center**, grouped by stable game identity.

### Multi-PC and recovery

- Use the same Game Sync Hub library across more than one PC.
- Detect divergent save histories from commit/history relationships instead of deciding only from timestamps.
- Prevent two independently advanced PCs from silently overwriting each other.
- Allow a PC to progress offline and publish normally later when the remote history has not advanced.
- Keep play statistics from different PCs and merge sessions by session identity.
- Recover the library on a new/clean PC from the information already stored in Google Drive.
- Re-link a reinstalled game to its new executable and local save path without changing its game identity.
- Recover a verified save from Drive with validation before the restored data becomes active.

### Transfer Center

The Transfer Center reports the real synchronization pipeline without blocking the rest of the interface.

It can represent preparation, download, upload, verification, pending/retry states and recovery work. Operations belonging to the same `GameId` remain grouped as one logical game even when several suboperations are running.

### Console Mode

Console Mode is designed for controller use on a TV or couch setup.

- Start Game Sync Hub directly in Console Mode if desired.
- Optionally enter Console Mode automatically when a controller is connected.
- Navigate the game carousel, menus, backups and search without requiring the mouse for normal use.
- Use each game's real cover/logo/background when available.
- Use dynamic game backgrounds, fallback artwork, themes and interface scaling.
- Configure background intensity/blur and reduce animations or transparency when preferred.
- Remember the last screen and selected game.
- Show recent games, favourites, play time, last session and save status according to the selected options.
- Configure optional ambient audio and notification sounds.

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
- Game Sync Hub reuses the **Toggle On-Screen Display** hotkey configured in MSI Afterburner when available.
- Game Sync Hub does **not** install Afterburner or RTSS and does not create the overlay itself.

### Optional Anti-UAC launch rules

For trusted games or launchers that normally request elevation every time they start, Game Sync Hub can configure an optional Anti-UAC launch rule.

- Rules are associated with the relevant game/launcher instead of disabling UAC globally.
- The feature is intended only for software the user already trusts.
- Removing or changing a game can invalidate/clean the corresponding rule when appropriate.

### Built-in updates

Game Sync Hub includes a built-in updater for stable releases published in this repository.

- Check for updates automatically in the background or manually from the application.
- Stable mode ignores draft and pre-release builds.
- Ask for confirmation before installing an update.
- Download the official `GameSyncHub.exe` asset and verify its SHA-256 against the release manifest.
- Replace the running executable only when Game Sync Hub is in a genuinely critical state that must not be interrupted.
- A failed, deferred or offline cloud operation that is not actively modifying save data does not need to block updates indefinitely.
- Use a temporary updater helper, startup handshake and rollback protection if the new executable cannot start correctly.
- Updating the application does not intentionally replace saves, Google Drive library data, SaveCache, junction configuration or local settings.

### Portable distribution

The public Windows build is distributed as a **single self-contained `GameSyncHub.exe`**. No mandatory installer is required.

### Visual guides

- [Visual documentation](visual-documentation.md)
- [Quick-start image](../media/quick-start-en.png)
- [Recovery image](../media/recovery-en.png)

---

<a id="español"></a>
## Español

Game Sync Hub es una aplicación portable para Windows pensada para organizar juegos locales de PC, proteger sus partidas guardadas y mantener sincronizada mediante Google Drive la información necesaria para recuperarlas. También incluye un Modo consola orientado a mando para utilizar la biblioteca desde un televisor o desde el sofá.

### Biblioteca de juegos y metadatos

- Añadir juegos locales a partir de su ejecutable o launcher.
- Mantener cada juego identificado de forma independiente aunque sus rutas locales cambien entre ordenadores.
- Buscar candidatos de metadatos públicos al añadir un juego.
- Obtener y aplicar, cuando están disponibles, **portada, fondo horizontal, icono y descripción**.
- Cambiar manualmente portada, fondo o icono si se desea.
- Conservar la multimedia del juego para poder recuperarla en otro PC.
- Registrar tiempo jugado, sesiones y última vez jugado.

### Ayuda con la ruta de partidas y protección local

- Configurar la carpeta local donde cada juego guarda sus partidas.
- Sugerir rutas conocidas para juegos reconocidos, manteniendo la posibilidad de elegir una ruta manualmente.
- Detectar selecciones de SavePath solapadas y peligrosas antes de modificar la protección.
- Proteger la ruta configurada mediante el sistema local de protección de partidas de Game Sync Hub.
- Validar el estado local de la partida antes de iniciar el juego.
- Mantener historial verificado de recuperación con estados **Current** y **Previous**.
- Generar material de recuperación manual para emergencias además del paquete protegido interno.
- Evitar sustituir silenciosamente una partida local desconocida o divergente por una copia de la nube.
- Mantener la identidad del juego cuando la ruta protegida debe migrarse de forma segura en el PC actual.

### Funcionamiento local-first

Google Drive aporta redundancia, pero no está pensado para convertirse en un requisito para jugar.

- Una partida local protegida y sana puede seguir utilizándose cuando no hay Internet.
- Una caída de Drive, DNS o red puede dejar la sincronización pendiente sin bloquear el juego.
- El nuevo progreso local se protege primero y puede subirse cuando vuelve la conexión.
- Jugar solo se bloquea cuando existe un riesgo real para la partida, como un conflicto pendiente, protección local insegura o una restauración/escritura crítica en curso.
- Los errores remotos permanentes se estabilizan o pasan a reparación en lugar de reintentarse indefinidamente.

### Sincronización con Google Drive

- Conectar una cuenta de Google Drive desde la aplicación.
- Sincronizar las partidas protegidas junto con la información necesaria para reconstruir la biblioteca de Game Sync Hub.
- Conservar identidad del juego, metadatos, multimedia, conocimiento portable de rutas y estadísticas dentro de la estructura gestionada en la nube.
- Mantener carpetas canónicas para la información, multimedia y partidas de cada juego.
- Reconciliar referencias gestionadas de Drive obsoletas o ausentes cuando pueden repararse con seguridad.
- No elegir entre dos recursos con contenido en conflicto únicamente por fecha o nombre.
- Utilizar staging determinista para la recuperación manual, de forma que un reintento pueda reanudar el mismo trabajo lógico sin crear staging duplicado.
- Reutilizar archivos de recuperación manual idénticos ya verificados cuando sea posible, evitando volver a subir un árbol sin cambios.
- Mostrar el trabajo de sincronización mediante el **Centro de transferencias**, agrupado por la identidad estable del juego.

### Varios PCs y recuperación

- Utilizar la misma biblioteca de Game Sync Hub en más de un ordenador.
- Detectar historiales divergentes mediante la relación entre commits/historia en lugar de decidir únicamente por timestamps.
- Evitar que dos PCs que hayan avanzado de forma independiente se sobrescriban silenciosamente.
- Permitir que un PC avance offline y publique después normalmente cuando el historial remoto no haya cambiado.
- Conservar estadísticas de distintos PCs y fusionar sesiones por su identidad.
- Recuperar la biblioteca en un PC nuevo/limpio utilizando la información ya guardada en Google Drive.
- Volver a vincular un juego reinstalado con su nuevo ejecutable y SavePath sin cambiar la identidad del juego.
- Recuperar una partida verificada desde Drive validándola antes de convertirla en la partida activa.

### Centro de transferencias

El Centro de transferencias muestra el pipeline real de sincronización sin bloquear el resto de la interfaz.

Puede representar preparación, descarga, subida, verificación, pendientes/reintentos y recuperación. Las operaciones del mismo `GameId` permanecen agrupadas como un único juego lógico aunque existan varias suboperaciones.

### Modo consola

El Modo consola está diseñado para utilizar Game Sync Hub con mando desde un televisor o desde el sofá.

- Iniciar Game Sync Hub directamente en Modo consola si se desea.
- Entrar automáticamente en Modo consola al conectar un mando si se activa esa opción.
- Navegar por el carrusel, menús, copias y búsqueda sin necesitar el ratón durante el uso normal.
- Utilizar portada/logo/fondo real de cada juego cuando está disponible.
- Fondos dinámicos, arte alternativo, temas y escala de interfaz.
- Configurar intensidad/desenfoque del fondo y reducir animaciones o transparencias.
- Recordar la última pantalla y el último juego seleccionado.
- Mostrar recientes, favoritos, tiempo jugado, última sesión y estado de la partida según las opciones elegidas.
- Configurar sonido ambiente y sonidos de notificación opcionales.

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
- Game Sync Hub reutiliza la tecla **Toggle On-Screen Display** configurada en MSI Afterburner cuando está disponible.
- Game Sync Hub **no instala** Afterburner ni RTSS y no genera por sí mismo el overlay.

### Reglas Anti-UAC opcionales

Para juegos o launchers de confianza que solicitan elevación cada vez que se ejecutan, Game Sync Hub permite configurar una regla Anti-UAC opcional.

- Las reglas se asocian al juego/launcher correspondiente en lugar de desactivar UAC globalmente.
- La función está pensada únicamente para programas en los que el usuario ya confía.
- Al eliminar o cambiar un juego, la regla correspondiente puede invalidarse/limpiarse cuando proceda.

### Actualizaciones integradas

Game Sync Hub incluye un actualizador integrado para las versiones estables publicadas en este repositorio.

- Comprobar actualizaciones automáticamente en segundo plano o manualmente desde la aplicación.
- El canal estable ignora borradores y versiones pre-release.
- Pedir confirmación antes de instalar.
- Descargar el asset oficial `GameSyncHub.exe` y verificar su SHA-256 frente al manifiesto de la Release.
- Sustituir el ejecutable únicamente cuando exista una operación realmente crítica que no deba interrumpirse.
- Una operación de nube fallida, diferida u offline que no esté modificando activamente las partidas no tiene por qué bloquear indefinidamente una actualización.
- Utilizar helper temporal, confirmación de arranque y rollback si el nuevo ejecutable no puede arrancar correctamente.
- La actualización de la aplicación no está diseñada para sustituir partidas, datos de biblioteca en Drive, SaveCache, configuración de junctions ni ajustes locales.

### Distribución portable

La versión pública para Windows se distribuye como **un único `GameSyncHub.exe` self-contained**. No necesita instalador obligatorio.

### Guías visuales

- [Documentación visual](visual-documentation.md)
- [Imagen de inicio rápido](../media/quick-start-es.png)
- [Imagen de recuperación](../media/recovery-es.png)
