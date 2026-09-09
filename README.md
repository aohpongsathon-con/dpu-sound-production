# dpu-sound-production
Faculty of Communication Arts, Dhurakij Pundit University

## Project files

- `sound-production-spa-fixed.html`: editable source, using relative assets.
- `index.html`: published entry point; keep identical to the fixed version.
- `sound-production-spa-embedded-assets.html`: standalone version; update alongside the fixed version, preserving embedded data URLs.
- `assets/`: required images, fonts and scripts.

Open the HTML in a browser. Keep the complete folder together; its location and drive can differ between computers.

## Switch computers

Install Git and authenticate with a GitHub account with write access. Clone once:

```sh
git clone https://github.com/aohpongsathon-con/dpu-sound-production.git
cd dpu-sound-production
```

Before editing on either computer:

```sh
git status
git pull --ff-only
```

After editing both HTML variants, synchronize the entry point and review before committing:

```powershell
Copy-Item sound-production-spa-fixed.html index.html
git diff --stat
git add --all
git commit -m "Describe the change"
git push
git status
```

Ensure push succeeds before switching. Pull on the other machine before editing. If pull reports local changes or divergent history, preserve and reconcile them; do not reset or force-push.

## Continuing development

The latest Tier List contains sound equipment only. Maintain both HTML variants together. Use relative paths in the fixed version and retain embedded assets in the standalone version. Give a new coding session this repository folder and README.

Git transfers committed files, not chat history, installed programs or browser storage. Export saved Diagram data separately if needed using available application export controls. Never commit credentials, personal exports or temporary files.

Pushing may trigger the repository's existing GitHub Pages deployment.
