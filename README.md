# ELIXIR Training Platform Lesson Template Instructions for Zensical

The website is generated with Zensical, with the theme Material.

This website is generated with [Zensical](https://zensical.org), the successor to MkDocs and Material for MkDocs.

Clone this repository, then install the dependencies (a virtual environment is recommended):
```bash
pip install -r requirements.txt
```

Citations (`[@citekey]` and `\full_bibliography`) are pre-rendered into `docs_build/` before Zensical builds, since Zensical has no plugin API yet to do this itself. Always edit source files under `docs/`, never under `docs_build/` (it is regenerated every run and is not committed to git).

To build or preview the site, run the citation renderer first, then Zensical:
```bash
python scripts/render_citations.py
zensical build     # writes the static site to site/
# or
zensical serve     # preview at http://localhost:8000/
```

If you edit a citation or `references.bib` while `zensical serve` is running, stop it (Ctrl+C) and re-run both commands to pick up the change.

Check it out with your browser at http://localhost:8000/.

If using the Github editor

If you commit to the branch main (the default branch), the website will be automatically updated in 30-60 seconds.
