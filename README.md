# Spindle 🎵

> Swipe to find your sound.

Spindle is a web application for music discovery. Swipe through curated song snippets, listen to 30-second previews, train your personalized taste profile, and share your favorite tracks to a real-time community feed.

---

## ✨ Features

- **Swipeable Discover Deck**: Swipe right to love, left to pass. Full support for touch, pointer drag, action buttons, and keyboard arrows (`←` / `→` / `Space`).
- **Vinyl Animation & Previews**: Dynamic spinning vinyl disc animation synchronized with audio previews fetched via the iTunes Search API.
- **Personalized Taste Profile ("For You")**: Tracks your favorite genres, top artists, and decades in real time with taste affinity bars and smart recommendations.
- **Firebase Authentication**: Sign up and log in via Email/Password or one-click Google Sign-In.
- **Cloud Firestore Database**:
  - **User Library Sync**: Preserves loved songs and taste profile across devices in the `users/{userId}` collection.
  - **Live Community Feed**: Global community feed in the `posts/{postId}` collection where listeners share tracks, write captions, and like songs in real-time.
- **Zero Build Step**: Pure modern HTML, CSS, and vanilla ES modules using the Firebase Modular SDK. Works instantly on any static host.

---

## 🚀 Live Demo on GitHub Pages

1. Go to your repository on GitHub: `https://github.com/Hootsworth/Spindle`
2. Navigate to **Settings** > **Pages**.
3. Under **Build and deployment** > **Source**, choose **Deploy from a branch**.
4. Select `main` (or `master`) branch and `/ (root)` folder.
5. Click **Save**. GitHub Pages will deploy your site at `https://hootsworth.github.io/Spindle/`.

---

## 🔒 Firebase Configuration

Spindle is pre-configured with Firebase project `spindle-3b452`:
- Authentication: Email/Password & Google Sign-In
- Cloud Firestore: `users` and `posts` collections
- Security rules defined in `firestore.rules`
