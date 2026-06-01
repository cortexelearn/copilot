# CortexEdge — Microsoft 365 Copilot for Aerospace

Deploy to: https://cortexelearn.github.io/copilot/  (repo name: copilot)

This version adds an "All Courses" back link in the sidebar (href="../") so the
PWA can return to the landing page — fixes the standalone dead-end.
Includes the exam phase-normalization fix. Cache: cortexedge-copilot-v3.

## Deploy / redeploy
1. Repo named exactly: copilot
2. Upload CONTENTS (index.html, sw.js, manifest.json, icons/) to repo ROOT.
3. Settings -> Pages -> branch main, / (root).
4. First load: hard-refresh or private window (new cache version).
