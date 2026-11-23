# BudgetCoin releases

Installers are attached to each [release](https://github.com/clearmediaukltd/budgetcoin-releases/releases).

This repo also serves the app's update check through GitHub Pages:

- `versions.json`: the newest release of each major version, e.g. `{"versions": ["1.4.2", "2.0.1"]}`. The app compares it with its own version and offers the download page when a newer one is out. Update it when you publish a release.
- `index.html` and `de/`, `fr/`, `es/`, `it/`, `nl/`, `pt/`: the website, generated from `website/` in the main repo by `node website/build.mjs --help` (which also copies the user guide into `help/`). Don't edit these files here. The app's update notice opens the home page.

The app reads `https://getbudgetcoin.com/versions.json`; `getbudgetcoin.com` is this site's custom domain (the `CNAME` file). Keep that domain pointing at whichever host serves this file.
