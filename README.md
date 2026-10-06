# cardiohaptics.github.io

Public support website for the iOS app **mrmr: cardio haptics**.

Its only purpose is to serve the app's Support URL for Apple App Store Connect.
It is a lightweight static site — plain HTML and CSS, no framework, no build step.

**Public support URL:** <https://cardiohaptics.github.io/>

## Contents

| File | Purpose |
| --- | --- |
| `index.html` | The support page: app description, Support section, FAQ, disclaimer |
| `styles.css` | All styling |
| `favicon.svg` | Site icon |
| `.nojekyll` | Disables Jekyll processing so files are served exactly as committed |
| `.github/workflows/pages.yml` | GitHub Actions workflow that deploys the site |

## How GitHub Pages is configured

This is a **user Pages repository** (named `cardiohaptics.github.io`), so it is published
at the account root: `https://cardiohaptics.github.io/`.

Pages is built with **GitHub Actions**, not the legacy branch-based deploy. In
**Settings → Pages → Build and deployment**, *Source* is set to **GitHub Actions**.

The workflow in `.github/workflows/pages.yml` runs on every push to `main` (and can be
started manually from the Actions tab). It uploads the repository root as the site
artifact and deploys it with `actions/deploy-pages`. There is no build step, so a push
is live within about a minute.

## Making changes

Edit `index.html` or `styles.css`, commit, and push to `main`. The workflow redeploys
automatically.

## Support contact

Support email for the app: cardiohaptics@gmail.com

---

mrmr: cardio haptics is an educational tool and is not intended for medical diagnosis or treatment.
