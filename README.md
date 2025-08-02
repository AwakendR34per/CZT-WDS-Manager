[CZT-WDS Launcher]
- CZT-WDS Launcher is an all-in-one tool for managing Steam-based dedicated servers (ARMA, Rust, SCUM, Insurgency Sandstorm, and more) with a simple, modern interface. No command-line knowledge required!

[Key Features]
- Easy Server Management: Start, stop, update, and configure servers for many popular games with just a few clicks.
- SteamCMD Integration: Built-in SteamCMD handling for seamless server downloads and updates.
- Scheduled Restarts & Updates: Automate your server’s maintenance and downtime.
- Crash Protection: Optional monitoring and auto-restart if your server crashes.
- Logs & Backups: Integrated log management and optional backups on restart.
- Account System: Supports free and premium user accounts, with extra features for premium.
- User-Friendly UI: Modern, dark-mode interface using CustomTkinter.

[How to Install]
- Download the latest release from the Releases page.
- Unzip and run SteamCZT_WDS_Launcher.exe.
- Register or log in within the app to start managing your servers.
- No Python or additional installs required.

[Supported Games / Engines]
- SCUM
- Rust
- Insurgency Sandstorm (ISS)
- ARMA
- Source Engine games (CS:GO, Garry’s Mod, etc.)
- Unreal Engine servers (ARK, Conan Exiles, etc.)
- Unity-based servers
More!

[Premium Features]
- Scheduled restarts and updates
- Crash protection
- Extra automation and advanced controls

Note: All server management happens on your computer. Licensing is hardware-bound for security.

 ========================================================================================

How to use:

SteamCZT - WDS (Windows Dedicated Server) Manager. 
    
    ~ Created By CaZual_T ...x_x

 ========================================================================================
 
[First Time Use]
    → [Install Dependencies] Installs DirectX and Visual C++ redistributables. (if needed)
    → Enter App ID (and save) You can click the ? for valid App IDs.
    → [First Time Install] installs SteamCMD and selected "App ID" server files. 
    → Wait for everything to install. (check log window)
    → Start your server!  
    
    [Note:] Scroll to the bottom if your server failed to start due to an invalid steamcmd login.

 ========================================================================================
                    
[Main Controls]
    [Main Buttons] (Start, Stop, Restart, Update)
    → Start = Starts the server.
    → Stop = Stops the server. 
    → Manual Restart = Manually restart the server.
    → Update Only = Closes Server (if running) then updates/verify server files.
    [Note:] 'Stop' & 'Manual Restart' will create a backup of .db or save folder if [Auto Backup] if selected.
                
    [Scheduled Restarts]
    - Here you can add and remove restart times by entering a time and clicking [+Add Time] (must use 24hr format ex. 23:59).
    [DEL Schedule] button clears the cfg of ALL saved time.
    [Show Current] button shows all of your active restart times. 
    → Will create a .db or save backup if [Auto Backup] if selected.
    → Will update/verify the current AppID selected if [Auto Update] if selected.

 ========================================================================================
                    
[WDS Config]
    → Set [Server Pathways] (option to open file locations as well)
    → Set [Port Number] (more info below @ PORT_SETUP)
    → Set [Max Players] overrides the max player option within serversetting.ini
    → Set [App ID] this is what get put into SteamCMD when the server is updated.
    → [Game Specific ARGS] These are presets of optional launch arguments for specific games.
    → [Engine Specific ARGS] Universal arguments, check the selected apps dev server docs for more          arguments info.      
    → [Install Dependencies] Installs DX Runtime and Latest C++ redistributables from microsoft
                    
[Port Setup]
    Start server on specified port. Connection port will be port+2                     
    EXAMPLE: If port is set to 7000, then players would connect using Your.Server.I.P:7002
        - Be sure to port forward BOTH ports on your network, and add them to your host machines firewall inbound rules. 
            1:) Windows Defender Firewall > Advanced Settings > Inbound Rules (left side) > New Rule (right side) 
                → Add a new rule with protocol UDP for 7000 (your server port)
                → Add a new rule with protocol TCP for 7002 (client port 'server port+2')
                → Add a new rule with protocol UDP for 27015 (steam query port)     
            2:) Login to your router and port forward the same ports.
                    
                    
[SteamCMD Login]
    → These credentials are saved locally (to your pc only) for use with SteamCMD command line.
    → Some games dont accept "anonymous" and require an actual SteamCMD user.
    → Click the question [?] mark next to "App ID" on the server config tab to check requirements.
    
    → YOU DO NOT NEED TO ENTER A USERNAME AND PASSWORD UNLESS YOUR GAMES SERVER REQUIRES IT.
                    