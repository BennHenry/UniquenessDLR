# UniDLR

A collaborative study of uniqueness for the logarithmic
Dobrushin–Lanford–Ruelle (DLR) equations.

The aim is to build a coherent, checked account of the mathematics: what is
known, which arguments work, and which questions remain. This project follows
the approach proposed in Benoît Henry’s essay *The Loss of Singularity*:
shared understanding, contributions in many forms, and the possibility of a
future manuscript under a collective name.

**Status: private research workspace; the mathematical drafts await review.**
The repository setup and a successful LaTeX build do not establish the
correctness of the proofs. See the [review status](docs/STATUS.md) for the
current starting points and known gaps.

## Start here

| Material | Role |
| --- | --- |
| [Latest full draft](<Raw materials/Revised 2/logarithmic_dlr_uniqueness_simplified.tex>) | Starting point for reading the complete argument, including definitions and bibliography. |
| [Existing draft PDF](<Raw materials/Revised 2/logarithmic_dlr_uniqueness_simplified.pdf>) | PDF supplied with that revision; use the build below to regenerate it locally. |
| [main.tex](main.tex) | Active working fragment on the entropy/Fisher-information comparison. It contains an unfinished alternative proof and is not the full manuscript. |
| [Raw materials](<Raw materials/README.md>) | Earlier drafts, revision notes, and patches retained for provenance. |
| [Review status](docs/STATUS.md) | Claims awaiting review, known source issues, and immediate tasks. |
| [Contributing](CONTRIBUTING.md) | How to propose, explain, and check a contribution. |

The supplied full draft studies stationary, simple, unit-intensity point
processes on the line. Its proposed comparison theorem assumes an integrated
number-variance bound; a further argument aims to derive that bound from finite
renormalized logarithmic electric energy. These are the draft’s claims, pending
review here.

## Working principles

- Questions, proofs, counterexamples, reference checks, exposition, and computation
  all contribute to the project.
- AI use is optional. Contributions are assessed through their mathematical
  content and checks. Record useful provenance when it is known.
- Keep established results, proposed arguments, and open gaps distinguishable.
  Cite sources precisely, including the version used when numbering matters.
- Git history records who changed what; it is not a ranking or a claim of
  ownership of a theorem. A collective publication name and acknowledgments
  remain to be discussed with contributors.

## Build locally

With GNU Make, `latexmk`, and a TeX installation containing the packages used
by the sources:

```sh
make manuscript
```

This compiles the latest full draft to
`build/manuscript/logarithmic_dlr_uniqueness_simplified.pdf`.

```sh
make working
```

This attempts to compile `main.tex` to `build/working/main.pdf`. It currently
stops at an existing double-superscript error on line 273. The working fragment
also has unresolved references and duplicate labels, listed in
[the status file](docs/STATUS.md). Neither command uploads files or installs
dependencies.

## Repository access

Any hosted repository must be **private**. Creating it, pushing content,
inviting collaborators, changing settings, or publishing material requires
Benoît’s approval before the online operation. No hosted service or remote is
configured by these project files.

The personal essay `TheLossOfSingularity.pdf` stays local and is excluded from
Git. The mathematical drafts and their supplied PDFs are intended to be
tracked. Generated build files and local credentials are ignored.
