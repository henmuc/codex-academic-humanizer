# Contributing

Contributions are welcome when they improve academic revision quality, factual preservation, or Codex skill usability.

## Good Contributions

- Better Chinese or English academic style rules.
- Additional AI-writing detection patterns grounded in real academic editing.
- Safer handling of citations, equations, LaTeX, Markdown, and bilingual terminology.
- Clear examples that show before/after behavior without using copyrighted paper text.

## Guardrails

- Do not add rules that encourage fabricating citations, data, experiments, or conclusions.
- Do not make the skill optimize for bypassing AI detectors.
- Do not add examples copied from unpublished manuscripts or copyrighted papers unless you have permission.
- Keep `SKILL.md` concise. Put detailed guidance in `references/`.

## Validation

Run the Codex skill validation script if available:

```powershell
python C:\Users\<you>\.codex\skills\.system\skill-creator\scripts\quick_validate.py .
```
