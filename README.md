# The Lifting Penguin — web app (iPhone + Android)

This is a web app you add to your iPhone's home screen. It opens full screen with its own icon and works offline. Your workout data stays on your phone.

## Files

| File | Purpose |
|---|---|
| `index.html` | The whole app |
| `manifest.webmanifest` | App name, icon, colours for the home screen |
| `sw.js` | Lets the app work offline |
| `*.png` | Penguin icons |

## 1. Put it online (free, with GitHub Pages)

1. On github.com, click **New repository**. Name it `lifting-penguin-app` and set it to **Public**. Free GitHub Pages needs a public repo. Only the app's code is public: your workouts never leave your phone.
2. Click **uploading an existing file**. Drag in `index.html`, `manifest.webmanifest`, `sw.js` and the four `.png` icon files. Click **Commit changes**.
3. Go to **Settings → Pages**. Under "Build and deployment", set **Source** to *Deploy from a branch*, **Branch** to `main`, folder to `/ (root)`, then click **Save**.
4. After a minute or two, the page shows your link, for example `https://husky-penguin.github.io/lifting-penguin-app/`.

## 2. Install it on your iPhone

1. Open the link in **Safari**. Other browsers on iPhone can't install web apps.
2. Tap the **Share** button (the square with an arrow), then **Add to Home Screen**, then **Add**.
3. Always open the app from the penguin icon on your home screen from now on. The home-screen app keeps its own data, separate from Safari.

On Android, open the link in Chrome, tap **⋮** and choose **Add to Home screen** (or **Install app**).

## Backups

Your data lives on the phone only. Use **Home → Export backup** now and then, and save the file to Files or iCloud Drive. **Import backup** restores it, for example on a new phone.

## Updating the app

Upload the changed files to the same repo. Then fully close the app and reopen it (sometimes twice) to get the new version. If you change files, also bump `VERSION` in `sw.js` (e.g. `lp-v2`).

## Tips

- Tap a weight or reps box and the number pad opens. **Next** on the keyboard jumps to the next box.
- Tap a value in the **Previous** column to copy last session's numbers.
- Only ticked sets count towards stats.
- On the Stats screen, **Landscape** shows the chart full screen, sideways. You can also turn the phone sideways if rotation lock is off.
- Tap any point on a chart to see its date and value.
