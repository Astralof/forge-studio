# Forge Studio

Desktop-Cockpit für die Spieleentwicklung mit KI-Agenten – für **Windows** und **Linux**.
Du arbeitest in einem Chat, Forge verteilt die Arbeit an **Claude Code**, **ChatGPT (über die Codex CLI)** und eine **lokale KI (Ollama)**, zeigt live, was die Agenten tun, und lässt dich Bilder, 3D-Modelle, Musik und Konzeptfragen direkt freigeben. Spiele baut und testet Forge mit **Godot**, 3D-Modelle und Renderings entstehen mit **Blender**.

> Dieses Repository enthält die **offiziellen Releases** (Installer + automatische Updates). Der Quellcode liegt separat.

## Download

**Aktuelle Version: 0.8.4**

| System | Download |
|---|---|
| Windows 10/11 – Installer (empfohlen) | [**ForgeStudio-0.8.4-windows-x64-setup.exe**](https://github.com/Astralof/forge-studio/releases/download/v0.8.4/ForgeStudio-0.8.4-windows-x64-setup.exe) |
| Windows – portabel, ohne Installation | [**ForgeStudio-0.8.4-windows-x64-portable.zip**](https://github.com/Astralof/forge-studio/releases/download/v0.8.4/ForgeStudio-0.8.4-windows-x64-portable.zip) |

Ältere Versionen und Prüfsummen: [alle Releases](https://github.com/Astralof/forge-studio/releases)

Danach aktualisiert sich Forge selbst – du musst hier nicht wieder vorbeischauen.

**Windows-Hinweis:** Die Installer sind (noch) nicht mit einem Code-Signing-Zertifikat signiert. Windows SmartScreen zeigt deshalb „Unbekannter Herausgeber“ → „Weitere Informationen“ → „Trotzdem ausführen“.

## Updates

Forge prüft beim Start und alle 6 Stunden, ob es hier ein neues Release gibt (ohne Konto, ohne Token). Ein Klick lädt das Paket, prüft **Prüfsumme und Signatur** (Ed25519 – nur vom Herausgeber signierte Pakete werden installiert), sichert deine Datenbank und installiert. Laufende Aufträge werden nicht kaputtgemacht: Forge wartet auf sie oder setzt sie nach dem Neustart fort.

## Voraussetzungen (optional, je nach Nutzung)

- **Claude Code** (Claude-Abo) – https://docs.claude.com/en/docs/claude-code
- **Codex CLI** (ChatGPT-Abo) – `npm install -g @openai/codex`
- **Ollama** für die lokale KI – https://ollama.com
- **Godot 4** für Godot-Projekte – https://godotengine.org
- **Blender** für 3D-Modelle, Animationen und Renderings (Agenten steuern es per Skript) – https://www.blender.org

Forge nutzt die **Abos** der CLIs. **Kostenpflichtige APIs sind standardmäßig gesperrt** und werden nie automatisch als Ersatz verwendet.

## Datenschutz & Sicherheit

- Deine Projekte bleiben auf deinem Rechner; Forge schreibt nur mit deiner Freigabe ins Projekt (Änderungen mit Sicherung und Rücknahme).
- Zugangsdaten (z. B. ein GitHub-Token) liegen im Schlüsselspeicher des Betriebssystems, nie in Logs.
- Forge liest keine Login-Dateien, Cookies oder Tokens der KI-Tools.

## Lizenz

Die Nutzung der veröffentlichten Pakete ist frei. Weitere Lizenzbedingungen folgen.
