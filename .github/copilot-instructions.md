## Repo-aware instructions for AI coding agents

This repository documents the "Resonance Architecture Hypothesis" — physics research, LaTeX publications, and source papers assembled by the author. The goal of these instructions is to help an AI coding agent be immediately productive when making documentation, small edits, or helping compile/publish artifacts.

Keep recommendations short and concrete. Only change source files that are clearly documentation (Markdown, README, research/*.md) unless the user explicitly asks you to modify LaTeX sources or PDFs.

Key locations (jump-to):
- `README.md` — overview and high-level links (root: `resonance-architecture/README.md`).
- `SOURCES.md` — canonical citation list and DOIs (root: `resonance-architecture/SOURCES.md`).
- `research/` — analytical markdown documents that explain experiments and physics.
- `papers/` — canonical PDFs and converted HTML (do not edit binary PDFs directly).
- `publications/` — LaTeX sources and archived .tex files (use care when editing; compilation requires typical TeX toolchain).

Big picture architecture and intent
- This is primarily a content/research repo, not an application codebase. The "components" are document collections: hypothesis (THE_CASE.md), deep-dive research, source PDFs, and LaTeX publication material.
- Dataflow is simple and file-based: authors edit markdown and LaTeX sources; compiled PDFs live in `publications/` or `papers/`. Links across files are relative and rely on consistent filenames/capitalization.

Developer workflows & commands (practical examples)
- To produce a PDF from the LaTeX sources in `publications/tex_archive/` use a TeX toolchain (example):

  pdflatex -interaction=nonstopmode letter_to_kyle.tex

  or, for multi-pass bibliography/styles:

  xelatex letter_to_kyle.tex && bibtex letter_to_kyle && xelatex letter_to_kyle.tex && xelatex letter_to_kyle.tex

- There are no automated test frameworks in the repo. For content changes, validate by opening the rendered Markdown or generated PDF.
- Use Git for authoring: small focused commits, descriptive messages, and open a PR for non-trivial edits.

Project-specific conventions
- Filenames are often ALL_CAPS or Title_Case (e.g., `THE_CASE.md`, `DUNN_DRILL_CORE_ANALYSIS.md`). Preserve existing capitalization when linking — relative links are case-sensitive on some systems.
- `SOURCES.md` is the canonical place for bibliographic updates. When adding a new paper, add the PDF to `papers/`, and add the citation (with DOI when available) to `SOURCES.md`.
- Markdown in `research/` is treated as authoritative narrative — prefer minimal structural changes and preserve historical notes and citations.

Integration points & external dependencies
- External: academic papers referenced by DOI and stored (where available) under `papers/`. Do not re-host paywalled PDFs without permission.
- Local: LaTeX style file `resonance-style.sty` under `publications/tex_archive/` is used by TeX sources — if you change the style, recompile affected docs and verify visual layout.

Guidance for automated editing by AI
- Safe edits (no review required): fix typos in Markdown, update README links when the target file is renamed, add cross-references inside `research/`.
- Edits that require human review: any change to LaTeX sources in `publications/`, any change to `SOURCES.md` that alters bibliographic content, and any change that removes or replaces PDFs in `papers/`.
- When summarizing papers, include direct file references (e.g., "See `papers/Luo_2024_Scientific_Reports_Ultrasonic_Friction.pdf`") so humans can verify.

Examples of patterns to follow (copy these when making similar edits)
- Add new paper: put PDF in `papers/`, add short citation + DOI line to `SOURCES.md`, and if relevant, add a short summary paragraph to `research/PHYSICS_DEEP_DIVE.md` with a relative link to the PDF.
- Update the letter: make changes to `publications/letter_to_kyle.tex` and then compile with `xelatex`/`pdflatex` and commit both `.tex` and the generated `.pdf` if requested by the repo owner.

Things to avoid
- Don't modify binary PDFs in-place. Don't change capitalization of files referenced by existing links without updating all references.
- Don't add large external datasets to the repo; instead create a references list in `SOURCES.md` linking to the DOI or external host.

If uncertain, ask: always open a short PR or ask the repository owner (Justin) for confirmation before making structural changes.

---
If anything above is unclear or missing (for example, specific LaTeX toolchain preferences or desired PDF output settings), tell me what to expand and I will iterate.
