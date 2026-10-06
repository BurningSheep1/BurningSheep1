
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

| | Projekt | Worum es geht | Technik |
|---|---|---|---|
| 🧠 | **OKF Studio** | Lokales Wissensmanagement nach dem **LLM-Wiki-Ansatz von Andrej Karpathy**, kombiniert mit Googles **Open Knowledge Format (OKF)**: Weboberfläche, Graphansicht der Verknüpfungen, Volltext- und semantische Suche, Fragen an eine KI, MCP-Server für Claude. Markdown bleibt die führende Quelle, alles andere ist abgeleitet. | Python · FastAPI · React · SQLite |
| 🌳 | **Decision Space** | Entscheidungen steuern und dokumentieren: Was hängt wovon ab – und was muss neu geprüft werden, wenn sich eine frühere Entscheidung ändert? | Next.js · TypeScript · PostgreSQL |
| 📇 | **Privates CRM** | Kontakte und Beziehungen pflegen – direkt über **Signal**: Text- und Sprachnachrichten an das CRM schicken, eine KI wertet sie aus und pflegt sie ein. Über n8n werden aus Ereignissen Aktionen. | signal-cli · KI für Text & Sprache · n8n |
| 🎧 | **Podcastplayer** | Selbst gehosteter Podcastplayer mit Transkription, Volltextsuche und Zusammenfassungen. Dazu eine native Android-App mit **Android Auto**: Sie lädt Folgen im WLAN vor, spielt sie offline im Auto ab und meldet den Hörstand an den Server zurück. | Python · FastAPI · Kotlin · Jetpack Compose · Gemini |
| 🧸 | **Kinderplayer** | Hörspiel-Player fürs Kinder-Tablet: große Cover-Kacheln, ein Knopf, Spotify ohne Spotify-App – wahlweise über Lautsprecher im WLAN. | Node.js · Express · Spotify Web Playback SDK |
| 🏃 | **Laufplan** | Trainingspläne aus Garmin-Daten: Wochenanalyse, Herzfrequenzzonen, Prognose auf die Zieldistanz, optional verfeinert durch ein lokales Sprachmodell. | Python · FastAPI · Ollama |
| 🧩 | **skills** | Deutschsprachige Skills für Claude Code zu Marketing und Organisationsarbeit – für Menschen ohne Fachausbildung im jeweiligen Gebiet. | Claude Code · Plugin-Marketplace |

### Homelab & KI selbst gehostet

Auf meinem Proxmox-Server laufen die Bausteine, auf denen die Projekte aufsetzen. Für semantische Suche und RAG kommen eigene **Embedding-Modelle** und ein **Qdrant**-Vektorspeicher dazu. **n8n** verbindet das Ganze zu Automatisierungen.

Die Modelle selbst laufen auf einem eigenen Rechner mit einer 16-GB-Grafikkarte. Dort betreibe ich Sprachmodelle mit **Ollama** – etwa Gemma 4 (12B), gpt-oss (20B) oder DeepSeek-R1 (14B) – und Bildmodelle mit **ComfyUI**, vor allem kompakte Flux-Modelle. So bleiben die Daten im eigenen Netz, und ich kann Modelle ausprobieren, ohne für jeden Versuch zu bezahlen. Gehostete Modelle wie Gemini oder Claude nutze ich dort, wo sie klar besser sind.

### Wie ich baue

- 🏠 **Selbst gehostet.** Die meisten Projekte laufen in LXC-Containern auf Proxmox, erreichbar übers VPN.
- 📄 **Offene Formate.** Die Daten gehören mir und bleiben lesbar – auch ohne die App.
- 🤖 **KI, wo sie hilft – und optional.** Fällt das Modell aus, funktioniert der Rest weiter.
- 🛠️ **Mit Claude Code.** Ich entwickle hauptsächlich mit Claude Code: Ich lege Architektur und Entscheidungen fest, Claude Code setzt um.
- 🧑‍👩‍👧 **Für den echten Alltag.** Gebaut für konkrete Probleme zu Hause, nicht als Demo.

### Werkzeuge

**Entwicklung** `Claude Code` `Python` `FastAPI` `TypeScript` `React` `Svelte` `Next.js` `Node.js` `Kotlin` `Jetpack Compose`<br>
**Daten** `SQLite` `PostgreSQL` `Qdrant`<br>
**KI** `Ollama` `ComfyUI` `Embedding-Modelle` `Gemini` `Claude`<br>
**Infrastruktur** `Proxmox` `LXC` `Caddy` `n8n` `signal-cli`

---

## 🇬🇧 English

### Projects

| | Project | What it does | Stack |
|---|---|---|---|
| 🧠 | **OKF Studio** | Local knowledge management following **Andrej Karpathy's LLM wiki approach**, combined with Google's **Open Knowledge Format (OKF)**: web editor, graph view of the links, full-text and semantic search, Q&A with an AI, MCP server for Claude. Markdown stays the source of truth; everything else is derived. | Python · FastAPI · React · SQLite |
| 🌳 | **Decision Space** | Steer and document decisions: what depends on what – and what needs to be reviewed when an earlier decision changes? | Next.js · TypeScript · PostgreSQL |
| 📇 | **Personal CRM** | Keep track of contacts and relationships – directly via **Signal**: send text and voice messages to the CRM, an AI interprets them and files them away. n8n turns events into actions. | signal-cli · AI for text & speech · n8n |
| 🎧 | **Podcastplayer** | Self-hosted podcast player with transcription, full-text search and summaries. Plus a native Android app with **Android Auto**: it pre-loads episodes over Wi-Fi, plays them offline in the car and syncs listening progress back to the server. | Python · FastAPI · Kotlin · Jetpack Compose · Gemini |
| 🧸 | **Kinderplayer** | Audio-drama player for a kids' tablet: big cover tiles, one button, Spotify without the Spotify app – or played through Wi-Fi speakers. | Node.js · Express · Spotify Web Playback SDK |
| 🏃 | **Laufplan** | Running plans from Garmin data: weekly analysis, heart-rate zones, race-time prediction, optionally refined by a local language model. | Python · FastAPI · Ollama |
| 🧩 | **skills** | German-language skills for Claude Code covering marketing and organisational work – for people without formal training in the field. | Claude Code · plugin marketplace |

### Homelab & self-hosted AI

My Proxmox server runs the building blocks the projects rely on. For semantic search and RAG I add my own **embedding models** and a **Qdrant** vector store. **n8n** ties it all together into automations.

The models themselves run on a separate machine with a 16 GB GPU. There I run language models with **Ollama** – for example Gemma 4 (12B), gpt-oss (20B) or DeepSeek-R1 (14B) – and image models with **ComfyUI**, mainly compact Flux models. Data stays on my own network, and I can try out models without paying for every experiment. I use hosted models such as Gemini or Claude where they are clearly better.

### How I build

- 🏠 **Self-hosted.** Most projects run in LXC containers on Proxmox, reachable via VPN.
- 📄 **Open formats.** The data is mine and stays readable – even without the app.
- 🤖 **AI where it helps – and optional.** If the model is down, everything else keeps working.
- 🛠️ **With Claude Code.** I mainly develop with Claude Code: I define the architecture and the decisions, Claude Code implements them.
- 🧑‍👩‍👧 **Built for real life.** Made for concrete problems at home, not as demos.

### Tools

**Development** `Claude Code` `Python` `FastAPI` `TypeScript` `React` `Svelte` `Next.js` `Node.js` `Kotlin` `Jetpack Compose`<br>
**Data** `SQLite` `PostgreSQL` `Qdrant`<br>
**AI** `Ollama` `ComfyUI` `embedding models` `Gemini` `Claude`<br>
**Infrastructure** `Proxmox` `LXC` `Caddy` `n8n` `signal-cli`

