# IITM Study Notes — Maths, C Programming & ESTC

<p align="center">
  <strong>Structured, visual study notes for IIT Madras BS degree coursework</strong><br>
  Explanations · Worked examples · LaTeX source · Compiled PDFs · External learning resources
</p>

> **Status:** Student-maintained learning resource. These notes supplement—not replace—the official course pages, lectures, assignments, and exam instructions. The notes are syllabus-aligned explanatory material, not verified transcripts of every lecture.

## Contents

| Subject | Source PDF | Editable source | Main topics |
|---|---|---|---|
| Maths for Electronics I (BSMA1101) | [`maths_notes.pdf`](subjects/maths/maths_notes.pdf) | [`maths_notes.tex`](subjects/maths/maths_notes.tex) | Functions, systems of equations, limits, continuity, calculus, series, integration, complex numbers, ODEs |
| Introduction to C Programming (BSCS1101) | [`c_programming_notes.pdf`](subjects/c-programming/c_programming_notes.pdf) | [`c_programming_notes.tex`](subjects/c-programming/c_programming_notes.tex) | Program structure, types, control flow, functions, pointers, arrays, memory, files, debugging |
| ESTC / Computer Systems Design (BSCS3031) | [`estc_notes.pdf`](subjects/estc/estc_notes.pdf) | [`estc_notes.tex`](subjects/estc/estc_notes.tex) | Boolean algebra, logic gates, canonical forms, timing, combinational/sequential logic, FSMs, ISA, ALU, CPU |

## Getting started

### Read the notes online
Open any PDF in the table above. GitHub renders PDF files in the browser. To download a copy, open the PDF and use the download control in GitHub's file viewer.

### Edit the notes
The `.tex` files are the editable LaTeX sources. They include mathematical notation and TikZ/PGFPlots visuals where applicable.

### Compile locally

Install a LaTeX distribution and ensure the `pdflatex` command is on your PATH.

- Windows: [MiKTeX](https://miktex.org/download)
- Cross-platform: [TeX Live](https://www.tug.org/texlive/)
- LaTeX editor: [Overleaf](https://www.overleaf.com/)
- TikZ/PGFPlots reference: [TikZ & PGF manual](https://tikz.dev/) and [PGFPlots manual](https://pgfplots.sourceforge.net/)

From the repository root:

```bash
pdflatex -interaction=nonstopmode -halt-on-error subjects/maths/maths_notes.tex
pdflatex -interaction=nonstopmode -halt-on-error subjects/c-programming/c_programming_notes.tex
pdflatex -interaction=nonstopmode -halt-on-error subjects/estc/estc_notes.tex
```

Depending on how the document sets its output directory, the generated PDFs may appear next to the source or in the current working directory. Replace the committed PDF after reviewing the output.

> Some LaTeX distributions may prompt to install missing packages on first compilation. The notes primarily use common packages including `amsmath`, `amssymb`, `geometry`, `xcolor`, `tikz`, and `pgfplots`.

## Learning workflow

1. Preview a topic before watching the corresponding lecture.
2. Watch the official lecture and note any instructor-specific conventions.
3. Re-derive formulas and solve the worked examples without looking.
4. Attempt the course assignment questions independently.
5. Record mistakes with the concept, mistaken assumption, corrected method, and a follow-up problem.
6. Review difficult topics after one day, one week, and one month.

## Official course pages

These links should be treated as the authority for current course scope, assessments, announcements, and course-specific conventions.

- [Maths for Electronics I — BSMA1101 (IITM)](https://study.iitm.ac.in/ae/course_pages/BSMA1101.html)
- [Introduction to C Programming — BSCS1101 (IITM)](https://study.iitm.ac.in/ae/course_pages/BSCS1101.html)
- [Computer Systems Design — BSCS3031 (IITM)](https://study.iitm.ac.in/ds/course_pages/BSCS3031.html)
- [IITM BS programme academics](https://study.iitm.ac.in/ds/academics.html)

## Recommended external resources

### Mathematics

- [MIT OpenCourseWare — Single Variable Calculus](https://ocw.mit.edu/courses/18-01sc-single-variable-calculus-fall-2010/)
- [Paul's Online Math Notes — Calculus I](https://tutorial.math.lamar.edu/Classes/CalcI/CalcI.aspx)
- [3Blue1Brown — Essence of Calculus](https://www.3blue1brown.com/topics/calculus)
- [OpenStax Calculus Volume 1](https://openstax.org/details/books/calculus-volume-1)

### C programming

- [Beej's Guide to C Programming](https://beej.us/guide/bgc/)
- [cppreference — C language](https://en.cppreference.com/w/c)
- [GNU C manual](https://www.gnu.org/software/c-intro-and-ref/manual/)
- [Compiler Explorer](https://godbolt.org/) — inspect compiler output
- [Compiler warnings and sanitizers (GCC)](https://gcc.gnu.org/onlinedocs/gcc/Warning-Options.html)

### Digital logic and computer systems (ESTC)

- [Nand2Tetris](https://www.nand2tetris.org/)
- [Digital Design and Computer Architecture resources — Harris & Harris](https://pages.hmc.edu/harris/ddca/)
- [CircuitVerse](https://circuitverse.org/) — interactive circuit simulation
- [Logisim-evolution](https://github.com/logisim-evolution/logisim-evolution)
- [RISC-V International — specifications and learning](https://riscv.org/technical/specifications/)

### LaTeX, diagrams, and publishing

- [Overleaf Learn LaTeX](https://www.overleaf.com/learn)
- [TikZ & PGF manual](https://tikz.dev/)
- [PGFPlots](https://pgfplots.sourceforge.net/)
- [GitHub Markdown guide](https://docs.github.com/en/get-started/writing-on-github)

## Build quality and known limits

- The committed PDFs are compiled study-note exports. Recompile after editing the source if you want new changes to appear in the PDF.
- Flowcharts and graphs are authored in LaTeX/TikZ/PGFPlots where included; diagrams should be reviewed at normal reading zoom before release.
- Course references and resource links can change; verify official portal details before relying on them for assessment deadlines or syllabus changes.
- The notes are not a substitute for solving assignments and past assessments yourself.
- Do not upload restricted assessment solutions, copyrighted course handouts, or private material without permission.

## Suggested contribution process

1. Create a branch for a topic or correction.
2. Make a focused change to the relevant `.tex` file.
3. Recompile the PDF and inspect every changed page.
4. Submit a pull request explaining what changed and how the output was checked.
5. Add references for external factual claims and verify all links.

## Repository structure

```text
iitm-study-notes/
├── README.md
├── LICENSE
├── CITATION.cff
├── CONTRIBUTING.md
├── .gitignore
├── subjects/
│   ├── maths/
│   │   ├── maths_notes.tex
│   │   └── maths_notes.pdf
│   ├── c-programming/
│   │   ├── c_programming_notes.tex
│   │   └── c_programming_notes.pdf
│   └── estc/
│       ├── estc_notes.tex
│       └── estc_notes.pdf
└── resources/
    └── README.md
```

## License and attribution

Unless a file header states otherwise, original explanatory prose and LaTeX artwork in this repository are intended to be shared under the MIT License. External course pages, books, videos, logos, and linked resources remain under their respective owners' terms. Do not redistribute external material merely because it is linked here.

Official references:
- Maths source notes: [Notion study guide](https://app.notion.com/p/403a8fc810f681ca96d0e9208f719e6f)
- C source notes: [Notion study guide](https://app.notion.com/p/403a8fc810f681228557d063ea987071)
- ESTC source notes: [Notion study guide](https://app.notion.com/p/403a8fc810f681798376c08924a7ca1b)


## Note on the current edition

The Maths PDF/source is the expanded edition most recently generated in this conversation. C and ESTC are the current generated exports and can be expanded further in future revisions.
