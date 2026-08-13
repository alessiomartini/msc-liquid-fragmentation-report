# Liquid Fragmentation — Hydrodynamics Group Report (UvA, 2025)

LaTeX source of a group report on **liquid fragmentation**, written for the
*Hydrodynamics* course of the MSc in Physics, University of Amsterdam, February
2025, by **Tommaso, Martina and Alessio**.

> **Status: unfinished draft.** Only the Introduction and Chapter 1 contain
> text. `Chapter2.tex`, `Chapter3.tex` and `Conclusions.tex` exist but are
> empty files, and the Introduction still carries its "The second section…" /
> "The third section…" placeholders. The repository is a single Overleaf import
> that was never completed; it is kept as a record of the work that was done.

## What the report is about

Liquid fragmentation is the transition from a macroscopic volume of liquid to a
dispersion of stable droplets. Instabilities in the liquid grow into corrugated
**ligaments**, which then break up into droplets of a wide range of sizes. The
process is everywhere, in industry and in nature: combustion engines,
electro-sprayed paint, cosmetics, ink-jet printers, volcanic eruptions, rain and
tephra formation.

The question the report is organised around is not *whether* a liquid breaks up,
but **what sets the resulting distribution of droplet sizes**.

### Chapter 1 — Theoretical models for fragmentation *(written)*

The only substantive chapter. It works through:

- **The bag breakup mode**, as a concrete worked example of a drop falling in a
  quiescent medium — its *deformation* under aerodynamic pressure, the *bag
  breakup* itself, and the resulting *distribution of fragments*.
- **Models for the size distribution**, three families of them, each producing a
  different characteristic law:
  - *sequential cascade of breakups* — a drop splits, the fragments split again,
    and the distribution is the fixed point of that cascade;
  - *aggregation scenarii* — the mirror-image picture, in which fragments
    coalesce;
  - *the maximum entropy principle and random breakups* — the distribution as
    the least-committed one consistent with the conserved quantities.

### Chapters 2–3 and Conclusions *(empty)*

Planned as: ligaments and drop formation (Chapter 2), applications (Chapter 3),
and conclusions. The files are committed but contain only their `\chapter{}`
line.

## Repository layout

```
main.tex           Master file (report class), \input order, biblatex setup
Introduction.tex   Written
Chapter1.tex       Written — theoretical models for fragmentation
Chapter2.tex       Empty — ligaments and drop formation
Chapter3.tex       Empty — applications
Conclusions.tex    Empty
bibliography.bib   References (Villermaux 2007 and others)
```

## Building

`biblatex` with the **biber** backend and the `phys` style, on a plain `report`
class — pdfLaTeX is fine:

```bash
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```

## Related repository

- [`hydrodynamics_2025_msc_course`](https://github.com/alessiomartini/hydrodynamics_2025_msc_course)
  — the numerical homework notebooks for the same course.
