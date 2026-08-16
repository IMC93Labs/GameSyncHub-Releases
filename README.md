# Game Sync Hub

Official releases, updates and user support for **Game Sync Hub**.  
Versiones oficiales, actualizaciones y soporte para **Game Sync Hub**.

[English](#english) · [Español](#espanol)

---

<a id="english"></a>
## English

### What is Game Sync Hub?

Game Sync Hub is a portable Windows application designed to organize local PC games, protect and recover their save data, synchronize selected information through Google Drive, and provide a controller-friendly console experience for TV/couch use.

It combines the normal desktop library with save protection, multi-PC recovery, automatic artwork/metadata enrichment, controller support and optional integrations such as Anti-UAC launch rules and an MSI Afterburner/RTSS performance-overlay shortcut.

### Highlights

- **Save protection and recovery** with validated local protection, Current / Previous history and manual emergency recovery material.
- **Google Drive synchronization** for protected saves plus the information required to recover the Game Sync Hub library on another PC.
- **Multi-PC safety** with divergence detection and protection against blindly overwriting an unknown local save.
- **New-PC/reinstall recovery**: recover the library from Drive and re-link a game to its new executable/save location.
- **Game metadata scraper**: search public candidates and apply available cover art, horizontal backgrounds, icons and descriptions.
- **Console Mode** with dynamic game artwork, themes, configurable background effects, favourites/recent games and controller-first navigation.
- **Controller support** for Xbox/XInput, PlayStation, Nintendo and generic HID devices, with adaptive button glyphs and reconnection handling.
- **Automatic Console Mode entry** when a controller is connected, if enabled, or direct Console Mode startup.
- **Play statistics** including play time, sessions and last-played information.
- **Offline-friendly operation** with pending synchronization resumed when connectivity returns and a Transfer Center for real sync activity.
- **Optional Anti-UAC rules** for trusted games/launchers without globally disabling Windows UAC.
- **Optional MSI Afterburner + RTSS controller shortcut**: Menu/Start + View/Select can reuse the configured Toggle On-Screen Display hotkey during a game.
- **Built-in updater** for future stable GitHub Releases, with SHA-256 verification, safe-state checks, startup handshake and rollback protection.
- **Portable single-file distribution**: the public Windows build is delivered as one self-contained `GameSyncHub.exe`.

➡️ **[See the complete feature guide](docs/guides/features.md)**

### Visual overview

![Game Sync Hub overview](docs/media/01-overview.png)

Game Sync Hub can identify a real game, retrieve its available artwork/metadata, protect its save folder and present the result in both the desktop library and Console Mode.

![Add game and save protection](docs/media/add-game-and-save.gif)

- [Complete feature guide](docs/guides/features.md)
- [Visual documentation](docs/guides/visual-documentation-es.md)
- [Quick-start visual guide](docs/media/quick-start-es.png)
- [Recovery visual guide](docs/media/recovery-es.png)

### Downloads and updates

Official builds are published only in **[Releases](https://github.com/IMC93Labs/GameSyncHub-Releases/releases)**.

Game Sync Hub is distributed as a portable Windows executable. The application includes a built-in updater that checks this repository for newer stable official releases and asks for confirmation before installing them. The downloaded executable is verified against the release manifest before replacement, and the updater includes rollback protection if the new build cannot complete its startup confirmation.

> Do not download Game Sync Hub from unofficial mirrors unless a release note explicitly points to them.

### Important notice

Game Sync Hub is a **personal hobby project**, created in my free time. I am **not a professional software developer**.

Development is carried out through **AI-assisted vibe coding**. Artificial-intelligence tools are used to generate, modify, review, document and test parts of the project.

The application is designed and tested with safety and reliability in mind, but software — especially software developed with AI assistance — can contain bugs, incompatibilities or unexpected behaviour. **Game Sync Hub is provided as-is, without guarantees, and you choose to use it at your own risk.**

Because Game Sync Hub can work with save files, local folders, NTFS links and cloud synchronization, keeping an **independent backup of important data** is strongly recommended.

Read the full **[Disclaimer](DISCLAIMER.md)** before using the application.

### Support

- **Bug:** [Report a bug](https://github.com/IMC93Labs/GameSyncHub-Releases/issues/new/choose)
- **Feature request:** [Request an improvement](https://github.com/IMC93Labs/GameSyncHub-Releases/issues/new/choose)
- **Questions and general help:** [Discussions](https://github.com/IMC93Labs/GameSyncHub-Releases/discussions)
- **Security issue:** read [Security policy](SECURITY.md) and report it privately when possible.

Support is provided on a best-effort basis. This is a hobby project and there is no guaranteed response time or service level.

### Source code

This repository is used for **official releases, public documentation and user support**. The source code is not published here.

See also: **[Support](SUPPORT.md)** · **[Security](SECURITY.md)** · **[Contributing](CONTRIBUTING.md)** · **[Disclaimer](DISCLAIMER.md)**

---

<a id="espanol"></a>
## Español

### ¿Qué es Game Sync Hub?

Game Sync Hub es una aplicación portable para Windows diseñada para organizar juegos locales de PC, proteger y recuperar sus partidas guardadas, sincronizar mediante Google Drive la información necesaria y ofrecer una experiencia de consola manejable con mando desde el televisor o el sofá.

Combina la biblioteca de escritorio con protección de saves, recuperación multi-PC, enriquecimiento automático de arte/metadatos, soporte de mandos e integraciones opcionales como reglas Anti-UAC y el atajo de overlay de rendimiento de MSI Afterburner/RTSS.

### Funciones destacadas

- **Protección y recuperación de partidas** con protección local validada, historial Current / Previous y material de recuperación manual para emergencias.
- **Sincronización mediante Google Drive** de partidas protegidas y de la información necesaria para recuperar la biblioteca de Game Sync Hub en otro PC.
- **Seguridad multi-PC** con detección de divergencias y protección frente a la sustitución ciega de una partida local desconocida.
- **Recuperación tras reinstalar/cambiar de PC**: recuperar la biblioteca desde Drive y volver a vincular cada juego con su nuevo ejecutable/ruta de saves.
- **Scraper de metadatos e imágenes**: busca candidatos públicos y aplica portada, fondo horizontal, icono y descripción cuando están disponibles.
- **Modo consola** con arte dinámico por juego, temas, efectos de fondo configurables, favoritos/recientes y navegación orientada a mando.
- **Soporte de mandos** Xbox/XInput, PlayStation, Nintendo y HID genéricos, con iconos adaptados y gestión de reconexión.
- **Entrada automática en Modo consola** al conectar un mando, si se activa, o inicio directo en Modo consola.
- **Estadísticas de juego** con tiempo jugado, sesiones y última vez jugado.
- **Trabajo sin conexión** con sincronización pendiente al volver la red y Centro de transferencias para mostrar actividad real.
- **Reglas Anti-UAC opcionales** para juegos/launchers de confianza sin desactivar globalmente el UAC de Windows.
- **Atajo opcional para MSI Afterburner + RTSS**: Menu/Start + View/Select puede reutilizar la tecla Toggle On-Screen Display configurada para abrir/cerrar el overlay durante un juego.
- **Actualizador integrado** para futuras Releases estables, con validación SHA-256, comprobación de estado seguro, confirmación de arranque y rollback.
- **Distribución portable en un solo archivo**: la versión pública de Windows se entrega como un `GameSyncHub.exe` self-contained.

➡️ **[Ver la guía completa de funciones](docs/guides/features.md#español)**

### Vista visual

![Vista general de Game Sync Hub](docs/media/01-overview.png)

Game Sync Hub puede identificar un juego real, obtener su arte/metadatos disponibles, proteger su carpeta de partidas y mostrar el resultado tanto en la biblioteca de escritorio como en Modo consola.

![Añadir juego y proteger partidas](docs/media/add-game-and-save.gif)

- [Guía completa de funciones](docs/guides/features.md#español)
- [Documentación visual](docs/guides/visual-documentation-es.md)
- [Guía visual rápida](docs/media/quick-start-es.png)
- [Guía visual de recuperación](docs/media/recovery-es.png)

### Descargas y actualizaciones

Las compilaciones oficiales se publican únicamente en **[Releases](https://github.com/IMC93Labs/GameSyncHub-Releases/releases)**.

Game Sync Hub se distribuye como un ejecutable portable para Windows. La aplicación incluye un actualizador integrado que consulta este repositorio para detectar versiones oficiales estables más recientes y solicita confirmación antes de instalarlas. El ejecutable descargado se valida frente al manifiesto de la Release antes de sustituir el actual, y el sistema dispone de rollback si la nueva versión no completa correctamente su confirmación de arranque.

> No descargues Game Sync Hub desde mirrors o páginas no oficiales salvo que una Release indique expresamente lo contrario.

### Aviso importante

Game Sync Hub es un **proyecto personal creado como hobby** y desarrollado en mi tiempo libre. **No soy desarrollador de software profesional.**

El desarrollo se realiza mediante **vibe coding asistido por inteligencia artificial**. Se utilizan herramientas de IA para generar, modificar, revisar, documentar y probar partes del proyecto.

La aplicación se diseña y prueba buscando que sea segura y fiable, pero cualquier software —especialmente software desarrollado con ayuda de IA— puede contener errores, incompatibilidades o comportamientos no previstos. **Game Sync Hub se proporciona tal cual, sin garantías, y cada usuario decide utilizarlo bajo su propia responsabilidad.**

Como Game Sync Hub puede trabajar con partidas guardadas, carpetas locales, enlaces NTFS y sincronización en la nube, se recomienda encarecidamente mantener una **copia de seguridad independiente de los datos importantes**.

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
