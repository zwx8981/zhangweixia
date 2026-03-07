# R-PANDA → portfolYOU migration draft

This folder contains a first-pass migration of the public content from the Google Site below into a structure that fits **portfolYOU**:

- Source site: https://sites.google.com/view/r-panda/home
- Theme docs: https://yousinix.github.io/portfolYOU/docs/

## Files included

- `_config.yml` — homepage text, social links, nav exclusions
- `_data/social-media.yml` — adds Google Scholar and ResearchGate icons
- `_data/timeline.yml` — education and career timeline
- `pages/about.md` — biography, interests, funding, service, talks
- `pages/publications.md` — publication list converted into markdown

## What to do next

1. Copy these files into your `portfolYOU` repository.
2. Put your profile photo at `assets/avatar.jpg`.
3. If your repo is not `zwx8981.github.io`, update the `repository:` line in `_config.yml`.
4. Optionally add a `pages/projects.html` page later if you want to showcase selected GitHub repos as projects.
5. Optionally add PDF / code links back into `pages/publications.md` for the strongest parity with the original Google Site.
