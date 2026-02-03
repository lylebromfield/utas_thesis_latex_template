# UTAS Thesis LaTeX Template

A LaTeX template for higher-degree research theses at the University of Tasmania. This is a cleaned and generalized version of the earlier IMAS-focused template.

## Origin

Adapted from https://github.com/mdsumner/utas_latex_thesis with general UTAS wording and a slimmer file set. Forked from https://github.com/wghuneke/UTasIMAS_PhDThesis_Template, which slightly tweaked the mdsumner version for IMAS.

## Key files

- `thesis.tex`: main document; controls which component files are included.
- `utasthesis.sty`: layout and formatting (margins, headers/footers, front matter flow).
- `components/prelude.tex`: candidate metadata (title, author, department/college), abstract, acknowledgements, and optional co-authorship statement.

## Typical structure

- `components/newcom.tex`: your custom commands.
- `components/acronym.tex`: list of acronyms.
- `chapters/chapter1/chapter1.tex`, `chapters/chapter2/chapter2.tex`: starter chapter files (copy/rename to add more).
- `components/app0.tex`: switches to appendix mode; add your appendix files after it.
- `components/biby.tex`: bibliography include.
- `components/index.tex`: index include (enable in `thesis.tex` if you need an index).

## Notes

- Edit `components/prelude.tex` to set your department/college and thesis metadata.
- Update or remove the co-authorship section in `components/prelude.tex` as appropriate.
- Replace `logo.png` with an appropriate UTAS/college logo if required.
- `thesis.tex` currently includes chapters/chapter1/chapter1, chapters/chapter2/chapter2, components/app0, components/biby, and components/index; add more includes as you create chapters/appendices, and use `\\includeonly{...}` to speed compilation during drafting.
- Each chapter lives under its own folder in `chapters/` and can keep figures in a per-chapter `figures/` subfolder to avoid clutter.
- Default packages include `acronym`, `natbib`, and `hyperref` (with hidden links).

Happy writing!
