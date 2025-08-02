# CZT-WDS Launcher 

**CZT-WDS Launcher** is an all-in-one tool for managing Steam-based dedicated servers (ARMA, Rust, SCUM, Insurgency Sandstorm, and more) with a simple, modern interface. No command-line knowledge required!

---

## Key Features

* **Easy Server Management:** Start, stop, update, and configure servers for many popular games with just a few clicks.
* **SteamCMD Integration:** Built-in SteamCMD handling for seamless server downloads and updates.
* **Scheduled Restarts & Updates:** Automate your server’s maintenance and downtime.
* **Crash Protection:** Optional monitoring and auto-restart if your server crashes.
* **Logs & Backups:** Integrated log management and optional backups on restart.
* **Account System:** Supports free and premium user accounts, with extra features for premium.
* **User-Friendly UI:** Modern, dark-mode interface using CustomTkinter.

---

## How to Install

1. **Download the latest release from the [Releases page](../../releases).**
2. **Run `CZT-WDS_Launcher_Setup.exe`.**
3. **Launch the app from your desktop or Start Menu shortcut. (Run as Admin)**
4. **Register or log in within the app to start managing your servers.**

> CZT needs to be "Run as Administrator" due to how it Starts/Stops the server. 

> No Python or additional installs required.

---

## Supported Games / Engines

* SCUM
* Rust
* Insurgency Sandstorm (ISS)
* ARMA
* Source Engine games (CS\:GO, Garry’s Mod, etc.)
* Unreal Engine servers (ARK, Conan Exiles, etc.)
* Unity-based servers
  *...and more!*

---

## Premium Features

* Scheduled restarts and updates
* Crash protection
* Extra automation and advanced controls

---

> **Note:** All server management happens on your computer. Licensing is hardware-bound for security.

---

## How to Use

**SteamCZT - WDS (Windows Dedicated Server) Manager**
\~ Created By CaZual\_T ...x\_x

### First Time Use

* **Go to the WDS Config tab**
* **Click \[Install Dependencies]** Installs DirectX and Visual C++ redistributables if needed.
* **Enter App ID (and save):** Click the `?` for valid App IDs.
* **Click \[First Time Install]:** Installs SteamCMD and selected server files.
* Wait for everything to install (watch the log window).
* Start your server!

> *Note:* If your server fails to start due to an invalid SteamCMD login, check the bottom of the log window.

---

### Main Controls

* **Main Buttons (Start, Stop, Restart, Update):**

  * **Start:** Starts the server.
  * **Stop:** Stops the server.
  * **Manual Restart:** Manually restart the server.
  * **Update Only:** Closes server (if running) then updates/verifies server files.
* *Note: 'Stop' & 'Manual Restart' will create a backup of the .db or save folder if \[Auto Backup] is enabled.*

---

### Scheduled Restarts

* Add/remove restart times by entering a time (24hr format, e.g., 23:59) and clicking \[+Add Time].
* `[DEL Schedule]` clears all saved times.
* `[Show Current]` displays active restart times.
* Will create backups if \[Auto Backup] is selected.
* Will update/verify the current AppID if \[Auto Update] is enabled.

---

### WDS Config

* Set **Server Paths** (with option to open file locations).
* Set **Port Number** (see Port Setup below).
* Set **Max Players** (overrides server config).
* Set **App ID** (used by SteamCMD).
* **Game Specific Args:** Presets for specific games.
* **Engine Specific Args:** Universal arguments (see your game's server docs for more info).
* **Install Dependencies:** Installs DX Runtime and latest C++ redistributables.

---

### Port Setup

Start server on specified port. Connection port will be port+2.

**Example:**
If port is set to 7000, then players connect using `Your.Server.I.P:7002`.

* Port forward **both** ports on your network and add them to your host machine's firewall:

  1. **Windows Defender Firewall:**

     * New rule (UDP 7000, TCP 7002, UDP 27015).
  2. **Router:** Port forward the same ports.

---

### SteamCMD Login

* Credentials are saved locally (your PC only) for use with SteamCMD.
* Some games require a real SteamCMD user, others allow "anonymous."
* Click `?` next to App ID in the server config tab for requirements.
* **You do NOT need to enter a username/password unless your server requires it.**

---






