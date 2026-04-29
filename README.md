# Codex Academic Humanizer

Codex Academic Humanizer is a Codex skill for polishing Chinese and English academic writing while preserving factual meaning, terminology, citations, equations, variables, figure/table references, and argument structure.

It is designed for thesis chapters, journal papers, conference papers, abstracts, introductions, methods, results, discussions, conclusions, and response letters.

## What It Does

- Reduces AI-like phrasing in academic prose.
- Uses a 36-pattern academic AI-writing checklist adapted for paper revision.
- Includes a Chinese-specific 36-pattern checklist for Chinese thesis and journal-paper prose.
- Adds a Chinese academic revision quality checklist for final self-review.
- Supports Chinese, English, and mixed Chinese-English academic text.
- Supports light, medium, and deep revision intensity.
- Can match a target academic writing sample without copying its facts.
- Preserves claims, evidence, hedging, citations, formulas, units, terms, and numbering.
- Produces two outputs by default:
  - a clean revised version ready to paste into the paper
  - a comparison table with brief notes

## What It Does Not Do

- It does not fabricate citations, data, experiments, or conclusions.
- It does not add unsupported literature review content.
- It does not turn formal academic writing into blog-style writing.
- It does not strengthen cautious claims into absolute claims.

## Installation

Clone this repository into your Codex skills directory:

```powershell
git clone https://github.com/YOUR-USER/codex-academic-humanizer.git "$env:USERPROFILE\.codex\skills\codex-academic-humanizer"
```

Or copy this repository folder to:

```text
C:\Users\<you>\.codex\skills\codex-academic-humanizer
```

Restart Codex if the skill is not discovered immediately.

## Usage

Invoke the skill explicitly:

```text
Use $codex-academic-humanizer to polish the following academic paragraph.
Keep all facts, citations, terms, and claim strength unchanged.
```

For Chinese:

```text
用 $codex-academic-humanizer 润色下面这段中文论文内容。
请保留事实、数据、术语、引用和论证结构，并输出直接改写稿与对照说明。
```

For English:

```text
Use $codex-academic-humanizer to revise the following English academic paragraph.
Preserve hedging, citations, terminology, and the original argument structure.
```

With revision intensity:

```text
Use $codex-academic-humanizer in deep mode to revise this introduction.
Do not add claims, citations, or results.
```

With a target style sample:

```text
Use $codex-academic-humanizer to revise the paragraph below.
Match the style of this sample, but do not copy its facts or phrases.
```

## Acknowledgements

This project is inspired by [blader/humanizer](https://github.com/blader/humanizer), an MIT-licensed Claude Code and OpenCode skill for reducing signs of AI-generated writing. It also draws Chinese-language workflow inspiration from [op7418/Humanizer-zh](https://github.com/op7418/Humanizer-zh), especially the idea of quick final checks and quality review. Codex Academic Humanizer adapts these general ideas for Codex and narrows the workflow to academic writing, bilingual Chinese-English paper revision, factual preservation, and dual-output comparison.

## Repository Structure

```text
.
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── chinese-academic-style.md
    ├── chinese-ai-patterns.md
    ├── chinese-revision-quality.md
    ├── english-academic-style.md
    ├── academic-ai-patterns.md
    ├── style-control.md
    └── output-formats.md
```

## License

MIT. See [LICENSE](LICENSE).
