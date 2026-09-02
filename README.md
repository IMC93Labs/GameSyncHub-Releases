# Game Sync Hub

Official releases, updates and user support for **Game Sync Hub**.  
Versiones oficiales, actualizaciones y soporte para **Game Sync Hub**.

[English](#english) · [Español](#espanol)

**Latest stable release / Última versión estable:** [v1.0.15](https://github.com/IMC93Labs/GameSyncHub-Releases/releases/tag/v1.0.15) · [All releases / Todas las versiones](https://github.com/IMC93Labs/GameSyncHub-Releases/releases)

---

<a id="english"></a>
## English

### What is Game Sync Hub?

Game Sync Hub is a portable Windows application for organizing local PC games, protecting and recovering save data, synchronizing selected information through Google Drive, and providing a controller-friendly Console Mode for TV/couch use.

It combines a desktop game library with local-first save protection, multi-PC recovery, automatic artwork/metadata enrichment, controller support, play statistics and optional integrations such as Anti-UAC launch rules and MSI Afterburner/RTSS performance-overlay control.

### Latest release — v1.0.15

- **Save and cloud reliability hardening:** upload/download recovery now survives interrupted operations while preserving verified local and remote states.
- **Durable recovery state:** journaled operations, monotonic terminal states, state reconciliation and compare-and-swap protection prevent stale background work from overwriting newer valid state.
- **Safer multi-PC synchronization:** stronger Current / Previous integrity and conflict handling avoid overwriting independent progress.
- **Recovered Google Drive performance:** remote inventory reuse and larger resumable-upload chunks restore practical synchronization times while keeping safety checks intact.
- **Controller hotplug stability:** fixed a native HID/WinMM failure path that could terminate Game Sync Hub when Bluetooth controllers disconnected or reconnected.
- **Console Mode polish:** refined library, settings, game editor, multimedia selection, motion, interface sounds, haptics and startup experience.
- **General stability and lifecycle improvements** across long-running controller, cloud and UI workflows.

➡️ **[See the v1.0.15 release summary](docs/releases/v1.0.15.md)**

### Highlights

- **Local-first save protection and recovery** with verified Current / Previous history and manual emergency-recovery material.
- **Google Drive synchronization** for protected saves and the information required to recover the Game Sync Hub library on another PC.
- **Interruption-safe synchronization:** resumable uploads, isolated download staging, durable journals and recovery checks are designed to avoid promoting partial save data.
- **Offline-friendly operation:** a healthy local save remains usable when Internet or Drive is temporarily unavailable, with pending work resumed later.
- **Multi-PC safety** with divergence detection and conflict preservation instead of blindly choosing the newest timestamp.
- **New-PC/reinstall recovery:** recover the library from Drive and re-link games to their new executable and save locations.
- **Automatic metadata and artwork enrichment** for covers, horizontal backgrounds, icons and descriptions when available.
- **Console Mode** with dynamic artwork, configurable background motion, favourites/recent games and controller-first navigation.
- **Controller support** for Xbox/XInput, PlayStation, Nintendo and generic HID devices, including adaptive glyphs and reconnection handling.
- **Play statistics** including play time, sessions and last-played information.
- **Transfer Center** showing real synchronization work such as pending, verifying, uploading and recovery operations.
- **Optional Anti-UAC rules** for trusted games and launchers without globally disabling Windows UAC.
- **Optional MSI Afterburner + RTSS integration** for controller-based OSD toggling when the direct RTSS path is available.
- **Built-in updater** using stable GitHub Releases, SHA-256 verification, safe-state checks, startup handshake and rollback protection.
- **Portable single-file distribution:** the public Windows build is delivered as one self-contained `GameSyncHub.exe`.

➡️ **[See the complete feature guide](docs/guides/features.md)**

### Visual overview

![Game Sync Hub overview](docs/media/01-overview.png)

Game Sync Hub can identify a game, retrieve available artwork/metadata, protect its save folder and present it in both the desktop library and Console Mode.

![Add Red Dead Redemption 2 and protect saves](docs/media/add-rdr2-full-flow.gif)

![Console Mode with several real games](docs/media/console-multi-game.gif)

- [Complete feature guide](docs/guides/features.md)
- [Visual documentation](docs/guides/visual-documentation.md)
- [Quick-start visual guide](docs/media/quick-start-en.png)
- [Recovery visual guide](docs/media/recovery-en.png)

### Downloads and updates

Official builds are published only in **[Releases](https://github.com/IMC93Labs/GameSyncHub-Releases/releases)**. The current stable build is always available from **[Latest release](https://github.com/IMC93Labs/GameSyncHub-Releases/releases/latest)**.

Each stable release includes the portable `GameSyncHub.exe`, a SHA-256 checksum file and the updater manifest. Game Sync Hub verifies downloaded updates before replacement and keeps rollback protection if a new build cannot complete its startup confirmation.

> Do not download Game Sync Hub from unofficial mirrors unless an official release explicitly points to them.

### Save-safety design

Game Sync Hub is designed so that Google Drive adds redundancy rather than becoming a requirement for playing. Save preparation is local-first, remote uploads use immutable packages, downloads are staged and verified before promotion, and ambiguous multi-PC states are preserved for conflict resolution instead of being overwritten automatically.

The software is extensively tested, but no software can guarantee zero risk. **Keep an independent backup of important saves.**

### Important notice

Game Sync Hub is a **personal hobby project** developed in my free time. I am **not a professional software developer**.

Development is carried out with **AI-assisted vibe coding**. AI tools are used to generate, modify, review, document and test parts of the project.

The application is provided **as-is, without guarantees**, and you choose to use it at your own risk. Because Game Sync Hub can work with save files, local folders, NTFS links and cloud synchronization, an independent backup of important data is strongly recommended.

Read the full **[Disclaimer](DISCLAIMER.md)** before using the application.

### Support

- **Bug:** [Report a bug](https://github.com/IMC93Labs/GameSyncHub-Releases/issues/new/choose)
- **Feature request:** [Request an improvement](https://github.com/IMC93Labs/GameSyncHub-Releases/issues/new/choose)
- **Questions and general help:** [Discussions](https://github.com/IMC93Labs/GameSyncHub-Releases/discussions)
- **Security issue:** read the [Security policy](SECURITY.md) and report it privately when possible.

Support is provided on a best-effort basis. This is a hobby project and there is no guaranteed response time or service level.

### Source code

This repository is used for **official releases, public documentation and user support**. The source code is not published here.

See also: **[Support](SUPPORT.md)** · **[Security](SECURITY.md)** · **[Contributing](CONTRIBUTING.md)** · **[Disclaimer](DISCLAIMER.md)**

---

<a id="espanol"></a>
## Español

### ¿Qué es Game Sync Hub?

Game Sync Hub es una aplicación portable para Windows destinada a organizar juegos locales de PC, proteger y recuperar partidas guardadas, sincronizar mediante Google Drive la información necesaria y ofrecer un Modo consola manejable con mando desde el televisor o el sofá.

Combina una biblioteca de escritorio con protección local-first de saves, recuperación multi-PC, enriquecimiento automático de arte/metadatos, soporte de mandos, estadísticas de juego e integraciones opcionales como reglas Anti-UAC y control del overlay de MSI Afterburner/RTSS.

### Última versión — v1.0.15

- **Refuerzo de seguridad de partidas y nube:** la recuperación de subidas y descargas soporta interrupciones manteniendo estados locales y remotos verificados.
- **Estado durable de recuperación:** journal de operaciones, estados terminales monotónicos, reconciliación y protección compare-and-swap evitan que tareas antiguas sobrescriban estados válidos más recientes.
- **Sincronización multi-PC más segura:** mayor integridad de Current / Previous y protección de conflictos sin sobrescribir progresos independientes.
- **Rendimiento de Google Drive recuperado:** reutilización del inventario remoto y chunks resumibles mayores reducen tiempos sin eliminar comprobaciones de seguridad.
- **Estabilidad de hotplug del mando:** corregida una ruta nativa HID/WinMM que podía cerrar Game Sync Hub al desconectar o reconectar mandos Bluetooth.
- **Pulido del Modo consola:** mejoras en biblioteca, ajustes, editor de juegos, selección multimedia, movimiento, sonidos, háptica y experiencia de arranque.
- **Mejoras generales de estabilidad y ciclo de vida** en flujos prolongados de mandos, nube e interfaz.

➡️ **[Ver el resumen de v1.0.15](docs/releases/v1.0.15.md#español)**

### Funciones destacadas

- **Protección y recuperación local-first de partidas** con historial Current / Previous verificado y material de recuperación manual para emergencias.
- **Sincronización mediante Google Drive** de partidas protegidas y de la información necesaria para recuperar la biblioteca en otro PC.
- **Sincronización resistente a interrupciones:** subidas reanudables, staging aislado de descarga, journals durables y verificaciones antes de promocionar datos.
- **Funcionamiento sin conexión:** una partida local sana sigue siendo utilizable si Internet o Drive fallan temporalmente y el trabajo pendiente se reanuda después.
- **Seguridad multi-PC** con detección de divergencias y conservación de conflictos en lugar de elegir simplemente la fecha más reciente.
- **Recuperación tras reinstalar o cambiar de PC:** recuperación de biblioteca y re-vinculación de ejecutables y rutas de saves.
- **Enriquecimiento automático de metadatos e imágenes** con portada, fondo horizontal, icono y descripción cuando están disponibles.
- **Modo consola** con arte dinámico, movimiento de fondo configurable, favoritos/recientes y navegación orientada a mando.
- **Soporte de mandos** Xbox/XInput, PlayStation, Nintendo y HID genéricos, con iconos adaptados y gestión de reconexión.
- **Estadísticas de juego** con tiempo jugado, sesiones y última vez jugado.
- **Centro de transferencias** con actividad real de sincronización: pendientes, verificación, subida y recuperación.
- **Reglas Anti-UAC opcionales** para juegos y launchers de confianza sin desactivar globalmente el UAC de Windows.
- **Integración opcional MSI Afterburner + RTSS** para alternar el OSD con mando cuando está disponible la ruta directa de RTSS.
- **Actualizador integrado** basado en Releases estables de GitHub, verificación SHA-256, comprobación de estado seguro, confirmación de arranque y rollback.
- **Distribución portable en un solo archivo:** la compilación pública de Windows se entrega como `GameSyncHub.exe` self-contained.

➡️ **[Ver la guía completa de funciones](docs/guides/features.md#español)**

### Vista visual

![Vista general de Game Sync Hub](docs/media/01-overview.png)

Game Sync Hub puede identificar un juego, obtener el arte/metadatos disponibles, proteger su carpeta de partidas y mostrarlo tanto en la biblioteca de escritorio como en Modo consola.

![Añadir Red Dead Redemption 2 y proteger partidas](docs/media/add-rdr2-full-flow.gif)

![Modo consola con varios juegos reales](docs/media/console-multi-game.gif)

- [Guía completa de funciones](docs/guides/features.md#español)
- [Documentación visual](docs/guides/visual-documentation.md)
- [Guía visual rápida](docs/media/quick-start-es.png)
- [Guía visual de recuperación](docs/media/recovery-es.png)

### Descargas y actualizaciones

Las compilaciones oficiales se publican únicamente en **[Releases](https://github.com/IMC93Labs/GameSyncHub-Releases/releases)**. La compilación estable actual siempre está disponible en **[Latest release](https://github.com/IMC93Labs/GameSyncHub-Releases/releases/latest)**.

Cada versión estable incluye el `GameSyncHub.exe` portable, su archivo de comprobación SHA-256 y el manifiesto del actualizador. Game Sync Hub verifica las actualizaciones descargadas antes de sustituir el ejecutable y mantiene protección de rollback si la nueva compilación no completa su confirmación de arranque.

> No descargues Game Sync Hub desde mirrors o páginas no oficiales salvo que una Release oficial indique expresamente lo contrario.

### Diseño de seguridad de las partidas

Game Sync Hub está diseñado para que Google Drive añada redundancia en lugar de convertirse en un requisito para jugar. La preparación de saves es local-first, las subidas remotas usan paquetes inmutables, las descargas se preparan y verifican antes de promocionarse y los estados multi-PC ambiguos se conservan para resolverlos en lugar de sobrescribirse automáticamente.

El software se somete a pruebas intensivas, pero ningún software puede garantizar riesgo cero. **Mantén una copia de seguridad independiente de las partidas importantes.**

### Aviso importante

Game Sync Hub es un **proyecto personal creado como hobby** y desarrollado en mi tiempo libre. **No soy desarrollador de software profesional.**

El desarrollo se realiza mediante **vibe coding asistido por inteligencia artificial**. Se utilizan herramientas de IA para generar, modificar, revisar, documentar y probar partes del proyecto.

La aplicación se proporciona **tal cual, sin garantías**, y cada usuario decide utilizarla bajo su propia responsabilidad. Como Game Sync Hub puede trabajar con partidas guardadas, carpetas locales, enlaces NTFS y sincronización en la nube, se recomienda encarecidamente mantener una copia de seguridad independiente de los datos importantes.

Lee el **[Aviso y responsabilidad](DISCLAIMER.md)** completo antes de utilizar la aplicación.

### Soporte

- **Error:** [Reportar un problema](https://github.com/IMC93Labs/GameSyncHub-Releases/issues/new/choose)
- **Mejora:** [Solicitar una mejora](https://github.com/IMC93Labs/GameSyncHub-Releases/issues/new/choose)
- **Preguntas y ayuda general:** [Discussions](https://github.com/IMC93Labs/GameSyncHub-Releases/discussions)
- **Problema de seguridad:** consulta la [Política de seguridad](SECURITY.md) y repórtalo de forma privada cuando sea posible.

El soporte se presta en la medida de lo posible. Es un proyecto realizado como hobby y no existe un tiempo de respuesta ni un nivel de servicio garantizados.

### Código fuente

Este repositorio se utiliza para **versiones oficiales, documentación pública y soporte a usuarios**. El código fuente no se publica aquí.

Consulta también: **[Soporte](SUPPORT.md)** · **[Seguridad](SECURITY.md)** · **[Contribuir](CONTRIBUTING.md)** · **[Aviso y responsabilidad](DISCLAIMER.md)**

---

**Game Sync Hub — IMC93Labs**