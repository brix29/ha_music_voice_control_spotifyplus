# 🎧 Home Assistant Spotify Voice Automations

This repository contains a collection of **Home Assistant automations** that enable **voice-controlled Spotify playback** via custom conversation triggers.  
With these automations, you can **play music**, **adjust volume**, and **control playback effortlessly**.

---

## 🎵 Features

- **Play Music by Artist**  
  *Example (DE):* `"Spiele Musik von Queen"`  
  *Example (EN):* `"Play music by Queen"`

- **Play Specific Songs**  
  *Example (DE):* `"Spiele den Song Bohemian Rhapsody"`  
  *Example (EN):* `"Play the song Bohemian Rhapsody"`

- **Play Podcasts**  
  *Example (DE):* `"Starte den Podcast Fest & Flauschig"`  
  *Example (EN):* `"Start the podcast Fest & Flauschig"`

- **Artist Radio & Playlists**  
  *Example (DE):* `"Spiele das Radio von Coldplay"` or `"Spiele die Playlist Party Hits"`  
  *Example (EN):* `"Play the radio of Coldplay"` or `"Play the playlist Party Hits"`

- **Control Playback**  
  Commands:  
  - *German:* `"Pause Spotify"`, `"Nächstes Lied"`, `"Shuffle an"`, `"Lautstärke auf 50%"`  
  - *English:* `"Pause Spotify"`, `"Next song"`, `"Shuffle on"`, `"Volume to 50%"`

- **Like Songs**  
  *Example (DE):* `"Ich mag dieses Lied"`  
  *Example (EN):* `"I like this song"`

---

## 🚀 Getting Started

### ✅ Prerequisites

- **Home Assistant** with **[SpotifyPlus](https://community.home-assistant.io/t/spotifyplus-integration/698651)** ( Big thanks to @thlucas )
- **Recommended hardware: [Home Assistant Voice Preview Edition (VPE)](https://www.home-assistant.io/voice-pe/)**
- Adjust entity IDs (e.g., `media_player.spotifyplus_yourID`) and Spotify IDs/links as needed.
- Add the following helpers in your `configuration.yaml`:

### 🔧 Helpers Configuration

```yaml
input_text:
  voice_spotify_last_search:
    name: "Last Playlist Search"
    initial: ""
```

```yaml
input_number:
  voice_spotify_last_search_index:
    name: "Last Playlist Search Index"
    min: 0
    max: 10
    step: 1
    mode: box
```

📢 Contributing
Feel free to fork, translate, suggest improvements, or add new automations!
Contributions are always welcome. 😊

For more details, check out the discussion here:
👉 [Home Assistant Community Forum](https://community.home-assistant.io/t/voice-music-control-with-spotifyplus-and-ha-voice-pe/837357)
