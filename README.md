# GitHub-facing content

Edit the files in this directory when you update what you publish on GitHub (Pages) or paste into the Chrome Web Store. The extension source code stays in the repository root; this folder is only policies, static HTML, and store listing text.

## Layout

| Path | Use |
|------|-----|
| `index.html` | Optional landing page for your Pages site |
| `privacy-policy.html` | Host on HTTPS; URL goes in the Web Store **Privacy policy** field |
| `PRIVACY_POLICY.md` | Same policy in Markdown (for the repo or your records) |
| `store/LISTING_COPY.md` | Short and long listing text for the dashboard |
| `store/PERMISSION_JUSTIFICATIONS.md` | Permission and host access explanations |
| `store/PRIVACY_PRACTICES_FORM.md` | Draft answers for the privacy practices questionnaire |

`.nojekyll` is present so GitHub Pages does not run Jekyll on these static files.

## Publishing on GitHub Pages

**Option 1 — `/docs` folder (built-in)**  
GitHub can serve from the `docs/` directory on your default branch. After you change `privacy-policy.html` or `index.html` here, copy them into `docs/` in the repo root (replace the existing files) so the live site matches this folder.

**Option 2 — GitHub Actions**  
Add a workflow that uploads this directory to Pages if you prefer not to use `/docs`.

Your privacy policy URL will look like: `https://<user>.github.io/<repo>/privacy-policy.html` when `privacy-policy.html` is at the site root.

## Chrome Web Store

Paste text from `store/`. Use the public HTTPS URL of `privacy-policy.html` in the listing. Icons and screenshots still come from `icons/` and `docs/chrome-store/` in the main project.
