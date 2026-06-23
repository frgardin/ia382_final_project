# Claude Code Guidelines for IA382 Final Project

## Overview
This document establishes conventions for editing, refactoring, and writing documentation in the IA382 final project (Privacy and Data Protection in AI Systems).

---

## Writing and Formatting Standards

### Line Length
**Maximum 60 characters per line** in all `.tex` files.

- Break at word boundaries, not mid-word.
- Preserve LaTeX command structure (don't break `\texttt{}`, `\textit{}`, etc. unnecessarily).
- Exception: URLs may exceed 60 characters if breaking would impair readability; prioritize keeping URLs intact.
- Improves diff readability in version control.

### Humanizer Skill for Text Content
**Always apply the `/humanizer` skill** when editing prose sections (methodology, abstract, conclusions).

Key patterns to avoid:
- Em dashes (use commas, semicolons, or restructure instead)
- Rule-of-three lists (break up forced symmetry)
- Copula avoidance ("addressed" → "discussed", "returned" → "produced")
- AI vocabulary words: "Key", "crucial", "landscape", "testament", "showcase"
- Superficial -ing analyses
- Vague attributions without specific sources

Goal: Writing should sound like human documentation, not generated text.

---

## Methodology Section

### Phase Documentation
Each phase (Perplexity, Claude, QuillBot, SlidesAI.io) must document:

1. **Objective**: Clear, one-sentence goal
2. **Configuration/Setup**: Exact settings, parameters, modes used
3. **Output Summary**: What was returned, with specific examples (not fabricated cases)
4. **Real-world examples**: Name actual cases (Clearview AI, OpenAI ChatGPT 2023 breach)
5. **Visual evidence**: Include figures with captions showing actual tool output

### Accuracy Requirements
- No fabricated statistics or case studies
- All referenced incidents must be verifiable
- Citation counts and sources must match actual tool responses
- Dates and technical details must be factually correct

---

## Content Structure

### Abstract
- Concise summary of all four tools and their roles
- What worked, what had limitations
- Reflection on responsible use of multiple AI systems

### Conclusions
- Restate the methodology's alignment with transparency principles
- Reflect on the pipeline's strengths and constraints
- Connect back to Neeli Prasad's call for human-AI collaboration

---

## Before Committing

1. **Line length**: Verify no `.tex` file exceeds 60 characters per line.
2. **Humanizer review**: Run `/humanizer` on any prose changes (methodology, abstract, conclusions).
3. **No em dashes**: Scan for `—`, `--`, or ` — ` patterns. Replace with commas or periods.
4. **Accuracy**: Confirm all technical details, case names, and statistics match source materials.
5. **LaTeX syntax**: Run `pdflatex` or Overleaf compile to ensure no errors.

---

## Git Commit Messages

Format: `scope: brief description`

Examples:
- `docs: reformat methodology to 60-char line limit`
- `style: apply humanizer to abstract and conclusions`
- `fix: update Perplexity results with accurate case data`
- `docs: add figure captions and labels`

Keep messages concise and action-focused.

---

## Tools and References

- **Humanizer skill**: `/humanizer` — removes AI-writing patterns
- **pdflatex**: Compile and verify LaTeX syntax
- **Overleaf**: Web editor for collaborative LaTeX viewing (https://www.overleaf.com/)

---

## Questions or Conflicts?

If a guideline conflicts with project needs, document the exception and the reason in a commit message or PR description.
