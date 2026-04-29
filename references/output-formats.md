# Output Formats

## Default Dual Output

Always provide two deliverables unless the user asks otherwise:

1. A clean revised version that can be pasted into the paper.
2. A comparison version with brief notes.

For Chinese tasks:

```markdown
## 直接改写稿

...

## 对照版与简短说明

| 原文 | 改写 | 说明 |
|---|---|---|
| ... | ... | ... |
```

For English tasks:

```markdown
## Revised Version

...

## Comparison and Notes

| Original | Revised | Notes |
|---|---|---|
| ... | ... | ... |
```

## Notes Style

- Keep notes short and substantive.
- Mention changes to claim strength, cohesion, sentence structure, terminology consistency, or academic tone.
- Do not list routine grammar corrections unless they affect meaning.
- If a sentence is unchanged, omit it from the comparison unless the user requested exhaustive comparison.

## Long Documents

For long papers or sections:

- Process by heading or paragraph group.
- Maintain a terminology list internally.
- Keep citation style, numbering, and section labels unchanged.
- If the full dual output would be too long, provide the clean revised version first and then a representative or section-by-section comparison.
- Tell the user when comparison is partial because of length constraints.

## Risk Flags

Flag issues in notes instead of silently fixing them when:

- A term is used inconsistently in the source.
- A citation appears to support an unclear or mismatched claim.
- A result sentence lacks the data needed to support a strong conclusion.
- A Chinese-English mixed term may have multiple accepted translations.
