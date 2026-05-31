Editing diagrams

- Diagrams are stored as `.drawio` files under `docs/` (for example `docs/aws-diagram.drawio`).
- Edit them with the desktop app or the web editor at https://app.diagrams.net/; save the updated `.drawio` file back into the `docs/` folder.
- Locally preview changes with:

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
mkdocs serve
```

- When ready, commit and push to the `main` branch. The GitHub Actions workflow will build the site and publish the generated `site/` to the `gh-pages` branch.
- If your default branch is not `main`, update `.github/workflows/deploy-mkdocs.yml` to the branch you use.
