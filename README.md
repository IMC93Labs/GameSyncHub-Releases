<p align="center">
  <strong>GAME SYNC HUB</strong><br>
  <sub>PC library · Console Mode · Controller integration · Save protection · Cloud recovery</sub>
</p>

<p align="center">
  <a href="https://github.com/IMC93Labs/GameSyncHub-Releases/releases/latest"><img alt="Latest release" src="https://img.shields.io/github/v/release/IMC93Labs/GameSyncHub-Releases?display_name=tag&sort=semver"></a>
  <img alt="Platform" src="https://img.shields.io/badge/platform-Windows-0078D4">
  <img alt="Release" src="https://img.shields.io/badge/channel-stable-2ea44f">
  <img alt="Build" src="https://img.shields.io/badge/tests-1651%2F1651%20PASS-2ea44f">
</p>

<p align="center">
  <a href="https://github.com/IMC93Labs/GameSyncHub-Releases/releases/latest"><strong>Download latest stable release</strong></a>
  ·
  <a href="docs/guides/features.md">Features</a>
  ·
  <a href="docs/guides/visual-documentation.md">Visual guide</a>
  ·
  <a href="SUPPORT.md">Support</a>
</p>

<p align="center">
  <img src="docs/media/07-console-mode.png" alt="Game Sync Hub Console Mode" width="92%">
</p>

> **v1.1.0 is now installer-based.** Previous portable users should install v1.1.0 manually. Future supported releases can be installed through Game Sync Hub's built-in updater.

[English](#english) · [Español](#español)

---

<a id="english"></a>
## English

### Turn a Windows gaming PC into a controller-first console experience

Game Sync Hub brings your local PC games into one place and adds a **Console Mode designed for TV/couch use**, while protecting saves locally and synchronizing recovery data through Google Drive.

It combines a desktop library, controller-aware game launching, play statistics, artwork/metadata, save protection, cloud recovery and an installed update system in one Windows application.

### What's new in v1.1.0

**v1.1.0 is the largest architectural update so far.** It moves Game Sync Hub to an installed application model and substantially strengthens controller, save/cloud and lifecycle reliability.

- **Installer-based distribution** with safe Setup-over-Setup updates prepared for future releases.
- **Controller Virtualization** for Xbox-compatible controllers over Bluetooth and Xbox Wireless Adapter, with isolation designed to avoid double input.
- **Control Center and Guide-button handling** during games, including haptic feedback and controller lifecycle recovery.
- **Controller Device Broker + HidHide integration** without per-game UAC prompts.
- **Durable save/cloud operations** with resumable work, recovery and multi-PC conflict protection.
- **Library reconstruction from Google Drive**, including metadata and artwork recovery.
- **Improved Add Game and multimedia flow.**
- **Safer startup, shutdown, session and updater lifecycle.**

➡️ **[Read the v1.1.0 release notes](docs/releases/v1.1.0.md)**

### Core experience

<p align="center">
  <img src="docs/media/01-overview.png" alt="Game Sync Hub desktop library" width="48%">
  <img src="docs/media/08-console-background.png" alt="Game Sync Hub console background" width="48%">
</p>

**Console Mode**

Use a gamepad-first interface for a living-room PC: browse the library, launch games, move through console menus and use each game's artwork as the visual experience.

**Controller integration**

Game Sync Hub handles controller presence, reconnection and game-session handoff. Xbox-compatible controllers have physically validated Bluetooth and Xbox Wireless Adapter paths in v1.1.0.

**Save protection and cloud recovery**

Protected saves are handled local-first. Google Drive adds redundancy and recovery data without being required for normal offline play. Durable operations and conflict detection are designed to avoid silently replacing independent progress.

**Library and metadata**

Add local games, enrich them with covers/backgrounds/icons/descriptions, keep play statistics and reconstruct the managed library on another PC when the required cloud data is available.

**Optional integrations**

Game Sync Hub can integrate with MSI Afterburner + RTSS for controller-based OSD toggling and can manage trusted Anti-UAC launch rules without disabling Windows UAC globally.

➡️ **[See the complete feature guide](docs/guides/features.md)**

### Install

1. Open the **[latest stable release](https://github.com/IMC93Labs/GameSyncHub-Releases/releases/latest)**.
2. Download `GameSyncHub-Setup-v1.1.0.exe` (or the Setup matching the latest version).
3. Run the installer and follow the setup wizard.
4. Launch Game Sync Hub normally. The application itself does not need to run elevated.

The `.sha256` file published with each Setup can be used to verify the download independently.

> Users coming from v1.0.x portable builds should install v1.1.0 manually. The public distribution model from v1.1.0 onward is the installer.

### Updates

Game Sync Hub checks the official stable GitHub release channel. The installed updater validates the release contract and downloaded Setup before handing installation to the installer. Drafts, prereleases, legacy portable ZIPs and invalid manifests are not part of the public update path.

### Validation

v1.1.0 was closed with:

- **1651/1651 automated tests PASS**
- **Release build: 0 warnings / 0 errors**
- Physical validation of Bluetooth and Xbox Wireless Adapter controller paths
- Physical Setup-over-Setup validation
- End-to-end installed update validation (`1.1.0 → 1.1.1` synthetic local release) with durable `Completed` handshake
- Extensive save/cloud interruption, recovery and multi-PC conflict testing performed during development

### Save safety

Game Sync Hub is designed to prefer verified local state and explicit recovery over silent destructive replacement. Even so, no software can guarantee zero risk when working with save files, local folders, NTFS links or cloud synchronization.

**Keep an independent backup of important saves.**

### Project status and source

This repository contains **official releases, public documentation and user support**. The application source code is not published here.

Game Sync Hub is a personal hobby project built with AI-assisted development and is provided as-is. See the full **[Disclaimer](DISCLAIMER.md)** before use.

### Support

- [Report a bug or request an improvement](https://github.com/IMC93Labs/GameSyncHub-Releases/issues/new/choose)
- [Questions and general help](https://github.com/IMC93Labs/GameSyncHub-Releases/discussions)
- [Support policy](SUPPORT.md)
- [Security policy](SECURITY.md)

---

<a id="español"></a>
## Español

### Convierte un PC gaming con Windows en una experiencia de consola manejable con mando

Game Sync Hub reúne tus juegos locales de PC en un solo lugar y añade un **Modo consola pensado para televisión y sofá**, mientras protege las partidas de forma local y sincroniza mediante Google Drive la información necesaria para recuperación.

Combina biblioteca de escritorio, lanzamiento adaptado al mando, estadísticas, arte/metadatos, protección de partidas, recuperación en la nube y un sistema de actualización instalado en una sola aplicación para Windows.

### Novedades de v1.1.0

**v1.1.0 es la mayor actualización arquitectónica hasta ahora.** Game Sync Hub pasa a un modelo de aplicación instalada y refuerza de forma importante mandos, Save/Cloud y ciclo de vida.

- **Distribución mediante instalador**, con Setup-over-Setup seguro preparado para futuras actualizaciones.
- **Controller Virtualization** para mandos compatibles con Xbox mediante Bluetooth y Xbox Wireless Adapter, con aislamiento pensado para evitar doble input.
- **Centro de Control y botón Guide** durante el juego, con respuesta háptica y recuperación del ciclo de vida del mando.
- **Controller Device Broker + HidHide**, sin solicitar UAC cada vez que se inicia un juego.
- **Operaciones Save/Cloud durables**, reanudables y con recuperación y protección frente a conflictos entre varios PCs.
- **Reconstrucción de biblioteca desde Google Drive**, incluidos metadatos y multimedia.
- **Mejoras en Añadir juego y selección multimedia.**
- **Mayor seguridad en inicio, cierre, sesiones y actualizaciones.**

➡️ **[Leer las notas de v1.1.0](docs/releases/v1.1.0.md#español)**

### Experiencia principal

<p align="center">
  <img src="docs/media/06-library-final.png" alt="Biblioteca de Game Sync Hub" width="48%">
  <img src="docs/media/07-console-mode.png" alt="Modo consola de Game Sync Hub" width="48%">
</p>

**Modo consola**

Interfaz pensada para utilizar el PC desde el sofá: recorre la biblioteca con mando, inicia juegos, utiliza menús de estilo consola y muestra el arte de cada título como parte de la experiencia.

**Integración de mandos**

Game Sync Hub gestiona presencia, reconexión y transferencia del mando a la sesión de juego. En v1.1.0 se han validado físicamente las rutas Bluetooth y Xbox Wireless Adapter para mandos compatibles con Xbox.

**Protección de partidas y recuperación cloud**

Las partidas protegidas siguen una filosofía local-first. Google Drive aporta redundancia y material de recuperación sin ser necesario para jugar normalmente sin conexión. Las operaciones durables y la detección de conflictos evitan sustituir silenciosamente progresos independientes.

**Biblioteca y metadatos**

Añade juegos locales, completa portadas/fondos/iconos/descripciones, conserva estadísticas y reconstruye la biblioteca gestionada en otro PC cuando la información necesaria está disponible en la nube.

**Integraciones opcionales**

Game Sync Hub puede integrarse con MSI Afterburner + RTSS para alternar el OSD desde el mando y gestionar reglas Anti-UAC para software de confianza sin desactivar globalmente el UAC de Windows.

➡️ **[Ver la guía completa de funciones](docs/guides/features.md#español)**

### Instalación

1. Abre la **[última versión estable](https://github.com/IMC93Labs/GameSyncHub-Releases/releases/latest)**.
2. Descarga `GameSyncHub-Setup-v1.1.0.exe` (o el Setup correspondiente a la versión más reciente).
3. Ejecuta el instalador y sigue el asistente.
4. Inicia Game Sync Hub normalmente. La aplicación no necesita ejecutarse elevada.

El archivo `.sha256` publicado junto a cada Setup permite verificar la descarga de forma independiente.

> Si vienes de una versión portable v1.0.x, instala v1.1.0 manualmente. Desde v1.1.0 el método público de distribución es el instalador.

### Actualizaciones

Game Sync Hub consulta el canal estable oficial de GitHub. El actualizador instalado valida el contrato de la Release y el Setup descargado antes de entregar la instalación al instalador. Los borradores, prereleases, ZIP portables antiguos y manifiestos inválidos no forman parte del camino público de actualización.

### Validación

v1.1.0 se cerró con:

- **1651/1651 pruebas automatizadas PASS**
- **Build Release: 0 warnings / 0 errors**
- Validación física de mandos mediante Bluetooth y Xbox Wireless Adapter
- Validación física de Setup-over-Setup
- Validación end-to-end de actualización instalada (`1.1.0 → 1.1.1` sintética local) con handshake durable `Completed`
- Amplias baterías de interrupción, recuperación y conflictos multi-PC de Save/Cloud realizadas durante el desarrollo

### Seguridad de las partidas

Game Sync Hub está diseñado para priorizar estados locales verificados y recuperación explícita frente a sustituciones destructivas silenciosas. Aun así, ningún software puede garantizar riesgo cero al trabajar con partidas, carpetas locales, enlaces NTFS o sincronización en la nube.

**Mantén una copia de seguridad independiente de las partidas importantes.**

### Estado del proyecto y código fuente

Este repositorio contiene **versiones oficiales, documentación pública y soporte a usuarios**. El código fuente de la aplicación no se publica aquí.

Game Sync Hub es un proyecto personal creado como hobby mediante desarrollo asistido por IA y se proporciona tal cual. Consulta el **[Aviso y responsabilidad](DISCLAIMER.md)** antes de utilizarlo.

### Soporte

- [Reportar un error o solicitar una mejora](https://github.com/IMC93Labs/GameSyncHub-Releases/issues/new/choose)
- [Preguntas y ayuda general](https://github.com/IMC93Labs/GameSyncHub-Releases/discussions)
- [Política de soporte](SUPPORT.md)
- [Política de seguridad](SECURITY.md)

---

<p align="center"><strong>Game Sync Hub · IMC93Labs</strong></p>
