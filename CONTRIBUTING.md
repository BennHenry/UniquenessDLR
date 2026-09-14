# Contributing to UniDLR

The goal is a mathematical account that contributors can understand and check
together. Finding a gap or making an argument easier to read is valuable work.

## Make a contribution reviewable

1. Choose a focused question, correction, or exposition task. The
   [status file](docs/STATUS.md) lists initial tasks.
2. Work on a branch, such as `review/gap-comparison`, and keep related changes
   together. Preserve the supplied drafts in `Raw materials` as the starting
   record; put new explorations in clearly named files under `notes/` or work
   in `main.tex` where appropriate.
3. Explain the statement, its assumptions, and the exact argument or source
   that supports the change. Use LaTeX labels when referring to manuscript
   results; page and theorem numbers can change between revisions.
4. Record what was checked and what remains uncertain. Build the affected
   document locally. A compiled PDF, symbolic calculation, or numerical check
   supports only the aspects it actually checks.
5. When sharing has been authorized, submit the branch for review. Update the
   status file when a check resolves a gap or discovers a new one.

The future maintained full manuscript can be assembled from reviewed work.
The current `main.tex` is a working fragment; do not replace it with an older
full draft and lose its ongoing edits.

## Review records

For a mathematical check, include enough information for someone else to
repeat it. A short note or review comment can use this format:

```text
Claim / source label:
Source version or commit:
Assumptions and dependencies:
Argument or check performed:
Outcome: proposed / checked / gap found / withdrawn
Remaining questions:
Reviewer and date:
```

Use “checked” only with an attached explanation of the check and its scope.
Imported revision notes describe prior work; they do not by themselves count
as a new review of the complete proof.

## Sources and AI assistance

Cite the original mathematical source and the exact result used. Distinguish
what the source proves from any deduction added here. If a reference has not
been checked, say so.

Use AI, or work without it, as you prefer. When known and useful, record the
tool or model, its role, and which parts of its output were checked. Unknown
provenance may be recorded as unknown. There is no need to upload private
conversations; a concise account of the contribution is enough.

Explain the submitted reasoning well enough for another contributor to
evaluate it. Neither human nor AI origin substitutes for checking an argument.

## Credit and publication

Record contributions to preserve context and acknowledge work, including
questions, reviewing, corrections, writing, and computation. Commit counts
and speed of production are not measures of mathematical value. Collective
publication, acknowledgments, and any reuse license remain future decisions.

Keep the hosted project private. Obtain Benoît’s approval before any operation
that changes something online, including a push, issue, pull request,
invitation, settings change, or release.
