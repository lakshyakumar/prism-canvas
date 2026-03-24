# Contributing to Prism Canvas

Thanks for your interest in contributing. Prism is a lean tool — contributions that keep it sharp and focused are most welcome.

---

## What we welcome

- **New report sections** — additional Lean Canvas parameters, validation frameworks, or research angles that give founders sharper insight
- **Prompt improvements** — better instructions that produce more specific, less generic output
- **Example outputs** — real (anonymised) Prism reports that demonstrate quality
- **Bug fixes** — cases where the skill produces hallucinated data, skips assumption confirmation, or misformats output
- **Platform ports** — adaptations of `PROMPT.md` for specific tools (Perplexity, Gemini, GPT-4o, etc.)

## What we don't want

- Generic prompt padding or filler sections
- Instructions that make output longer without making it sharper
- Breaking changes to the `$ARGUMENTS` / slash command interface without discussion first

---

## How to contribute

1. **Fork** this repo
2. **Create a branch** — use a descriptive name: `feat/add-pricing-section`, `fix/assumption-confirmation-flow`
3. **Make your changes** — edit `prism.md` and/or `PROMPT.md`
4. **Test it** — run the skill or paste the prompt and verify the output is specific, cited, and opinionated
5. **Open a PR** — describe what you changed and why, include a before/after example if the change affects output quality

---

## Testing your changes

**For `prism.md` (Claude Code skill):**
```
cp prism.md ~/.claude/commands/prism.md
```
Then in Claude Code:
```
/prism "I want to build a marketplace for exotic pets targeting hobbyist collectors"
```
Confirm the assumption step fires before any web search begins.

**For `PROMPT.md` (universal prompt):**
Paste the contents into any LLM with web search enabled (ChatGPT, Gemini, Perplexity) and replace `[YOUR IDEA]` with a test idea. Verify it confirms assumptions before researching.

---

## PR checklist

- [ ] Assumption confirmation step is preserved and fires before any research
- [ ] Output remains specific — real company names, real numbers, cited sources
- [ ] No filler, no generic advice
- [ ] Example in the skill still uses the exotic pet marketplace (not a real user's idea)
- [ ] `prism.md` and `PROMPT.md` stay in sync if you change shared logic

---

## Questions

Open an issue or start a GitHub Discussion. Keep it specific — vague "how do I use this" questions are better answered by reading the README.
