# Update log

Entries are listed newest first. Each future update records its date, a concise description, the affected files or sections, and the verification performed. Multiple updates on the same date may have separate entries; Git history identifies their exact commits.

## 2026-10-03 — Initial source import

- Imported all 44 supplied book files with their original names, directory structure, and contents: `author/`, `book.tex`, `book2.tex`, `ComplexGeometry.bib`, `images/`, `latexmkrc`, `liesmich.txt`, `mathematical_revision_log.tex`, and `style/`.
- Preserved the existing mathematical revision log unchanged. Its historical revisions predate this repository and are not attributed to the import date.
- Added repository documentation, instructions for recording future updates, and ignore rules for generated TeX files.
- Verification: SHA-256 comparison confirmed that all imported files match the supplied originals. No mathematical edits were made; compilation was not run.
