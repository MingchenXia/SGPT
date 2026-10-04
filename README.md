# SGPT

LaTeX sources for **Singularities in global pluripotential theory — Lectures at Zhejiang University**, by Mingchen Xia.

The initial import preserves all 44 supplied files byte for byte, including the existing mathematical revision log.

## Source files

- `book.tex`: main book.
- `book2.tex`: alternative main file that suppresses chapter mottos after the acknowledgements.
- `author/`: chapters, appendices, front matter, and bibliography setup.
- `ComplexGeometry.bib`: bibliography database.
- `images/`: supplied image assets.
- `style/`: document class, bibliography styles, and index styles.
- `latexmkrc`: supplied build configuration.
- `liesmich.txt`: supplied SVMono documentation.
- `mathematical_revision_log.tex`: existing account of substantive mathematical revisions.

## Building

With a TeX distribution and `latexmk` installed, run from the repository root:

```sh
latexmk -pdf book.tex
```

Use `latexmk -pdf book2.tex` for the alternative version. The supplied `latexmkrc` sets the paths for the bundled styles and configures the index. Compilation has not been verified as part of the source import.

## Updates

Git commits retain the exact file history. [CHANGELOG.md](CHANGELOG.md) records dated summaries of updates, with the affected files or sections and the verification performed. The supplied [mathematical revision log](mathematical_revision_log.tex) remains the detailed historical account of mathematical revisions.

Updates are made when the author requests them or supplies revised files. There is no scheduled folder monitoring or automatic publication. Future assistant sessions should follow [AGENTS.md](AGENTS.md) and update the changelog alongside book changes.

Every substantive mathematical change is proposed through a pull request and accompanied by a PDF excerpt of the modified passages for the author to review. The proposal branch may be committed and pushed to open the PR. Merging into `main` and publishing the revised book require the author's explicit approval of that version. The update log records only actual changes.
