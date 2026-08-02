# Viam Site

Public landing page for **Viam**, an AI game studio system: a RAG knowledge
base, a simulated multi-agent studio, and a quantitative-data gate that
validates a game idea before anyone spends months building it.

Live at the repo's GitHub Pages URL (see the repository's **About** section
on GitHub for the exact link).

## What this repo is

This repo is marketing and informational content only:

- `index.html`, a single self-contained static page (inline CSS and JS, no
  build step, no external script dependencies beyond the Google Fonts
  stylesheet link).
- `README.md`, this file.

The actual product, the `viam` CLI and the underlying multi-agent orchestration
system, lives in a separate, private repository. Nothing here contains product
source code, API keys, or credentials, and nothing should ever be added here
that does.

## Structure

The page is organized into five sections, reflected in the on-page floating
table of contents:

1. **What Viam is:** the three-layer pitch (RAG knowledge base, multi-agent
   studio, quantitative-data gate).
2. **What's inside:** a closer look at each layer, plus the `viam` CLI.
3. **Origin:** the existing agent tools and Unity AI assistants surveyed
   before writing a line of CLI code, and the gap they leave.
4. **What we didn't build:** deliberately out of scope, and why.
5. **Roadmap:** the three phases from a private internal tool to a
   conditional full-scale product.

## Local preview

No build tooling is required. Open the file directly in a browser:

```bash
start index.html   # Windows
open index.html    # macOS
```

Or serve it locally to test relative paths and fonts exactly as GitHub Pages
would:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Deployment

Deployed via GitHub Pages directly from this repository (no CI workflow, no
build artifacts). Pushing a change to `main` updates the live site once
GitHub Pages picks up the new commit.

## Contributing

Changes here should stay scoped to the public-facing pitch: accuracy of the
claims made about Viam, wording, and visual polish. Product features,
architecture details, or roadmap dates should only be added once they are
true and ready to be public. Do not commit secrets, API keys, analytics
tokens, or personal file paths.
