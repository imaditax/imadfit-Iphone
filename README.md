# ImadFit iPhone (local version)

This keeps the original simple Bootstrap-style ImadFit interface, but replaces the Flask/SQLite server with browser IndexedDB storage so it can run as an iPhone Home Screen web app. Your old workout history is supplied separately in `PRIVATE-BACKUP/previous-workouts.json`; do not upload that private backup to a public hosting repository. Import it from the Workouts page after installing the app.

## Included
- All 16 original exercises and their exact YouTube URLs
- Includes an optional manual import button for your private workout-history backup
- Exercise Library search, View Exercise and Watch Tutorial buttons
- Add custom exercises, including YouTube tutorial URLs
- Create workouts, add sets, delete sets, delete workouts
- Data stays in this browser on this device; no login, account, or PC sync
- PWA manifest and service worker for offline app shell

## Important
- You must publish this folder to an HTTPS static host (GitHub Pages is free) for iPhone installation.
- Open the hosted link in Safari, tap Share, then Add to Home Screen.
- Open the app once while online so it can cache its files.
- Workout and exercise data are stored only on this iPhone/browser. Clearing Safari website data or deleting the installed app can erase them. Make regular backups; export/import is a sensible next feature.
- YouTube links are saved offline, but playing videos requires internet.
- Bootstrap is loaded from its CDN, so first load requires internet; the app's local files and data work offline after caching, but styling may be less complete if the CDN stylesheet was not cached.
