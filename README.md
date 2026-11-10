# Forge Studio

Desktop-Cockpit für die Spieleentwicklung mit KI-Agenten – für **Windows** und **Linux**.
Du arbeitest in einem Chat, Forge verteilt die Arbeit an **Claude Code**, **ChatGPT (über die Codex CLI)** und eine **lokale KI (Ollama)**, zeigt live, was die Agenten tun, und lässt dich Bilder, 3D-Modelle, Musik und Konzeptfragen direkt freigeben.

> Dieses Repository enthält die **offiziellen Releases** (Installer + automatische Updates). Der Quellcode liegt separat.

## Download

Unter **[Releases](../../releases/latest)**:

| System | Datei |
|---|---|
| Windows 10/11 (Installer) | `ForgeStudio-<version>-windows-x64-setup.exe` |
| Windows (portabel, ohne Installation) | `ForgeStudio-<version>-windows-x64-portable.zip` |
| Linux (AppImage) | `ForgeStudio-<version>-linux-x86_64.AppImage` |
| Ubuntu/Debian | `forge-studio_<version>_amd64.deb` |

**Windows-Hinweis:** Die Installer sind (noch) nicht mit einem Code-Signing-Zertifikat signiert. Windows SmartScreen zeigt deshalb „Unbekannter Herausgeber“ → „Weitere Informationen“ → „Trotzdem ausführen“.

## Updates

Forge prüft beim Start und alle 6 Stunden, ob es hier ein neues Release gibt (ohne Konto, ohne Token). Ein Klick lädt das Paket, prüft **Prüfsumme und Signatur** (Ed25519 – nur vom Herausgeber signierte Pakete werden installiert), sichert deine Datenbank und installiert. Laufende Aufträge werden nicht kaputtgemacht: Forge wartet auf sie oder setzt sie nach dem Neustart fort.

## Voraussetzungen (optional, je nach Nutzung)

- **Claude Code** (Claude-Abo) – https://docs.claude.com/en/docs/claude-code
- **Codex CLI** (ChatGPT-Abo) – `npm install -g @openai/codex`
- **Ollama** für die lokale KI – https://ollama.com
- **Godot 4** für Godot-Projekte – https://godotengine.org

Forge nutzt die **Abos** der CLIs. **Kostenpflichtige APIs sind standardmäßig gesperrt** und werden nie automatisch als Ersatz verwendet.

## Datenschutz & Sicherheit

- Deine Projekte bleiben auf deinem Rechner; Forge schreibt nur mit deiner Freigabe ins Projekt (Änderungen mit Sicherung und Rücknahme).
- Zugangsdaten (z. B. ein GitHub-Token) liegen im Schlüsselspeicher des Betriebssystems, nie in Logs.
- Forge liest keine Login-Dateien, Cookies oder Tokens der KI-Tools.

## Lizenz

Die Nutzung der veröffentlichten Pakete ist frei. Weitere Lizenzbedingungen folgen.
