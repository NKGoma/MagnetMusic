# Norster 🎵

A Hitster-style music timeline party game that uses **your own Spotify playlists**.

## How to play

1. Open the app and connect with Spotify
2. Pick any playlist from your library
3. Enter player names
4. The app plays a random song through your Spotify app — without showing what it is
5. Each player decides where the song fits on their timeline (use the physical metal strips + tokens)
6. Press **Reveal** to see the year, title, and artist
7. Press **Correct** or **Wrong** — then it's the next player's turn
8. First to 10 correct songs wins and becomes the **Norster**!

---

## One-time setup (takes 5 minutes)

You need a free Spotify Developer **Client ID**. Here's how:

### Step 1 — Create a Spotify Developer app

1. Go to **[developer.spotify.com](https://developer.spotify.com)** and log in with your **normal Spotify account**
2. Click **Create app**
3. Fill in:
   - **App name:** Norster (or anything you like)
   - **App description:** My music game
   - **Redirect URI:** paste your GitHub Pages URL — e.g. `https://YOUR-USERNAME.github.io/MagnetMusic/`
   - **APIs used:** tick **Web API**
4. Click **Save**
5. On the next screen, click **Settings** — you'll see your **Client ID** — copy it

### Step 2 — Add your Client ID to the app

1. Open `index.html` in any text editor
2. Find this line near the top of the `<script>` section:
   ```
   const CLIENT_ID = 'YOUR_CLIENT_ID_HERE';
   ```
3. Replace `YOUR_CLIENT_ID_HERE` with your real Client ID (keep the quotes)
4. Save the file

### Step 3 — Deploy to GitHub Pages

1. Push the updated `index.html` to your repo
2. Go to your repo on GitHub → **Settings** → **Pages**
3. Set source to **main branch / root folder**
4. Your app is live at `https://YOUR-USERNAME.github.io/MagnetMusic/`

---

## Requirements

- **Spotify Premium** — required for playback control via the Spotify API
- A modern browser (Chrome, Firefox, Safari, Edge)
- Spotify open on any device (laptop, phone, etc.) before playing

## How the tokens work

Each player gets **3 tokens** (tracked in the app). Use them however you agree as a group — e.g.:
- Skip a song and get a new one
- Challenge another player's placement
- Get a hint

## Difficulty modes

You can agree on a difficulty before starting:
- **Easy:** just place the song in order on your timeline
- **Medium:** also name the artist and title
- **Hard:** guess the exact year too — get a bonus token if correct!

---

Built with plain HTML/CSS/JS + Spotify Web API (PKCE flow). No backend, no framework.
