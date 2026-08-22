# Game Sync Hub — Visual documentation / Documentación visual

[English](#english) · [Español](#español)

---

<a id="english"></a>
## English

This guide uses a continuous demo based on real game metadata and media cached by Game Sync Hub. The main flow follows **Red Dead Redemption 2** from add-game to library and Console Mode.

### 1. Add a game

![Add Red Dead Redemption 2](../media/02-add-game.png)

Game Sync Hub accepts EXE, LNK, BAT and CMD launchers. The launcher path is local to the PC and is not synchronized to Google Drive.

### 2. Scraper and game art

![Scraper candidates](../media/03-scraper-search.png)

![Selected scraper result](../media/04-scraper-result.png)

The assistant keeps a stable provider identity, such as Steam AppID, and associates cover, background and description with that game.

### 3. SavePath and protection

![SavePath setup](../media/05-save-path.png)

Known save paths are portable. Game Sync Hub suggests paths only when they exist on the current PC.

![Save protection](../media/09-save-protection.png)

### 4. Library

![Library overview](../media/01-overview.png)

![Final library](../media/06-library-final.png)

The demo library shows Red Dead Redemption 2 plus other real games with their own cover/background metadata.

### 5. Console Mode

![Console Mode with RDR2](../media/07-console-mode.png)

![Console Mode with another selected game](../media/08-console-background.png)

The selected game changes the cover and background dynamically.

![Console multi-game GIF](../media/console-multi-game.gif)

### 6. Controller integration

![Controller settings](../media/10-controller-settings.png)

Console Mode is designed around logical actions, with controller glyphs adapted to the selected controller profile.

![Controller console GIF](../media/controller-console.gif)

### 7. Performance overlay shortcut

![Performance overlay settings](../media/11-performance-overlay.png)

Game Sync Hub does not install MSI Afterburner or RivaTuner Statistics Server. With MSI Afterburner + RTSS already configured, Menu/Start + View/Select toggles the RTSS On-Screen Display directly when the RTSS interface is available, independently of the keyboard hotkey configured in Afterburner. The hotkey path remains only as a compatibility fallback.

### 8. Anti-UAC launcher support

![Anti-UAC settings](../media/12-anti-uac.png)

Anti-UAC rules are tied to the game identity and verified launcher. Game Sync Hub does not disable Windows UAC globally.

### 9. Recovery

![Recovery guide](../media/13-recovery.png)

The recovery image is marked as a guide: it is built from real UI fragments and real cached media to explain the safety flow without exposing personal data.

### 10. Updates

![Updates](../media/14-updates.png)

Stable public updates are checked from the official release repository.

---

<a id="español"></a>
## Español

Esta guía usa una demo continua basada en metadatos y multimedia reales cacheados por Game Sync Hub. El flujo principal sigue **Red Dead Redemption 2** desde el alta hasta la biblioteca y el Modo consola.

### 1. Añadir un juego

![Añadir Red Dead Redemption 2](../media/02-add-game.png)

Game Sync Hub acepta lanzadores EXE, LNK, BAT y CMD. La ruta del lanzador es local del PC y no se sincroniza con Google Drive.

### 2. Scraper y arte del juego

![Candidatos del scraper](../media/03-scraper-search.png)

![Resultado seleccionado del scraper](../media/04-scraper-result.png)

El asistente conserva una identidad estable del proveedor, como Steam AppID, y asocia portada, fondo y descripción con ese juego.

### 3. SavePath y protección

![Configurar SavePath](../media/05-save-path.png)

Las rutas conocidas de partidas son portables. Game Sync Hub solo las sugiere cuando existen en el PC actual.

![Protección de partidas](../media/09-save-protection.png)

### 4. Biblioteca

![Vista general de biblioteca](../media/01-overview.png)

![Biblioteca final](../media/06-library-final.png)

La biblioteca demo muestra Red Dead Redemption 2 y otros juegos reales con su propia portada/fondo.

### 5. Modo consola

![Modo consola con RDR2](../media/07-console-mode.png)

![Modo consola con otro juego seleccionado](../media/08-console-background.png)

El juego seleccionado cambia dinámicamente la portada y el fondo.

![GIF de Modo consola multi-juego](../media/console-multi-game.gif)

### 6. Mandos

![Ajustes de mando](../media/10-controller-settings.png)

El Modo consola usa acciones lógicas y adapta los glyphs al perfil de mando seleccionado.

![GIF de consola con mando](../media/controller-console.gif)

### 7. Atajo de overlay de rendimiento

![Ajustes de overlay de rendimiento](../media/11-performance-overlay.png)

Game Sync Hub no instala MSI Afterburner ni RivaTuner Statistics Server. Con MSI Afterburner + RTSS ya configurados, Menu/Start + View/Select muestra u oculta directamente el OSD de RTSS cuando su interfaz está disponible, independientemente de la tecla configurada en Afterburner. La ruta basada en hotkey queda únicamente como fallback de compatibilidad.

### 8. Anti-UAC

![Ajustes Anti-UAC](../media/12-anti-uac.png)

Las reglas Anti-UAC se vinculan a la identidad del juego y a un launcher verificado. Game Sync Hub no desactiva UAC globalmente.

### 9. Recuperación

![Guía de recuperación](../media/13-recovery.png)

La imagen de recuperación está marcada como guía: usa fragmentos reales de UI y multimedia real cacheada para explicar el flujo sin exponer datos personales.

### 10. Actualizaciones

![Actualizaciones](../media/14-updates.png)

Las actualizaciones públicas estables se comprueban desde el repositorio oficial de releases.
