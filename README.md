# Prism Canvas

> Full-spectrum market intelligence for founders.

Prism is a Claude Code skill (`/prism`) that takes your startup idea and produces a structured market intelligence report — covering the Lean Canvas, competitor analysis, strategic timing, validation questions, and marketing hooks.

---

## Installation

**1. Copy the skill into your Claude Code commands directory:**

```bash
cp prism.md ~/.claude/commands/prism.md
```

**2. Restart Claude Code.**

> The app does not pick up new commands until it is restarted. If `/prism` does nothing or is not recognised, restart Claude Code and try again.

---

## Usage

**Desktop app (Claude Code GUI)** — type directly, no quotes needed:
```
/prism your idea here
/prism your idea here --extended
```

**Terminal (CLI)** — wrap your idea in quotes to avoid shell issues:
```bash
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

## Don't have Claude Code?

Use `PROMPT.md` — paste it into any LLM with web search (ChatGPT, Gemini, Perplexity, Claude.ai) and replace `[YOUR IDEA]` with your idea.

---

## Output format

- Named companies, real funding numbers, real sources
- Opinionated — tells you what matters, not just what exists
- No filler, no generic advice
