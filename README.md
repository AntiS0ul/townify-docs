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
    ├── world/                 # Travel, resource world, roads, dungeons
    ├── money/                 # Earning, shops, fishing
    ├── rewards/               # Voting, crates, events & minigames
    ├── perks/                 # Storage, cosmetics, gem store & upgrades
    ├── reference/             # Shortcuts, commands, FAQ
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

### 2. Turn on GitHub Pages — **set the Source to "GitHub Actions"**

This is the step that matters most. The included workflow (`.github/workflows/deploy.yml`) **builds the site with MkDocs and deploys the finished HTML directly** to GitHub Pages.

1. In the repo, go to **Settings → Pages**.
2. Under **Build and deployment → Source**, choose **GitHub Actions**.
   *(Do **not** choose "Deploy from a branch" — that makes GitHub render your raw Markdown with Jekyll, which ignores the Material theme, the sidebar, search, admonitions, and grid cards.)*
3. Push to `main` (step 1). The **Deploy Guide** action runs automatically — watch it under the repo's **Actions** tab. When it finishes, the deploy step prints your live URL.

Your guide goes live at `https://<your-username>.github.io/<repo-name>/` within a minute or two. Every future `git push` to `main` rebuilds and redeploys it.

> **If the action fails with a permissions error,** go to **Settings → Actions → General → Workflow permissions** and make sure Actions are allowed to run. Pages deployment permissions are already declared in the workflow itself.

> **Coming from an older setup?** If you previously set the Pages source to a branch (`main` or `gh-pages`), switch it to **GitHub Actions** now. Serving from a branch is exactly what causes the "no sidebar / no search / raw `!!! note` text" problem — GitHub runs Jekyll on the source instead of serving the MkDocs build.

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

## Keeping things in sync

A few values in the guide come from outside the plugin configs. Update them here if they change:

- **Vote links** — `docs/rewards/voting.md` lists the enabled sites from `VotingPlugin/VoteSites.yml`. Update the table if you add or remove a site.
- **Discord invite** — the guide uses `discord.gg/townify` (the invite the in-game `/discord` command gives). Update it everywhere if that changes.
- **Server address / port** — `play.townifymc.xyz`, default ports (Bedrock `19132`), in `docs/getting-started/connecting.md`.
- **Server rules** (`docs/getting-started/rules.md`) — these mirror the official Townify rules document. When you update the [source doc](https://docs.google.com/document/d/1YOt9tf9FxzV93Trj2E4JNTnDjW_D4fPdZ6XZFjzGWYk/edit?tab=t.0), update this page to match so the two stay in sync.

## How this guide stays accurate

The numbers in this guide (rank costs, claim prices, job list, crate names, storage unlocks, etc.) were generated from the live server's plugin configs, so they reflect what's actually on TownifyMC. When you change server values, update the corresponding page so the guide stays in sync.

---

*Built with MkDocs Material. Content © TownifyMC.*
