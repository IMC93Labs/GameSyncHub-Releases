# Game Sync Hub — Features / Funciones

[English](#english) · [Español](#español)

---

<a id="english"></a>
## English

Game Sync Hub is a Windows gaming hub focused on a controller-first Console Mode, local-first save protection and recovery across PCs.

### Game library

- Add local games from supported launchers.
- Keep stable game identity even when executable paths differ between PCs.
- Retrieve available cover art, backgrounds, icons and descriptions.
- Replace media manually when desired.
- Track play time, sessions and last-played information.
- Rebuild managed library information from Google Drive on a new PC.

### Console Mode

- Controller-first interface designed for TV/couch use.
- Optional automatic entry when a controller is detected.
- Browse the library, recent games and favourites with a gamepad.
- Dynamic artwork and background motion.
- Configurable interface sounds and haptic feedback.
- Quick Control Center available during supported game sessions.
- Console session state survives supported controller reconnect scenarios.

### Controller integration

Game Sync Hub contains a controller abstraction layer for Xbox/XInput, PlayStation, Nintendo and generic HID families. Exact behaviour depends on the device and Windows driver.

For Xbox-compatible controllers, v1.1.0 physically validates:

- Bluetooth input path.
- Xbox Wireless Adapter input path.
- Guide-button handling.
- Control Center access.
- Haptic feedback / rumble.
- Reconnection and active-session recovery.
- Controller virtualization and physical-device isolation designed to avoid double input.

The virtualization path uses a protected Controller Device Broker and HidHide integration. The application itself runs normally as the user; elevation is handled only where installation/service configuration requires it.

### Save-path protection

- Configure the folder where each game stores its saves.
- Use known save-path suggestions when available, while preserving manual selection.
- Reject unsafe overlapping save paths.
- Validate local save state before launch where protection requires it.
- Maintain verified recovery history.
- Preserve unknown/divergent local states rather than silently overwriting them.

### Local-first save/cloud behaviour

Google Drive provides redundancy and recovery, but normal play is not intended to require an online connection.

- Healthy local saves remain playable offline.
- Network or Drive interruptions can leave remote work pending without blocking the game unnecessarily.
- Local progress is protected before background upload.
- Remote work is resumable and journaled.
- Critical restore/write operations remain protected by launch/update gates.

### Multi-PC safety and recovery

- Detect divergent histories instead of relying only on timestamps.
- Avoid silently overwriting independent progress from another PC.
- Merge play sessions by stable session identity.
- Recover managed library information and save material on another PC.
- Re-link games to local executable/save paths after reinstall or migration.

### Transfer Center

The Transfer Center reflects real synchronization work such as pending, preparing, uploading, downloading, verifying and recovery operations while keeping the rest of the application usable.

### Optional RTSS integration

For users who already run MSI Afterburner + RivaTuner Statistics Server (RTSS), Game Sync Hub can toggle the existing performance OSD from a controller shortcut during supported game sessions. Game Sync Hub does not install or create the RTSS overlay itself.

### Anti-UAC support

Game Sync Hub can manage launch rules for trusted games/launchers that would otherwise request elevation each time they start. This does not disable Windows UAC globally.

### Installed distribution

Starting with **v1.1.0**, public releases use an installer:

`GameSyncHub-Setup-vX.Y.Z.exe`

Portable v1.0.x users should install v1.1.0 manually. Portable builds are no longer the public distribution method.

### Built-in updater

For installed v1.1.0+ releases, the updater:

- Reads the official stable GitHub release channel.
- Ignores drafts and prereleases.
- Requires the exact versioned Setup asset name.
- Validates the release manifest, version, size, SHA-256, SourceCommit, ProductVersion and minimum updater version.
- Does not select the legacy portable ZIP path.
- Downloads to local staging with progress and cancellation handling.
- Respects active-game, controller-lease and save/cloud safety gates before handoff.
- Closes Game Sync Hub safely and executes only the previously validated Setup.
- Allows Setup to request the installation UAC prompt; Game Sync Hub itself remains non-elevated.
- Uses a durable operation/nonce/version/commit handshake before marking an update completed.

A cancelled or failed Setup is not reported as a successful update.

### Visual documentation

- [Visual guide](visual-documentation.md)
- [Quick-start image](../media/quick-start-en.png)
- [Recovery image](../media/recovery-en.png)

---

<a id="español"></a>
## Español

Game Sync Hub es una plataforma gaming para Windows centrada en un Modo consola manejable con mando, protección local-first de partidas y recuperación entre varios PCs.

### Biblioteca de juegos

- Añadir juegos locales desde lanzadores compatibles.
- Mantener una identidad estable aunque la ruta del ejecutable cambie entre PCs.
- Obtener portadas, fondos, iconos y descripciones cuando estén disponibles.
- Sustituir multimedia manualmente.
- Registrar tiempo jugado, sesiones y última vez jugado.
- Reconstruir la información gestionada de la biblioteca desde Google Drive en otro PC.

### Modo consola

- Interfaz orientada al mando para televisión y sofá.
- Entrada automática opcional al detectar un mando.
- Navegación por biblioteca, recientes y favoritos con gamepad.
- Multimedia dinámica y movimiento de fondos.
- Sonidos de interfaz y respuesta háptica configurables.
- Centro de Control rápido durante sesiones de juego compatibles.
- Conservación de la sesión de consola en escenarios soportados de desconexión/reconexión del mando.

### Integración de mandos

Game Sync Hub dispone de una capa de abstracción para familias Xbox/XInput, PlayStation, Nintendo y HID genérico. El comportamiento exacto depende del dispositivo y del controlador de Windows.

En mandos compatibles con Xbox, v1.1.0 ha validado físicamente:

- Entrada mediante Bluetooth.
- Entrada mediante Xbox Wireless Adapter.
- Botón Guide.
- Acceso al Centro de Control.
- Vibración / rumble.
- Reconexión y recuperación de sesión activa.
- Virtualización del mando y aislamiento del dispositivo físico para evitar doble input.

La virtualización utiliza un Controller Device Broker protegido e integración con HidHide. La aplicación se ejecuta normalmente como usuario; la elevación se utiliza únicamente donde la instalación/configuración del servicio lo requiere.

### Protección de rutas de partidas

- Configurar la carpeta donde cada juego guarda sus partidas.
- Utilizar sugerencias de rutas conocidas cuando están disponibles, manteniendo selección manual.
- Rechazar rutas solapadas inseguras.
- Validar el estado local antes del lanzamiento cuando la protección lo requiere.
- Mantener historial verificado de recuperación.
- Preservar estados locales desconocidos o divergentes en lugar de sobrescribirlos silenciosamente.

### Funcionamiento Save/Cloud local-first

Google Drive aporta redundancia y recuperación, pero el juego normal no está pensado para depender de una conexión online.

- Las partidas locales sanas siguen siendo utilizables sin conexión.
- Los cortes de red o Drive pueden dejar trabajo remoto pendiente sin bloquear innecesariamente el juego.
- El progreso local se protege antes de la subida en segundo plano.
- El trabajo remoto es reanudable y queda registrado en journal.
- Las operaciones críticas de restauración/escritura mantienen sus bloqueos de seguridad.

### Seguridad multi-PC y recuperación

- Detectar historiales divergentes en vez de decidir únicamente por timestamps.
- Evitar sobrescribir silenciosamente progreso independiente de otro PC.
- Fusionar sesiones de juego por identidad estable de sesión.
- Recuperar biblioteca gestionada y material de partidas en otro PC.
- Volver a vincular juegos a sus rutas locales tras reinstalación o migración.

### Centro de transferencias

El Centro de transferencias refleja trabajo real de sincronización: pendiente, preparación, subida, descarga, verificación y recuperación, manteniendo utilizable el resto de la aplicación.

### Integración RTSS opcional

Si el usuario ya utiliza MSI Afterburner + RivaTuner Statistics Server (RTSS), Game Sync Hub puede alternar el OSD existente mediante un atajo de mando durante sesiones compatibles. Game Sync Hub no instala ni genera el overlay de RTSS.

### Soporte Anti-UAC

Game Sync Hub puede gestionar reglas de lanzamiento para juegos/launchers de confianza que de otro modo solicitarían elevación en cada inicio. Esto no desactiva globalmente el UAC de Windows.

### Distribución instalada

Desde **v1.1.0**, las versiones públicas utilizan instalador:

`GameSyncHub-Setup-vX.Y.Z.exe`

Los usuarios de v1.0.x portable deben instalar v1.1.0 manualmente. Las builds portables dejan de ser el método público de distribución.

### Actualizador integrado

En instalaciones oficiales v1.1.0+, el actualizador:

- Consulta el canal estable oficial de GitHub.
- Ignora drafts y prereleases.
- Exige el nombre exacto del Setup correspondiente a la versión.
- Valida manifiesto, versión, tamaño, SHA-256, SourceCommit, ProductVersion y versión mínima del updater.
- No selecciona el antiguo camino ZIP portable.
- Descarga a staging local con progreso y cancelación.
- Respeta juego activo, leases de mando y gates Save/Cloud antes del handoff.
- Cierra Game Sync Hub de forma segura y ejecuta únicamente el Setup ya validado.
- Permite el UAC propio del instalador; Game Sync Hub permanece sin elevar.
- Usa un handshake durable con operación/nonce/versión/commit antes de marcar la actualización como completada.

Un Setup cancelado o fallido no se informa como actualización correcta.

### Documentación visual

- [Guía visual](visual-documentation.md#español)
- [Imagen de inicio rápido](../media/quick-start-es.png)
- [Imagen de recuperación](../media/recovery-es.png)
