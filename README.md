# Take Log

An offline take sheet for tracking sessions. Songs hold part tabs (Drums, Bass, Guitar, Piano, Vocals to start, all renameable), and each part is a grid of song sections × takes. Built for an iPad on the desk, and it works with no internet.

## Put it online once (GitHub Pages, free)

You only need internet for this setup step and for later updates.

1. Go to **github.com/new**. Name the repository `take-log`, set it to **Public**, and click **Create repository**.
   (Free GitHub Pages needs a public repo. Only the app's code is public. Your take data never leaves the iPad.)
2. On the new repo page, click **uploading an existing file**. Drag in all six files from this folder:
   `index.html`, `sw.js`, `manifest.webmanifest`, `icon-192.png`, `icon-512.png`, `apple-touch-icon.png`.
   Click **Commit changes**.
3. Go to **Settings → Pages**. Under *Build and deployment*, set **Source** to *Deploy from a branch*, then pick **main** and **/(root)**. Click **Save**.
4. Wait about a minute and refresh that page. It shows your link, something like
   `https://YOUR-USERNAME.github.io/take-log/`

## Install on the iPad

1. Open the link in **Safari** (it has to be Safari for Add to Home Screen).
2. Tap **Share → Add to Home Screen → Add**.
3. Open it once from the home screen while you still have wifi. That saves a copy on the iPad.
4. Test it: turn on Airplane Mode and open Take Log. It should load normally.

## Using it

- **Songs** (top right): switch, add, reorder or delete songs, plus backups.
- **Tabs**: Overview first, then one per part. **+ Add part** makes a new one; type over the name to rename it. **Part options** moves or deletes it.
- **Sections**: built once per song and shared by every part. Use **+ Section** for common names or type any name. Repeats number themselves (Verse 1, Verse 2). The **⋯** on a section lets you move it, split it into lines, mark it *Not in this part*, or delete it.
- **Split into lines**: paste a section's lyrics and each line becomes its own row. This works on any part, not only vocals.
- **Marking**: pick a mark (★ Keeper, ✓ Good, ✎ Punch / edit, ? Relook, ✕ Bad), then tap cells. Tapping the same mark again clears it. **Undo** reverses the last change.
- **Overview**: every part against every section. `T3` is the keeper take, `2/4` means lines with a keeper, `open` means marked but no keeper yet, and `—` means not in this part.
- **Keyboard** (if you use one): 1–5 pick a mark, 0 erases, T adds a take, ⌘Z undoes.

## Backups (important)

Everything is stored on the iPad only. If you delete the app from the home screen, its data goes with it.

- At the end of a session, open **Songs → Export all songs**. The share sheet opens, so you can **AirDrop** the file to the tracking Mac and drop it in the session folder. AirDrop works without wifi.
- **Import file** brings a backup back in. It adds songs and replaces any with the same ID, so importing the same backup twice is safe.

## Updating the app later

Upload the new `index.html` (and any other changed files) to the same repo. Open the app twice while online: the first launch downloads the update in the background, and the second launch runs it. Your data isn't touched.
