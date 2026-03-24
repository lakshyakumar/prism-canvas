# Prism Canvas

> Full-spectrum market intelligence for founders.

Prism is a Claude Code skill (`/prism`) that takes your startup idea and produces a structured market intelligence report — covering the Lean Canvas, competitor analysis, strategic timing, validation questions, and marketing hooks.

---

## Usage

```
/prism "your idea here"
/prism "your idea here" --extended
```

**Default mode** runs the 9-section Lean Canvas:
Problem · Solution · UVP · Unfair Advantage · Customer Segments · Key Metrics · Channels · Cost Structure · Revenue Streams

**Extended mode** adds 12 more sections:
Why Now · Jobs To Be Done · Riskiest Assumptions · First Customer · Moat · Rising Competitors · Failed Competitors · Market Gap · Mom Test Questions · Marketing Hook · Idea Refinement · Cause Alignment

---

## How it works

1. You provide your idea — the problem you see, your rough solution, and who you think the customer is
2. Prism confirms its understanding of all three before doing any research (no silent assumptions)
3. Once confirmed, it searches the web and produces a sharp, source-backed report

---

## Installation

Copy `prism.md` into your Claude Code commands directory:

```
cp prism.md ~/.claude/commands/prism.md
```

Then use `/prism` in any Claude Code session.

---

## Output format

- Named companies, real funding numbers, real sources
- Opinionated — tells you what matters, not just what exists
- No filler, no generic advice
