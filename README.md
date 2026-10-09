<!---
BurningSheep1/BurningSheep1 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

<div align="center">

# Hallo, ich bin Manuel 👋

Hauptberuflich arbeite ich an Organisation und Transformation.<br>
Hier baue ich Werkzeuge für mich, meine Familie und meinen Homeserver.

🇩🇪 Deutsch · 🇬🇧 [English](#-english)

</div>

---

## 🇩🇪 Deutsch

### Projekte

#### Wissen & Organisation

| | Projekt | Worum es geht | Technik |
|---|---|---|---|
| 🧠 | **OKF Studio** | Lokales Wissensmanagement nach dem **LLM-Wiki-Ansatz von Andrej Karpathy**, kombiniert mit dem **Open Knowledge Format (OKF)**. Notizen unterwegs in Sekunden erfassen – auch im Funkloch –, später einarbeiten: Die KI schlägt einen Änderungssatz über mehrere Seiten vor, ich prüfe ihn, ein Git-Commit übernimmt ihn. Dazu Volltext-, semantische und hybride Suche, eine Frageansicht für alle, die nur etwas wissen wollen, ein Pflegelauf für verwaiste Seiten und tote Verweise, eine REST-API für n8n und ein **MCP-Server für Claude**. Markdown bleibt die führende Quelle, alles andere ist abgeleitet. Die KI ist austauschbar (Ollama, Gemini, OpenAI) und optional. | FastAPI · React · SQLite · MCP |
| 🌳 | **Decision Space** | Entscheidungen steuern und dokumentieren: Was hängt wovon ab – und was muss neu geprüft werden, wenn sich eine frühere Entscheidung ändert? | Next.js · PostgreSQL |
| 🧩 | **Business-Skills für Claude** | Deutschsprachige Skills für Mitarbeitende im Mittelstand, nutzbar in Claude Code und auf claude.ai. Ein gemeinsames **Unternehmensprofil** gibt allen Skills Kontext; daraus entstehen zum Beispiel **Entscheidungsvorlagen** für die Geschäftsführung mit Optionen, Bewertungsmatrix, Risiken und Empfehlung. | Claude Code · Skills |

#### Familie & Alltag

| | Projekt | Worum es geht | Technik |
|---|---|---|---|
| 📇 | **FriendsCRM** | Persönliches Beziehungsmanagement über **Signal**: Einmal am Tag kommt, was ansteht – Geburtstage, Jahrestage, erwähnte Ereignisse, Geschenkideen. Ich antworte im selben Chat, was ich erfahren habe; eine lokale KI macht daraus Vorschläge, die ich mit einem Tap bestätige. Die KI schreibt nie direkt in den Datenbestand, jeder Fakt verweist auf seine Quelle. Dazu Kalender-Abo, Fragen per Signal (`? Lisa`), Abruf der Metadaten zu Telefonaten, und eine Web-App zum Pflegen. Keine Cloud in der Verarbeitung. | FastAPI · SvelteKit · PostgreSQL + pgvector · signal-cli · Ollama |
| 🎧 | **Podcastplayer** | Selbst gehosteter Podcastplayer: Neue Folgen laufen von selbst durch – laden, transkribieren, zusammenfassen. Volltextsuche in den Transkripten, Podcast-Suche, Kapitel, Hörstatistik. Dazu eine native **Android-App mit Android Auto**: Sie lädt Folgen im WLAN vor, spielt sie offline im Auto ab und meldet den Hörstand an den Server zurück. | FastAPI · Svelte · Kotlin · Jetpack Compose · Gemini |
| 🧸 | **Kinderplayer** | Hörspiel-Player fürs Kinder-Tablet: große Cover-Kacheln, alle Folgen auf einer Seite, ein Knopf – Spotify ohne Spotify-App. Wahlweise über Lautsprecher im WLAN (Sonos, Echo, Chromecast), dann ist das Tablet nur Fernbedienung. Mit Elternbereich und als App installierbar. | Node.js · Express · Spotify Web Playback SDK |
| 🎨 | **Klecks** | Mal-App für Kinder von 3 bis 9: freies Malen, Ausmalbilder und Malen nach Zahlen, mit einem Chamäleon als Maskottchen. Offline, ohne Werbung, ohne Tracking, ohne Konten. Unterstützt Stifte mit Druckempfindlichkeit und Handballenerkennung. Eine Codebasis für Android-Tablet und Browser. | Svelte · Capacitor · PWA |

#### Gesundheit & Sport

| | Projekt | Worum es geht | Technik |
|---|---|---|---|
| 🏃 | **Laufplan** | Trainingspläne aus Garmin-Daten: Läufe kommen jeden Morgen automatisch aus Garmin Connect. Wochenanalyse, Herzfrequenzzonen, Prognose auf die Zieldistanz und ein Mehrwochenplan bis zum Wettkampf – mit ausformulierten Einheiten statt reiner Kilometerangaben. Optional verfeinert durch ein lokales Sprachmodell. | FastAPI · Ollama · Garmin Connect |

#### Spiele

| | Projekt | Worum es geht | Technik |
|---|---|---|---|
| ⚔️ | **Ätherfront** | Kompetitives Sammelkartenspiel zum Anfassen: Zonenkontrolle statt Lebenspunkte, jede Karte ist Einheit, Ressource oder verdeckter Schläfer. Dazu eine Balancing-Engine, die Tausende Partien mit Bots simuliert und auswertet, und spielbare Prototypen im Browser. | Node.js · React |
| 🚐 | **Ablesetour** | Browserspiel über den Alltag eines Ablesedienstes: Wasserzähler ablesen, Heizkostenverteiler tauschen, Rauchmelder prüfen – mit Feierabendverkehr, Blitzern, Glatteis und einem Biber, der Kupferrohre liebt. Wochenendprojekt, entstanden als Spaß unter Kollegen. | HTML5 · JavaScript |

#### Im Netz

| | Projekt | Worum es geht | Technik |
|---|---|---|---|
| 📚 | **KI-Notizen** | Ein Websiteprojekt mit Grundlagenwissen zu KI, ursprünglich gestartet für Familie und Freunde: kostenlos, ohne Werbung, ohne Affiliate-Links, ohne Kurse. Die Menschen, von denen ich selbst lerne, sind dort verlinkt. **Aktuell offline. Überarbeitung der Inhalte und Zielgruppe** | Astro |

### Homelab & KI selbst gehostet

Auf meinem **Proxmox**-Server laufen die Bausteine, auf denen die Projekte aufsetzen – jedes Projekt in einem eigenen LXC-Container, gesichert mit dem **Proxmox Backup Server**. **Caddy** holt die Zertifikate über **deSEC** per DNS-Challenge, so bleibt alles im Heimnetz, ohne Portfreigabe; von unterwegs geht es übers VPN. Für semantische Suche und RAG kommen eigene **Embedding-Modelle**, **Qdrant** und **pgvector** dazu. **n8n** verbindet das Ganze zu Automatisierungen.

Die Modelle selbst laufen auf einem eigenen Rechner mit einer 16-GB-Grafikkarte. Dort betreibe ich Embedding- und Sprachmodelle mit **Ollama** – etwa Gemma 4 (12B), gpt-oss (20B) oder DeepSeek-R1 (14B) – und Bildmodelle mit **ComfyUI**, vor allem kompakte Flux-Modelle. So bleiben die Daten im eigenen Netz, und ich kann Modelle ausprobieren, ohne für jeden Versuch zu bezahlen. Gehostete Modelle wie Gemini oder Claude nutze ich dort, wo sie klar besser sind und keine privaten Daten anfallen.

### Wie ich baue

- 🏠 **Selbst gehostet.** Die meisten Projekte laufen in LXC-Containern auf Proxmox, von außen erreichbar übers VPN.
- 📄 **Offene Formate.** Die Daten gehören mir und bleiben lesbar – auch ohne die App.
- 🤖 **KI, wo sie hilft – und optional.** Fällt das Modell aus, funktioniert der Rest weiter. Und die KI macht Vorschläge, entscheiden tue ich.
- 🛠️ **Mit Claude Code.** Ich entwickle hauptsächlich mit Claude Code: Ich lege Architektur und Entscheidungen fest, Claude Code setzt um.
- 🧑‍👩‍👧 **Für den echten Alltag.** Gebaut für konkrete Probleme zu Hause, nicht als Demo.

### Werkzeuge

**KI & Modelle** `Claude` `Gemini` `Ollama` `ComfyUI` `Embedding-Modelle` `MCP`<br>
**Selbst hosten** `Proxmox` `n8n` `signal-cli` `Proxmox Backup Server` `Caddy` `VPN`<br>
**Daten & Wissen** `PostgreSQL` `SQLite` `Qdrant` `Obsidian`<br>
**Entwicklung** `Claude Code` `Git` `GitHub`<br>

---

## 🇬🇧 English

### Projects

#### Knowledge & organisation

| | Project | What it does | Stack |
|---|---|---|---|
| 🧠 | **OKF Studio** | Local knowledge management following **Andrej Karpathy's LLM wiki approach**, combined with the **Open Knowledge Format (OKF)**. Capture notes on the go in seconds – even without signal – and work them in later: the AI proposes a change set across several pages, I review it, and a Git commit applies it. Plus full-text, semantic and hybrid search, a Q&A view for people who just want answers, a maintenance run for orphaned pages and dead links, a REST API for n8n and an **MCP server for Claude**. Markdown stays the source of truth; everything else is derived. The AI is swappable (Ollama, Gemini, OpenAI) and optional. | FastAPI · React · SQLite · MCP |
| 🌳 | **Decision Space** | Steer and document decisions: what depends on what – and what needs to be reviewed when an earlier decision changes? | Next.js · PostgreSQL |
| 🧩 | **Business skills for Claude** | German-language skills for employees of small and mid-sized companies, usable in Claude Code and on claude.ai. A shared **company profile** gives every skill its context; from it come, for example, **decision papers** for management with options, a scoring matrix, risks and a recommendation. | Claude Code · Skills |

#### Family & everyday life

| | Project | What it does | Stack |
|---|---|---|---|
| 📇 | **FriendsCRM** | Personal relationship management via **Signal**: once a day it tells me what's coming up – birthdays, anniversaries, events people mentioned, gift ideas. I reply in the same chat with what I've learned; a local AI turns it into suggestions I confirm with one tap. The AI never writes to the data directly, and every fact links back to its source. Plus a calendar feed, questions via Signal (`? Lisa`) and a web app for editing. No cloud in the processing chain. | FastAPI · SvelteKit · PostgreSQL + pgvector · signal-cli · Ollama |
| 🎧 | **Podcastplayer** | Self-hosted podcast player: new episodes go through on their own – download, transcribe, summarise. Full-text search across transcripts, podcast search, chapters, listening stats. Plus a native **Android app with Android Auto**: it pre-loads episodes over Wi-Fi, plays them offline in the car and syncs listening progress back to the server. | FastAPI · Svelte · Kotlin · Jetpack Compose · Gemini |
| 🧸 | **Kinderplayer** | Audio-drama player for a kids' tablet: big cover tiles, every episode on one page, one button – Spotify without the Spotify app. Or play through Wi-Fi speakers (Sonos, Echo, Chromecast) and the tablet becomes a remote. With a parents' area, installable as an app. | Node.js · Express · Spotify Web Playback SDK |
| 🎨 | **Klecks** | Drawing app for kids aged 3 to 9: free drawing, colouring pages and paint by numbers, with a chameleon mascot. Offline, no ads, no tracking, no accounts. Supports pressure-sensitive styluses and palm rejection. One codebase for Android tablet and browser. | Svelte · Capacitor · PWA |

#### Health & sport

| | Project | What it does | Stack |
|---|---|---|---|
| 🏃 | **Laufplan** | Running plans from Garmin data: runs are pulled from Garmin Connect every morning. Weekly analysis, heart-rate zones, race-time prediction and a multi-week plan up to race day – with fully written-out sessions instead of bare distances. Optionally refined by a local language model. | FastAPI · Ollama · Garmin Connect |

#### Games

| | Project | What it does | Stack |
|---|---|---|---|
| ⚔️ | **Ätherfront** | Competitive physical trading card game: zone control instead of life points, and every card is a unit, a resource or a face-down sleeper. Plus a balancing engine that simulates and analyses thousands of bot games, and playable browser prototypes. | Node.js · React |
| 🚐 | **Ablesetour** | Browser game about a day as a meter reader: read water meters, swap heat-cost allocators, check smoke alarms – with rush-hour traffic, speed cameras, black ice and a beaver that loves copper pipes. Weekend project for colleagues. | HTML5 · JavaScript |

#### On the web

| | Project | What it does | Stack |
|---|---|---|---|
| 📚 | **KI-Notizen** | A website project with AI fundamentals: free, no ads, no affiliate links, no courses. The people I learn from myself are linked there. **Currently offline** | Astro |

### Homelab & self-hosted AI

My **Proxmox** server runs the building blocks the projects rely on – each project in its own LXC container, backed up with **Proxmox Backup Server**. **Caddy** gets certificates from **deSEC** via DNS challenge, so everything stays on the home network without port forwarding; on the road I use a VPN. For semantic search and RAG I add my own **embedding models**, **Qdrant** and **pgvector**. **n8n** ties it all together into automations.

The models themselves run on a separate machine with a 16 GB GPU. There I run embedding and language models with **Ollama** – for example Gemma 4 (12B), gpt-oss (20B) or DeepSeek-R1 (14B) – and image models with **ComfyUI**, mainly compact Flux models. Data stays on my own network, and I can try out models without paying for every experiment. I use hosted models such as Gemini or Claude where they are clearly better and no private data is involved.

### How I build

- 🏠 **Self-hosted.** Most projects run in LXC containers on Proxmox, reachable from outside via VPN.
- 📄 **Open formats.** The data is mine and stays readable – even without the app.
- 🤖 **AI where it helps – and optional.** If the model is down, everything else keeps working. And the AI suggests; I decide.
- 🛠️ **With Claude Code.** I mainly develop with Claude Code: I define the architecture and the decisions, Claude Code implements them.
- 🧑‍👩‍👧 **Built for real life.** Made for concrete problems at home, not as demos.

### Tools

**AI & models** `Claude` `Gemini` `Ollama` `ComfyUI` `embedding models` `MCP`<br>
**Self-hosting** `Proxmox` `n8n` `signal-cli` `Proxmox Backup Server` `Caddy` `deSEC` `VPN`<br>
**Data & knowledge** `PostgreSQL` `pgvector` `SQLite` `Qdrant` `Obsidian` <br>
**Development** `Claude Code` `Git` `GitHub`<br>
