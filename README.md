# Spindle 🎵

> Swipe to find your sound.

Spindle is an interactive, full-stack music discovery web application combining tactile physical metaphors (spinning vinyl, DJ scratching, card gestures) with algorithmic taste matching, multiplayer listening rooms, real-time social sharing, internal DMs & group chats, and complete user profile customization.

---

## ✨ Features & Innovations

### 💬 1. Internal DMs & Group Chat (with Song Attachments)
- **1-on-1 Direct Messaging**: Start a conversation with any listener by email or handle.
- **Group Listening Circles**: Create named groups (e.g. *Late Night Vinyl Club 🌙*) with member management.
- **Embedded Song Attachments**: Drop loved songs directly into chat bubbles with inline **Play/Pause** preview buttons so friends can listen together.
- **Real-Time Delivery**: Subcollection architecture (`chats/{chatId}/messages`) powered by Cloud Firestore.

### 📰 2. 100% Real Community Feed (Zero Dummy Data)
- **In-App Post Composer**: Share what you're spinning right now, attach any track from your library, and write thoughts/captions.
- **Real-Time Live Updates**: Instant global updates via Firestore `posts` collection.
- **Interactive Discussion**: Full comment threads on every post with author handles and timestamps.
- **Feed Filtering**: Toggle between **All Community** and **My Posts**.

### 👤 3. Accounts Page & Profile Customization
- **User Identity**: Custom display name, `@handle`, bio, and avatar emoji selector (`🎧`, `🎵`, `⚡`, `🌙`, `🔥`, `💿`).
- **Listening Stats**: Tracks total loved tracks, passed count, artists discovered, and daily streak.
- **Post Management**: View and manage all community feed posts authored by your account.
- **Genre DNA**: Breakdown of top listening genre affinities.

### ⚙️ 4. Settings & Theme Customization
- **Audio Experience**: Toggle DJ vinyl scratching sounds, tape-stop slowdown, and autoplay previews.
- **Visual Themes**: Switch between **Deep Ink (Default)**, **Midnight AMOLED**, and **Cyber Neon**.
- **Data & History**: Clear local swipe cache, export taste data, and manage account authentication.

### 🎧 5. Sensory & Vinyl Audio (Web Audio API)
- **Interactive Vinyl Scratching**: Touch and scrub the vinyl record sticking out of the card to dynamically modulate audio playback rate and trigger synthesized analog needle scratch sound effects.
- **Pull-Down Tape Stop**: Dragging down on any card produces an authentic decelerating tape-stop pitch drop effect before springing back.
- **⚡ Drop Jump**: Instant chorus/drop seek button that skips right into the track's peak energy segment.
- **Beat-Reactive Ambient Background**: An `AnalyserNode` frequency pipeline pulses the background glow and ripples the vinyl grooves in sync with real-time bass frequencies.

### 👥 6. Spindle Blend (Multiplayer Match Room)
- **Tinder for Music**: Create a room to get a 6-digit code (e.g., `SPIN84`), or join a friend's room.
- **Synchronized Deck**: Both players swipe through the exact same 10 tracks with live real-time progress indicators.
- **Compatibility Reveal**: An animated score gauge reveals your taste compatibility percentage (e.g. *82% Taste Match!*) and lists mutual favorites with a 1-click **Save All to Library** button.

### 🧬 7. Generative Sound Aura (Music DNA Card)
- **Canvas-Powered Visual Identity**: Generates a high-res, shareable visual card blending radiant radial gradient auras matched to your top listening genres.
- **Aura Archetypes**: Assigns your taste profile an archetype (e.g. *The Midnight Dreamer*, *The Electric Nomad*, *The Sunset Optimist*).
- **1-Click Download & Social Share**: Export to PNG or trigger native Web Share for Instagram Stories / TikTok / Twitter.

### 🧭 8. Dynamic Discovery: Vibe Radar & Time Machine
- **2D Vibe Radar Pad**: Interactive coordinate pad allowing you to drag a puck across two axes (*Chill ⟷ Hype* and *Vintage ⟷ Modern*) to steer recommendations.
- **Time Machine Decades Bar**: Filter your feed across eras (*70s Classics*, *80s Retro*, *90s Golden*, *2000s Y2K*, *2010s Hits*, *2020s Modern*).
- **Pass Roasting**: Swiping left prompts quick roast badges (*😴 Too slow*, *📢 Overproduced*, *🔁 Overplayed*, *🙅 Weird vibe*) that dynamically tune your recommendation penalties.

### 🎯 9. Daily Blind 10 ("Wordle for Music")
- **Pure Intuition Listening**: Mystery tracks with masked titles, artists, and blurred artwork.
- **Streak Tracker**: Test your ear by swiping without visual bias and build daily listening streaks.

### 📥 10. 1-Click Export to Spotify & Apple Music
- **Universal Export**: Transfer all loved tracks into Spotify via direct web intents or download a pre-formatted `.CSV` tracklist ready for TuneMyMusic and SongShift import.

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
- Cloud Firestore: `users`, `posts`, `chats`, `chats/{chatId}/messages`, and `rooms` collections
- Production-grade security rules configured in `firestore.rules`
