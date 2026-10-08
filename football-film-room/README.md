# Football Film Room

A 4-hour crash course in reading football before the snap (8 stations), plus a game-day prediction drill. It's a single static page, so GitHub Pages can host it for free. It installs on a phone's home screen and works offline.

## Put it on GitHub Pages (about 5 minutes, all in the browser)

1. Sign in at github.com, click **+** (top right), then **New repository**.
2. Name it `football-film-room`, set it to **Public**, and click **Create repository**.
   (On a free account, GitHub Pages needs a public repo. The page has no personal data in it; your snaps stay on your device.)
3. On the new repo page, click **uploading an existing file**. Unzip `football-film-room.zip` and drag in **everything inside the folder**: `index.html`, `manifest.webmanifest`, `sw.js`, `.nojekyll`, `README.md` and the `icons` folder. Click **Commit changes**.
   - `.nojekyll` is a hidden file. If your computer hides it, skip it; the site still works without it.
4. Go to **Settings → Pages**. Under **Build and deployment**, set Source to **Deploy from a branch**, Branch to **main** and folder to **/ (root)**, then click **Save**.
5. Wait a minute or two. Your app will be at:
   `https://YOUR-GITHUB-USERNAME.github.io/football-film-room/`

## Install it like an app

- **iPhone (Safari):** open the link, tap **Share**, then **Add to Home Screen**.
- **Android (Chrome):** open the link, tap **⋮**, then **Install app** (or **Add to Home screen**).
- **Desktop Chrome/Edge:** click the install icon at the right end of the address bar.

## Where your data lives

- Games, snaps, quiz answers and station progress are saved **in that browser on that device**.
- **Export backup** (Station 8) downloads a `.json` file of all your games, reviews and plays. **Import backup or review** merges a file back in. Snaps are matched by their timestamp, so importing the same file twice doesn't duplicate anything.
- To move to a new phone: export on the old one, import on the new one.
- Clearing your browser's site data deletes your saved games, so export now and then.

## Getting a game review from Claude

The automatic reviews on the claude.ai version read that page's built-in database, which this GitHub copy can't reach. To get a review here:

1. After the game, tap **Export backup**.
2. Send the file to Claude and ask for a game review of that game.
3. Claude sends back a review file. Tap **Import backup or review** and pick it. The review shows up under the game, and any new plays are added to Station 5.

## Updating the app later

Upload the new `index.html` over the old one (same **Add file → Upload files** button). Also open `sw.js`, change `film-room-v1` to `film-room-v2` (and so on each time), and commit, so installed copies pick up the update the next time they're opened online.
