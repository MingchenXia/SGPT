# Update log

Entries are listed newest first. Each future update records its date, a concise description, the affected files or sections, and the verification performed. Multiple updates on the same date may have separate entries; Git history identifies their exact commits.

## 2026-10-04 — Publish the approved revision

- Merged author-approved [PR #1](https://github.com/MingchenXia/SGPT/pull/1) into `main` as `473dba373e1638a825630421dd54e6e8be0c956e`, including the revised Theorem 5.2.2 and the PSWZ26 bibliography entry.
- Published the compiled 545-page book to [SGPT_final.pdf](https://mingchenxia.github.io/Lectures/SGPT_final.pdf) in website commit `e66816291aa70559317d22025275c49ac94e1ca1`. The cover reads `Updated on October 4, 2026.`
- Verification: the merged source tree matches the approved PR head, and all 44 book source files match the successful XeLaTeX build. GitHub Pages completed deployment; the downloaded public PDF matches the local compiled PDF with SHA-256 `0fd575dc57ee9030de2bc6005fc5a8be5e24e8d1ed73d233e400330d503d2e61`.

## 2026-10-04 — State the explicit threshold in Theorem 5.2.2

- Set the exclusion threshold in Theorem 5.2.2 to `1`, removed the separate one-ray assertion and the scaling sentence, and renumbered the former part (3) as part (2). Updated the proof and removed its redundant discussion of the unspecified constant.
- Updated the application in Corollary 5.2.1 to the new part (2), using the potential associated with `kP`. The separating-direction bound now requires `C > Lambda` and remains uniform in `k`.
- Verification: completed two mathematical and editorial reads of the theorem, proof, and affected corollary. Checked that the toric chapter no longer uses `C_0` and no source references the removed item or equation labels. Recompiled the full book with XeLaTeX (545 pages), with no unresolved references, citations, or overfull boxes. Inspected the rendered review excerpt on pages 178–181, including the full theorem and corollary proofs and the subsequent example's integral reference.

## 2026-10-04 — Add the missing PSWZ26 reference

- Added `PSWZ26` to `ComplexGeometry.bib` in the existing preprint format: Kai Pang, Haoyuan Sun, Zhiwei Wang, and Xiangyu Zhou, *Capacity stability of complex Monge–Ampère equations with moving prescribed singularities*, arXiv:2607.12797 (2026). Included a linked arXiv identifier in `howpublished` so that the current BibTeX style displays it.
- Verification: checked the authors, title, year, and primary subject against arXiv, and matched the existing footnote's assertion to Theorem 1.2 (= Theorem 5.1) of version 1. Recompiled the full book with XeLaTeX; there are no unresolved references or citations. Inspected the rendered footnote on page 85 and bibliography entry on page 528.

## 2026-10-04 — Simplify the proof of Theorem 5.2.2

- Replaced the separate boundary-coordinate computations for parts (2) and (3) of Yao's theorem in `author/chapter_toric_ample.tex` by one argument in a smooth toric affine chart. A tube around the given ray reduces nonintegrability to a one-dimensional exponential integral; part (2) is the case of one ray.
- The new proof permits the uniform choice `C_0 = 1`, including after replacing the polytope by any positive integer multiple. Removed the figure and auxiliary estimates used only by the previous proof, and retained the integral formula used by the subsequent example.
- Verification: completed two mathematical and editorial reads of the revised proof, checking the multiplier-ideal reduction, local frame, logarithmic volume factor, tube Jacobian, boundary cases, and scaling. Compiled the full book with XeLaTeX and inspected the rendered review excerpt. The existing undefined citation `PSWZ26` remains; no new unresolved references or citations were introduced.

## 2026-10-04 — Mathematical review workflow

- Updated `AGENTS.md` and `README.md` to require a pull request and a PDF excerpt for every substantive mathematical change. Only explicit author approval permits merging the reviewed version into `main` and publishing its PDF.
- Specified that the update log records only actual changes, and that an instruction to withhold publication takes precedence over the normal release workflow.
- Verification: reviewed the documentation diff and confirmed that all book source files remain unchanged.

## 2026-10-03 — Initial source import

- Imported all 44 supplied book files with their original names, directory structure, and contents: `author/`, `book.tex`, `book2.tex`, `ComplexGeometry.bib`, `images/`, `latexmkrc`, `liesmich.txt`, `mathematical_revision_log.tex`, and `style/`.
- Preserved the existing mathematical revision log unchanged. Its historical revisions predate this repository and are not attributed to the import date.
- Added repository documentation, instructions for recording future updates, and ignore rules for generated TeX files.
- Verification: SHA-256 comparison confirmed that all imported files match the supplied originals. No mathematical edits were made; compilation was not run.
