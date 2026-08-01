# Physics of Quantum Error-Correcting Codes with Dipole-Conserving Excitations

**Fractonic Excitations in Dipole-Conserving Hypergraph-Product Codes**

Bachelor's thesis, Department of Applied Physics, Faculty of Science, Tokyo University of Science, 2025  
Author: Sho Nishihara

## PDF

The compiled thesis is available here:

[out/master.pdf](out/master.pdf)

## Directory structure

```
.
├── .gitignore         # Files excluded from Git tracking
├── .latexmkrc         # Build configuration (uplatex + upbibtex; output: out/)
├── readme.md          # This file
├── LICENSE.md         # MIT License
├── master.tex         # Main LaTeX file and parent for subfiles
├── template.sty       # Shared settings and package imports
├── references.bib     # Bibliography
│
├── chapter/           # TeX source files for each chapter
│   ├── 00_preface.tex
│   ├── 01_shor.tex
│   ├── 02_generalized_pauli.tex
│   ├── 03_stabilizer.tex
│   ├── 04_toric_code_qec.tex
│   ├── 05_toric_code_construction.tex
│   ├── 06_toric_code_physics.tex
│   ├── 99_acknowledgements.tex
│   └── figures/       # Figures used in the thesis
│       ├── chap1_*.png
│       ├── chap2_*.png
│       └── chap4_*.png
│
└── out/
    └── master.pdf     # Compiled PDF
```

## LaTeX document structure

`master.tex` is the parent file. It imports the chapter files with `\subfile{}`.

The chapters currently included in the compiled document are:

```
master.tex
├── Preface                              (chapter/00_preface.tex)
├── Table of contents
├── Chapter 1: Shor code                 (chapter/01_shor.tex)
├── Chapter 2: Generalized Pauli operators and qudits
│                                        (chapter/02_generalized_pauli.tex)
├── Chapter 3: Stabilizer formalism      (chapter/03_stabilizer.tex)
├── Chapter 4: Toric-code quantum error correction
│                                        (chapter/04_toric_code_qec.tex)
└── Acknowledgements                     (chapter/99_acknowledgements.tex)
```

The source files `05_toric_code_construction.tex` and `06_toric_code_physics.tex` are present in the repository but are currently commented out in `master.tex` and therefore are not included in the compiled PDF.

## Compilation environment

The following settings are defined in `.latexmkrc`:

- Compiler: `uplatex`
- Bibliography processor: `upbibtex`
- Output directory: `out/` (`out/master.pdf` is generated there)

When using the [LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop) extension in VS Code, `.latexmkrc` is loaded automatically and the document is compiled on save.
