---
name: codex-academic-humanizer
description: Polish and humanize Chinese or English academic writing while preserving factual meaning, terminology, citations, equations, variables, figure/table references, and argument structure. Use when Codex needs to revise thesis, journal paper, conference paper, abstract, introduction, method, results, discussion, response letter, or other scholarly text to reduce AI-like phrasing, improve academic readability, and output both a clean revised version and a paragraph-by-paragraph comparison with brief notes.
---

# Codex Academic Humanizer

## Purpose

Revise academic prose so it reads like careful human scholarly writing, not generic AI output. Preserve the author's claims, evidence, scope, uncertainty, technical terms, and citation intent.

This skill is for style, clarity, and academic naturalness. It is not for adding new research content, fabricating citations, changing results, or strengthening claims beyond the source.

## Operating Rules

- Preserve all facts, data, citations, formulas, variables, units, figure/table numbers, section references, dataset names, model names, and domain terms.
- Do not add literature, examples, mechanisms, limitations, conclusions, or numerical results unless they are explicitly present in the source or the user asks for content development.
- Keep the paper's disciplinary register. Do not make formal academic writing sound like a blog, speech, product pitch, or popular science article.
- Maintain hedging and uncertainty. Do not turn "may", "suggests", "is associated with", or "under the tested conditions" into absolute claims.
- Keep paragraph functions intact unless the user asks for restructuring. Preserve the role of background, gap, method, result, interpretation, and limitation paragraphs.
- If the source is ambiguous or internally inconsistent, flag the issue in the comparison notes instead of silently resolving it by invention.
- For long inputs, process by section and keep a running terminology list so wording stays consistent.

## Workflow

1. Identify the mode:
   - Use Chinese mode for Chinese academic prose.
   - Use English mode for English academic prose.
   - Use mixed mode when the text includes both; preserve each language's academic conventions.
2. Identify the section type if possible: abstract, introduction, related work, method, experiment, results, discussion, conclusion, or response letter.
3. Diagnose AI-like features before revising:
   - Template transitions and stock phrases.
   - Repeated sentence rhythm.
   - Vague intensifiers or empty evaluative language.
   - Mechanical listing without argumentative flow.
   - Overly polished but underspecified sentences.
4. Revise for academic naturalness:
   - Make sentence structure varied but controlled.
   - Replace generic claims with precise formulations grounded in the source.
   - Improve cohesion between sentences without adding unsupported content.
   - Keep terminology stable and avoid needless synonym rotation for technical terms.
5. Self-check the revision:
   - Compare claims against the original.
   - Check that no new fact, citation, data point, or causal relation was introduced.
   - Check that hedging, conditions, and limitations remain present.
   - Check that the style is academic, not casual.
6. Output both required deliverables unless the user requests a different format:
   - Direct revised version.
   - Comparison version with original, revised text, and brief notes.

## Language References

Read the relevant reference only when needed:

- For Chinese academic prose, use `references/chinese-academic-style.md`.
- For English academic prose, use `references/english-academic-style.md`.
- For output structure and long-document handling, use `references/output-formats.md`.

## Default Output

Use this structure by default:

```markdown
## 直接改写稿

[Revised text ready to paste into the paper.]

## 对照版与简短说明

| 原文 | 改写 | 说明 |
|---|---|---|
| ... | ... | ... |
```

For English-only user requests, use English headings:

```markdown
## Revised Version

[Revised text ready to paste into the paper.]

## Comparison and Notes

| Original | Revised | Notes |
|---|---|---|
| ... | ... | ... |
```

Keep notes concise. Explain material style, precision, cohesion, or claim-scope changes; do not annotate every small grammar edit.
