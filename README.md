# LPL Plugins Repo

This folder is the publishable marketplace feed for the GitHub repository:

- `https://github.com/Boic69/LPL-Plugins`

Recommended layout:

- `official.json`
- `packages/<plugin-id>/<plugin-id>-<version>.zip`

Recommended raw feed URL after push:

- `https://raw.githubusercontent.com/Boic69/LPL-Plugins/main/official.json`

Recommended release strategy:

1. Keep `official.json` in the repo root.
2. Commit versioned plugin zip files under `packages/`.
3. Optionally also upload the same zip files to GitHub Releases.
4. Bump the version in `plugin.toml`, rebuild the package zip, update `official.json`, and push.

The in-client Marketplace can consume this feed directly.
