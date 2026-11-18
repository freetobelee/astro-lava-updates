# Astro Lava updates

Public update feed for Lee Welsch's [Astro Lava](https://github.com/freetobelee/astro-lava) app (the app repo itself is private).

This repository holds **only**:

- `manifest.json` — current APK and content versions, download URLs, and SHA-256 digests
- `apk/` — signed APKs
- `content/` — content packs (web panel, effect catalog, GLSL shaders)

No source code and no tokens. The Astro app reads this feed over HTTPS on boot and every 6 hours. It never gets a GitHub credential.

**Manifest URLs** (the app tries these in order, then the Pi):

- https://freetobelee.github.io/astro-lava-updates/manifest.json
- https://raw.githubusercontent.com/freetobelee/astro-lava-updates/main/manifest.json

Publish new packs with `scripts/release.sh` in the private app repo.
