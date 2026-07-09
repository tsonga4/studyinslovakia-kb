# Study in Slovakia — Knowledge Base

Public knowledge base for international students, built with
[Material for MkDocs](https://squidfunk.github.io/mkdocs-material/).
Content lives in Markdown files under `docs/`.

## Edit content

1. Edit or add `.md` files in `docs/`.
2. Add new pages to the `nav:` section of `mkdocs.yml` so they appear in the menu.
3. Commit and push to `main` — GitHub Actions rebuilds and publishes automatically.

## Preview locally

```bash
pip install mkdocs-material
mkdocs serve
```

Then open http://127.0.0.1:8000. The page reloads as you edit.

## How it's published

Pushing to `main` triggers `.github/workflows/deploy.yml`, which builds the site
and deploys it to GitHub Pages. Custom domain: `studyinslovakia.info`.

Search is built in — it indexes every page automatically.
