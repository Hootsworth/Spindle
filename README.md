# Spindle 🎵

> Swipe to find your sound.

Spindle is an interactive, full-stack music discovery web application combining tactile physical metaphors (spinning vinyl, DJ scratching, card gestures) with algorithmic taste matching, multiplayer listening rooms, and real-time social sharing.

---

## ✨ Features & Innovations

### 🎧 1. Sensory & Vinyl Audio (Web Audio API)
- **Interactive Vinyl Scratching**: Touch and scrub the vinyl record sticking out of the card to dynamically modulate audio playback rate and trigger synthesized analog needle scratch sound effects.
- **Pull-Down Tape Stop**: Dragging down on any card produces an authentic decelerating tape-stop pitch drop effect before springing back.
- **⚡ Drop Jump**: Instant chorus/drop seek button that skips right into the track's peak energy segment.
- **Beat-Reactive Ambient Background**: An `AnalyserNode` frequency pipeline pulses the background glow and ripples the vinyl grooves in sync with real-time bass frequencies.

### 👥 2. Spindle Blend (Multiplayer Match Room)
- **Tinder for Music**: Create a room to get a 6-digit code (e.g., `SPIN84`), or join a friend's room.
- **Synchronized Deck**: Both players swipe through the exact same 10 tracks with live real-time progress indicators.
- **Compatibility Reveal**: An animated score gauge reveals your taste compatibility percentage (e.g. *82% Taste Match!*) and lists mutual favorites with a 1-click **Save All to Library** button.

### 🧬 3. Generative Sound Aura (Music DNA Card)
- **Canvas-Powered Visual Identity**: Generates a high-res, shareable visual card blending radiant radial gradient auras matched to your top listening genres.
- **Aura Archetypes**: Assigns your taste profile an archetype (e.g. *The Midnight Dreamer*, *The Electric Nomad*, *The Sunset Optimist*).
- **1-Click Download & Social Share**: Export to PNG or trigger native Web Share for Instagram Stories / TikTok / Twitter.

### 🧭 4. Dynamic Discovery: Vibe Radar & Time Machine
- **2D Vibe Radar Pad**: Interactive coordinate pad allowing you to drag a puck across two axes (*Chill ⟷ Hype* and *Vintage ⟷ Modern*) to steer recommendations.
- **Time Machine Decades Bar**: Filter your feed across eras (*70s Classics*, *80s Retro*, *90s Golden*, *2000s Y2K*, *2010s Hits*, *2020s Modern*).
- **Pass Roasting**: Swiping left prompts quick roast badges (*😴 Too slow*, *📢 Overproduced*, *🔁 Overplayed*, *🙅 Weird vibe*) that dynamically tune your recommendation penalties.

### 🎯 5. Daily Blind 10 ("Wordle for Music")
- **Pure Intuition Listening**: Mystery tracks with masked titles, artists, and blurred artwork.
- **Streak Tracker**: Test your ear by swiping without visual bias and build daily listening streaks.

### 📥 6. 1-Click Export to Spotify & Apple Music
- **Universal Export**: Transfer all loved tracks into Spotify via direct web intents or download a pre-formatted `.CSV` tracklist ready for TuneMyMusic and SongShift import.

### 🔒 7. Cloud Firestore & Firebase Auth
- **User Accounts**: Email/Password and Google Sign-In with local-to-cloud profile migration.
- **Live Community Feed**: Real-time shared songs with atomic like counters and caption discussions.
- **Security Rules**: Production-grade `firestore.rules` protecting user PII, validating schemas, and securing multiplayer rooms.

---

## 🚀 Live Demo on GitHub Pages

1. Go to repository: `https://github.com/Hootsworth/Spindle`
2. Navigate to **Settings** > **Pages**.
3. Under **Build and deployment** > **Source**, choose **Deploy from a branch**.
4. Select `main` branch and `/ (root)` folder.
5. Live link: `https://hootsworth.github.io/Spindle/`

---

## 🔒 Firebase Configuration

Spindle is connected to Firebase project `spindle-3b452`:
- Authentication: Email/Password & Google Sign-In
- Cloud Firestore: `users`, `posts`, and `rooms` collections
- Security rules configured in `firestore.rules`
