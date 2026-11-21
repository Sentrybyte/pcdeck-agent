# PCDeck Agent for Windows

The PC side of **[PCDeck](https://sentrybyte.github.io/pcdeck/)** – control your Windows PC from your Android phone over Wi-Fi.

## Download

**[⬇ PCDeck-Agent-Setup.exe](https://github.com/Sentrybyte/pcdeck-agent/releases/latest/download/PCDeck-Agent-Setup.exe)** (Windows 10 / 11, 64-bit)

## Install

1. Run `PCDeck-Agent-Setup.exe` and allow it to make changes (it needs admin rights once to set up the firewall and autostart).
2. If Windows SmartScreen says *"Windows protected your PC"*, click **More info → Run anyway**. The installer is not code-signed yet.
3. The agent starts in the system tray and runs automatically when you sign in.
4. Open PCDeck on your phone (same Wi-Fi), tap your PC and confirm the pairing code.

## What the installer does

- Installs the agent to `C:\Program Files\PCDeck`.
- Allows incoming connections on TCP 5600 and UDP 5601 **from your local network only**.
- Adds a "PCDeck Agent" task that starts the agent when you sign in.
- Everything is removed by the uninstaller (Settings → Apps → PCDeck Agent).

## Security

All traffic between the phone and the PC is encrypted with TLS. The phone pins the PC's key, and every new phone must be confirmed on the PC with a matching code. See the [privacy policy](https://sentrybyte.github.io/pcdeck/privacy.html).

Questions: sentry0byte@gmail.com
