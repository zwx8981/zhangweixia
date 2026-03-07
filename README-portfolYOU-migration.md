# R-PANDA → portfolYOU (Academic Refined Version)

This refined version is tuned to feel more like an academic homepage.

## What changed

- Added a custom **home page** at `pages/index.md`
  - keeps the original landing section from portfolYOU
  - adds a research overview
  - adds selected publications with direct Paper/Code links
  - adds featured GitHub repositories directly on the homepage
- Refined **Publications** into:
  - a highlighted "Selected First-Authored Publications" section
  - a cleaner grouped full list using expandable sections
- Added a dedicated **Code** page at `pages/code.html`
- Reordered the navbar to better match an academic personal site:
  - Publications
  - About
  - Code
- Updated wording across the site to emphasize research, service, and academic visibility

## Files added / updated

- `_config.yml`
- `pages/index.md`
- `pages/about.md`
- `pages/publications.md`
- `pages/code.html`
- `_data/timeline.yml`
- `_data/social-media.yml`

## Still recommended

1. Put your portrait photo at `assets/avatar.jpg`
2. If your repo is not `zwx8981.github.io`, update `_config.yml`:
   - `repository: your-username/your-repo`
   - If you publish from a project repo (for example `https://username.github.io/repo-name/`), also set `baseurl: "/repo-name"`
3. If you want a Chinese/English bilingual homepage later, duplicate the Publications/About pages and add language switching manually.
