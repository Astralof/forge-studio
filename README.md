# Forge Studio

Desktop-Cockpit für die Spieleentwicklung mit KI-Agenten – für **Windows** (Linux-Pakete folgen wieder).
Du arbeitest in einem Chat, Forge verteilt die Arbeit an **Claude Code**, **ChatGPT (über die Codex CLI)** und eine **lokale KI (Ollama)**, zeigt live, was die Agenten tun, und lässt dich Bilder, 3D-Modelle, Musik und Konzeptfragen direkt freigeben. Spiele baut und testet Forge mit **Godot**, 3D-Modelle und Renderings entstehen mit **Blender**, Bilder auf Wunsch lokal mit **ComfyUI**.

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

## Was Forge kann

- **Ein Chat für alles:** Forge entscheidet regelbasiert, wer eine Nachricht bearbeitet (Claude, ChatGPT oder die lokale KI), teilt gemischte Wünsche auf und zeigt an deiner Nachricht, ob sie wartet, läuft oder fertig ist. An jeder fertigen Antwort: **„✓ Übernehmen“** oder **„↩ Antworten / anpassen“**. Bilder fügst du mit Strg+V ein.
- **Forge schläft nie (außer du pausierst):** Ist Claude im Abo-Limit, bleibt nichts liegen – Aufträge warten und laufen nach dem Reset automatisch weiter, oder (Einstellung) ChatGPT übernimmt sofort. **„⏹ Alles stoppen“** gibt den PC mit einem Klick frei, „▶ Weiter“ setzt fort.
- **Freigaben & Entscheidungen:** Rückfragen der Agenten werden zu Entscheidungskarten (auch „Nicht jetzt entscheiden“); Assets, Sounds und Änderungen gibst du je Datei frei oder lehnst sie ab.
- **Sicher arbeiten lassen:** Schreib-Aufträge laufen in einer Arbeitskopie mit Änderungsprüfung, jede Datei wird vor einer Änderung gesichert, Löschen/Umbenennen braucht ein eigenes Recht, und nach jeder Änderung laufen automatisch die betroffenen Tests (ohne Token-Kosten).
- **Godot:** Spiel starten, Tests, KI-Demo mit Aufnahme und Prüfung, Installer per Knopf. Optional verbindet Forge Claude mit dem **laufenden Godot-Editor** (MCP), damit Szenen über den Editor statt als Text geändert werden.
- **Bilder lokal erzeugen (ComfyUI):** Z-Image Turbo und FLUX.2 klein – nur Modelle, die für ein verkauftes Spiel lizenziert sind; Ergebnisse kommen als Freigabe-Karte.
- **KI-Herkunft & Steam:** Forge liest aus KI-Bildern Modell, Prompt und Lizenz, prüft sie für den Verkauf und erzeugt den Text für Steams Angabe zu KI-Inhalten.
- **Projekt-Überblick:** Roadmap und Meilensteine, Konzept, Graph, Verlauf, Code & Git, Medien-Browser mit Vorschau (Bilder, 3D, Ton, Video).

## Updates

Forge prüft beim Start und alle 6 Stunden, ob es hier ein neues Release gibt (ohne Konto, ohne Token). Ein Klick lädt das Paket, prüft **Prüfsumme und Signatur** (Ed25519 – nur vom Herausgeber signierte Pakete werden installiert), sichert deine Datenbank und installiert. Laufende Aufträge werden nicht kaputtgemacht: Forge wartet auf einen sicheren Punkt und setzt sie nach dem Neustart fort.

## Voraussetzungen (optional, je nach Nutzung)

- **Claude Code** (Claude-Abo) – https://docs.claude.com/en/docs/claude-code
- **Codex CLI** (ChatGPT-Abo) – `npm install -g @openai/codex`
- **Ollama** für die lokale KI – https://ollama.com (empfohlen: ein Modell ab ~7B, z. B. `qwen2.5:7b`)
- **Godot 4** für Godot-Projekte – https://godotengine.org
- **Blender** für 3D-Modelle, Rigging, Animationen und Renderings (Agenten steuern es per Skript) – https://www.blender.org
- **ComfyUI** für lokale Bilderzeugung – https://github.com/Comfy-Org/ComfyUI
- **Node.js** für die optionale Godot-Editor-Anbindung (MCP) – https://nodejs.org

Forge nutzt die **Abos** der CLIs. **Kostenpflichtige APIs sind standardmäßig gesperrt** und werden nie automatisch als Ersatz verwendet. Forge installiert nichts ungefragt – unter *Projekt → Einrichtung* steht für jede Funktion, was sie braucht.

## Datenschutz & Sicherheit

- Deine Projekte bleiben auf deinem Rechner; Forge schreibt nur mit deiner Freigabe ins Projekt (Änderungen mit Sicherung und Rücknahme).
- **„Was geht raus?“** im Chat zeigt vor dem Senden, was an Anthropic bzw. OpenAI geht und was auf dem PC bleibt; lokale KI und ComfyUI arbeiten ohne Internet.
- Zugangsdaten (z. B. ein GitHub-Token) liegen im Schlüsselspeicher des Betriebssystems, nie in Logs.
- Forge liest keine Login-Dateien, Cookies oder Tokens der KI-Tools.

## Lizenz

Die Nutzung der veröffentlichten Pakete ist frei. Weitere Lizenzbedingungen folgen.
