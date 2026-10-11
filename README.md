
<div align="center">

# Hallo, ich bin Manuel 👋

Hier baue ich Werkzeuge und PoCs für mich, meine Familie & Freunde auf meinen Homeserver. <br>
Mit und dank KI.

🇩🇪 Deutsch · 🇬🇧 [English](#-english)

</div>

---

## 🇩🇪 Deutsch

### Projekte

#### Wissen & Organisation

| | Projekt | Worum es geht | Technik |
|---|---|---|---|
| 🧠 | **OKF Studio** | Lokales Wissensmanagement nach dem **LLM-Wiki-Ansatz von Andrej Karpathy**, kombiniert mit dem **Open Knowledge Format (OKF)**. Notizen unterwegs in Sekunden erfassen, auch im Funkloch, später einarbeiten: Die KI schlägt einen Änderungssatz über mehrere Seiten vor, ich prüfe ihn, ein Git-Commit übernimmt ihn. Dazu Volltext-, semantische und hybride Suche, eine Frageansicht für alle, die nur etwas wissen wollen, ein Pflegelauf für verwaiste Seiten und tote Verweise, eine REST-API für n8n und ein **MCP-Server für Claude**. Markdown bleibt die führende Quelle, alles andere ist abgeleitet. Die KI ist austauschbar (Ollama, Gemini, OpenAI) und optional. | LLM Wiki · OKF · Ollama · MCP |
| 🌳 | **Decision Space** | Entscheidungen steuern und dokumentieren: Was hängt wovon ab – und was muss neu geprüft werden, wenn sich eine frühere Entscheidung ändert? | Next.js · PostgreSQL |
| 🧩 | **Business-Skills für Claude** | Deutschsprachige Skills für Mitarbeitende im Mittelstand, nutzbar in Claude Code und im Chat (als Prompt). Ein gemeinsames **Unternehmensprofil** gibt allen Skills Kontext; daraus entstehen zum Beispiel **Entscheidungsvorlagen** für die Geschäftsführung mit Optionen, Bewertungsmatrix, Risiken und Empfehlung. | Claude Code · Skills |

#### Familie & Alltag

| | Projekt | Worum es geht | Technik |
|---|---|---|---|
| 📇 | **FriendsCRM** | Persönliches Beziehungsmanagement über **Signal**: Einmal am Tag kommt, was ansteht – Geburtstage, Jahrestage, erwähnte Ereignisse, Geschenkideen. Ich antworte im selben Chat, was ich erfahren habe; eine lokale KI macht daraus Vorschläge, die ich mit einem Tap bestätige. Die KI schreibt nie direkt in den Datenbestand, jeder Fakt verweist auf seine Quelle. Dazu Kalender-Abo, Fragen per Signal-Chat, Abruf der Metadaten zu Telefonaten und eine Web-App zum Pflegen. | signal-cli · Ollama · lokale App |
| 🎧 | **Podcastplayer** | Selbst gehosteter Podcastplayer: Neue Folgen laufen von selbst durch: laden, transkribieren, zusammenfassen. Volltextsuche in den Transkripten, Podcast-Suche, Kapitel, Hörstatistik. Dazu eine native **Android-App mit Android Auto**: Sie lädt Folgen im WLAN vor, spielt sie offline im Auto ab und meldet den Hörstand an den Server zurück. | Native App · Android Auto · Gemini |
| 🧸 | **Kinderplayer** | Hörspiel-Player fürs Kinder-Tablet: große Cover-Kacheln, alle Folgen auf einer Seite, ein Knopf: Spotify ohne Spotify-App. Wahlweise über Lautsprecher im WLAN (Sonos, Echo, Chromecast), dann ist das Tablet nur Fernbedienung. Mit Elternbereich und als App installierbar. | Spotify Web Playback SDK |
| 🎨 | **Klecks** | Mal-App für Kinder von 3 bis 9: freies Malen, Ausmalbilder und Malen nach Zahlen. Offline, ohne Werbung, ohne Tracking, ohne Konten. Unterstützt Stifte mit Druckempfindlichkeit und Handballenerkennung. Eine Codebasis für Android-Tablet und Browser. | PWA |

#### Gesundheit & Sport

| | Projekt | Worum es geht | Technik |
|---|---|---|---|
| 🏃 | **Laufplan** | Trainingspläne aus Garmin-Daten: Läufe kommen jeden Morgen automatisch aus Garmin Connect. Wochenanalyse, Herzfrequenzzonen, Prognose auf die Zieldistanz und ein Mehrwochenplan bis zum Wettkampf – mit ausformulierten Einheiten statt reiner Kilometerangaben. Der Trainingsplan optional verfeinert durch ein lokales Sprachmodell. | FastAPI · Ollama · Garmin Connect |

#### Spiele

| | Projekt | Worum es geht | Technik |
|---|---|---|---|
| ⚔️ | **Ätherfront** | Kompetitives Kartenspiel: Zonenkontrolle statt Lebenspunkte, jede Karte ist Einheit, Ressource oder verdeckter Schläfer. Dazu eine Balancing-Engine, die Tausende Partien mit Bots simuliert und auswertet, spielbar im Browser. | Node.js · React |
| 🚐 | **Ablesetour** | Browserspiel über den Alltag eines Ablesedienstes: Wasserzähler ablesen, Heizkostenverteiler tauschen, Rauchmelder prüfen. Mit Feierabendverkehr, Blitzern, Glatteis und einem Biber, der Kupferrohre liebt. Wochenendprojekt, entstanden als Spaß unter Kollegen. | HTML5 · JavaScript |

#### Im Netz

| | Projekt | Worum es geht | Technik |
|---|---|---|---|
| 📚 | **KI-Notizen** | Ein Websiteprojekt mit Grundlagenwissen zu KI, ursprünglich gestartet für Familie und Freunde: kostenlos, ohne Werbung, ohne Affiliate-Links, ohne Kurse. Die Menschen, von denen ich selbst lerne, sind dort verlinkt. **Aktuell offline – Inhalte und Zielgruppe werden überarbeitet.** | Astro |

### Homelab & KI selbst gehostet

Auf meinem **Proxmox**-Server laufen die Projekt in LXC-Containern, gesichert mit dem **Proxmox Backup Server**. Wo eine PWA nötig holt **Caddy** die Zertifikate über **deSEC**; von unterwegs geht es übers VPN. Für semantische Suche und RAG kommen lokale **Embedding-Modelle**, **Qdrant** und **pgvector** dazu. **n8n** verbindet das Ganze wo sinnvoll zu Automatisierungen.

Die Modelle selbst laufen auf einem eigenen Rechner mit einer 16-GB-Grafikkarte. Dort betreibe ich Embedding- und Sprachmodelle mit **Ollama** – etwa Gemma 4 (12B), und Bildmodelle mit **ComfyUI**, vor allem kompakte Flux-Modelle. So bleiben die Daten im eigenen Netz, und ich kann Modelle verschiedener Größen für Aufgaben ausprobieren. Gehostete Modelle wie Gemini oder Claude nutze ich dort, wo keine privaten Daten verarbeitet werden.

### Wie ich baue

- 🏠 **Selbst gehostet.** Die meisten Projekte laufen in LXC-Containern auf Proxmox, von außen erreichbar übers VPN. KI-Features in den Apps über Ollama.
- 🛠️ **Mit Claude Code.** Ich entwickle hauptsächlich mit Claude Code: Ich entscheide, Claude Code setzt um.
- 🧑‍👩‍👧 **Für den echten Alltag.** Gebaut für konkrete Probleme zu Hause und die Arbeit, nicht als Demo.

### Werkzeuge

**KI & Modelle** `Claude` `Gemini` `Ollama` `ComfyUI` `Embedding-Modelle` `MCP`<br>
**Selbst hosten** `Proxmox` `n8n` `signal-cli` `Proxmox Backup Server` `Caddy` `VPN`<br>
**Daten & Wissen** `PostgreSQL` `SQLite` `Qdrant` `Obsidian`<br>
**Entwicklung** `Claude Code` `Git` `GitHub`

---

## 🇬🇧 English

### Projects

#### Knowledge & organisation

| | Project | What it does | Stack |
|---|---|---|---|
| 🧠 | **OKF Studio** | Local knowledge management following **Andrej Karpathy's LLM wiki approach**, combined with the **Open Knowledge Format (OKF)**. Capture notes on the go in seconds – even without signal – and work them in later: the AI proposes a change set across several pages, I review it, and a Git commit applies it. Plus full-text, semantic and hybrid search, a Q&A view for people who just want answers, a maintenance run for orphaned pages and dead links, a REST API for n8n and an **MCP server for Claude**. Markdown stays the source of truth; everything else is derived. The AI is swappable (Ollama, Gemini, OpenAI) and optional. | LLM wiki · OKF · Ollama · MCP |
| 🌳 | **Decision Space** | Steer and document decisions: what depends on what – and what needs to be reviewed when an earlier decision changes? | Next.js · PostgreSQL |
| 🧩 | **Business skills for Claude** | German-language skills for employees of small and mid-sized companies, usable in Claude Code and in a Chat (as Prompt). A shared **company profile** gives every skill its context; from it come, for example, **decision papers** for management with options, a scoring matrix, risks and a recommendation. | Claude Code · Skills |

#### Family & everyday life

| | Project | What it does | Stack |
|---|---|---|---|
| 📇 | **FriendsCRM** | Personal relationship management via **Signal**: once a day it tells me what's coming up – birthdays, anniversaries, events people mentioned, gift ideas. I reply in the same chat with what I've learned; a local AI turns it into suggestions I confirm with one tap. The AI never writes to the data directly, and every fact links back to its source. Plus a calendar feed, questions via Signal (`? Lisa`), call metadata import and a web app for editing. No cloud AI in the processing chain. | signal-cli · Ollama · local app |
| 🎧 | **Podcastplayer** | Self-hosted podcast player: new episodes go through on their own – download, transcribe, summarise. Full-text search across transcripts, podcast search, chapters, listening stats. Plus a native **Android app with Android Auto**: it pre-loads episodes over Wi-Fi, plays them offline in the car and syncs listening progress back to the server. | Native app · Android Auto · Gemini |
| 🧸 | **Kinderplayer** | Audio-drama player for a kids' tablet: big cover tiles, every episode on one page, one button – Spotify without the Spotify app. Or play through Wi-Fi speakers (Sonos, Echo, Chromecast) and the tablet becomes a remote. With a parents' area, installable as an app. | Spotify Web Playback SDK |
| 🎨 | **Klecks** | Drawing app for kids aged 3 to 9: free drawing, colouring pages and paint by numbers. Offline, no ads, no tracking, no accounts. Supports pressure-sensitive styluses and palm rejection. One codebase for Android tablet and browser. | PWA |

#### Health & sport

| | Project | What it does | Stack |
|---|---|---|---|
| 🏃 | **Laufplan** | Running plans from Garmin data: runs are pulled from Garmin Connect every morning. Weekly analysis, heart-rate zones, race-time prediction and a multi-week plan up to race day – with fully written-out sessions instead of bare distances. Plan optionally refined by a local language model. | FastAPI · Ollama · Garmin Connect |

#### Games

| | Project | What it does | Stack |
|---|---|---|---|
| ⚔️ | **Ätherfront** | Competitive physical trading card game: zone control instead of life points, and every card is a unit, a resource or a face-down sleeper. Plus a balancing engine that simulates and analyses thousands of bot games, and playable browser prototypes. | Node.js · React |
| 🚐 | **Ablesetour** | Browser game about a day as a meter reader: read water meters, swap heat-cost allocators, check smoke alarms – with rush-hour traffic, speed cameras, black ice and a beaver that loves copper pipes. A weekend project, made for fun among colleagues. | HTML5 · JavaScript |

#### On the web

| | Project | What it does | Stack |
|---|---|---|---|
| 📚 | **KI-Notizen** | A website project with AI fundamentals, originally started for family and friends: free, no ads, no affiliate links, no courses. The people I learn from myself are linked there. **Currently offline – content and audience are being reworked.** | Astro |

### Homelab & self-hosted AI

My projects run in LXC containers on a **Proxmox** server and are backed up using **Proxmox Backup Server**. Where a PWA is required, **Caddy** handles certificate retrieval via **deSEC**, while remote access is managed via VPN. Local **embedding models**, **Qdrant**, and **pgvector** are used for semantic search and RAG, with **n8n** linking everything together into automated workflows where appropriate.

The models themselves run on a dedicated machine equipped with a 16 GB graphics card. I use **Ollama** to host embedding and language models—such as Gemma 4 (12B)—and **ComfyUI** for image models, primarily compact Flux variants. This setup keeps data within my own network and allows me to experiment with models of various sizes for different tasks. I use hosted models like Gemini or Claude only when no private data is being processed.

### How I build

- 🏠 **Self-hosted.** Most projects run in LXC containers on Proxmox, reachable from outside via VPN.
- 🛠️ **With Claude Code.** I mainly develop with Claude Code: I decide, Claude Code implements.
- 🧑‍👩‍👧 **Built for real life.** Made for concrete problems at home or work, not as demos.

### Tools

**AI & models** `Claude` `Gemini` `Ollama` `ComfyUI` `embedding models` `MCP`<br>
**Self-hosting** `Proxmox` `n8n` `signal-cli` `Proxmox Backup Server` `Caddy` `VPN`<br>
**Data & knowledge** `PostgreSQL` `SQLite` `Qdrant` `Obsidian`<br>
**Development** `Claude Code` `Git` `GitHub`
