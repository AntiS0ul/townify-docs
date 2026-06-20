# TownifyMC Guide

The official player guide for **TownifyMC**, built with [MkDocs](https://www.mkdocs.org/) and [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/). It publishes to GitHub Pages automatically on every push to `main`.

```
townify-guide/
├── mkdocs.yml                 # Site config: nav, theme, extensions
├── requirements.txt           # Python deps (mkdocs-material)
├── .github/workflows/deploy.yml   # Auto-deploy to GitHub Pages
└── docs/                      # All content lives here (Markdown)
    ├── index.md               # Home page
    ├── getting-started/       # Connecting, first hour, rules
    ├── progression/           # Ranks, economy, jobs, skills, quests
    ├── towns/                 # Towns, nations, war
    ├── money/                 # Earning, shops, fishing
    ├── rewards/               # Voting, crates
    ├── perks/                 # Storage, cosmetics
    ├── reference/             # Commands, FAQ
    └── stylesheets/extra.css  # TownifyMC gold/amber theming
```

## Quick start

### 1. Put it on GitHub

Create a new repository (e.g. `townify-guide`) and push these files:

```bash
git init
git add .
git commit -m "Initial TownifyMC guide"
git branch -M main
git remote add origin https://github.com/<your-username>/townify-guide.git
git push -u origin main
```

### 2. Turn on GitHub Pages

The included workflow (`.github/workflows/deploy.yml`) builds the site and pushes it to a `gh-pages` branch on every push to `main`. To serve it:

1. Push to `main` once (step 1). The **Deploy Guide** action runs automatically — watch it under the repo's **Actions** tab.
2. In the repo, go to **Settings → Pages**.
3. Under **Build and deployment → Source**, choose **Deploy from a branch**.
4. Set the branch to **`gh-pages`** and folder to **`/ (root)`**, then **Save**.

Your guide goes live at `https://<your-username>.github.io/townify-guide/` within a minute or two. Every future `git push` to `main` redeploys it.

> **Note:** the workflow needs permission to push the `gh-pages` branch. If the action fails with a permissions error, go to **Settings → Actions → General → Workflow permissions** and select **Read and write permissions**.

### 3. (Optional) Use a custom subdomain

To serve the guide at `guide.townifymc.xyz` instead of the `github.io` URL — the same way you set up the Dynmap subdomain:

1. Create a file named `CNAME` (no extension) inside `docs/` containing just:
   ```
   guide.townifymc.xyz
   ```
   MkDocs copies files in `docs/` to the site root, so this lands where GitHub Pages expects it.
2. Add a DNS record at your domain provider:
   ```
   CNAME   guide   <your-username>.github.io.
   ```
3. In **Settings → Pages → Custom domain**, enter `guide.townifymc.xyz` and save. Enable **Enforce HTTPS** once the certificate provisions.
4. Uncomment the matching `site_url` line in `mkdocs.yml`.

## Editing the guide

All content is plain Markdown in `docs/`. To change a page, edit its `.md` file. To add a page:

1. Create the `.md` file under the relevant folder in `docs/`.
2. Add it to the `nav:` section of `mkdocs.yml` so it appears in the sidebar.

### Preview locally (optional but recommended)

You don't need this to publish — the GitHub Action builds for you — but it's handy for previewing changes before pushing.

```bash
# Requires Python 3.9+
pip install -r requirements.txt
mkdocs serve
```

Then open <http://127.0.0.1:8000> in your browser. It live-reloads as you edit.

To do a one-off production build into `site/` without serving:

```bash
mkdocs build
```

## Things to finalize before launch

A few values are pulled from the server config but weren't finalized in-game yet. Search the docs for the wrench emoji (:material-wrench: renders as a wrench icon) to find them. The main ones:

- **Vote links** — the vote-site URLs aren't set in `VotingPlugin/Config.yml` yet. Add them so `/vote` shows clickable links, then update `docs/rewards/voting.md`.
- **Discord invite** — replace the placeholder `discord.gg/townifymc` links throughout if your real invite differs.
- **Server address / port** — confirm `play.townifymc.xyz` and the Bedrock port are correct in `docs/getting-started/connecting.md`.
- **Command names** marked with a wrench — a handful of menu/alias commands depend on your exact plugin setup; confirm them in-game.
- **Server rules** (`docs/getting-started/rules.md`) — these are sensible defaults; edit them to match how you actually run the server.

## How this guide stays accurate

The numbers in this guide (rank costs, claim prices, job list, crate names, storage unlocks, etc.) were generated from the live server's plugin configs, so they reflect what's actually on TownifyMC. When you change server values, update the corresponding page so the guide stays in sync.

---

*Built with MkDocs Material. Content © TownifyMC.*
