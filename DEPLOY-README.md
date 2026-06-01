# CortexEdge — Microsoft 365 Copilot for Aerospace (standalone track)

Standalone PWA for deployment to: https://cortexelearn.github.io/copilot/

## Build notes
- Full v43 CortexEdge app, locked to the COPILOT track (currentTrack = "copilot").
- Track-switcher UI hidden; saved-track restore disabled so it always stays on COPILOT.
- Cache: cortexedge-copilot-v1 (unique per track, no collisions).
- All paths relative (./), works under the /copilot/ subpath.

## Deploy
1. Create GitHub repo named exactly: copilot
2. Upload the CONTENTS of this folder (index.html, sw.js, manifest.json, icons/) to the repo ROOT.
   Do NOT upload the .zip itself — GitHub Pages does not unzip.
3. Settings -> Pages -> Deploy from branch: main, folder / (root).
4. Open https://cortexelearn.github.io/copilot/ (wait ~1 min for first build).

## First load
Hard-refresh or use a private window the first time so an old service worker
isn't serving cached content. On future updates, bump the cache version in sw.js.

## Smoke test
- [ ] Title shows "Microsoft 365 Copilot for Aerospace"
- [ ] Correct lessons in sidebar, NO track switcher
- [ ] Final exam loads questions (25-question attempt from the 53-pool)
- [ ] Quizzes score; install + offline works; progress persists
