# PromptForge

> Build better AI prompts. Free, open source, no account needed.

A static prompt builder based on Anthropic's official 6-technique prompting framework. Fill in structured fields, get a clean XML-formatted prompt you can copy straight into Claude or any AI tool — with real examples, weak vs strong comparisons, and a live strength meter.

**[Live demo →](https://yourusername.github.io/promptforge)**

---

## What it does

PromptForge has three tabs:

**Build prompt** — A guided form that assembles your prompt in real time as you type. Includes a strength meter (empty → weak → ok → good → strong), a 6-point self-check checklist, technique tags, and one-click copy.

**Example prompts** — 7 pre-built examples across 6 domains (coding, study, writing, business, career, analysis). Filter by domain. Click any card to load it into the builder instantly.

**Weak vs strong** — 6 side-by-side comparisons showing a weak prompt and its strong rewrite, with a diagnosis of exactly which techniques were missing. Load any strong version directly into the builder.

---

## The 6 techniques

Based on [Anthropic's official prompting best practices](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/overview):

| # | Technique | What it means |
|---|-----------|---------------|
| 1 | Role | Who Claude should be — specific, quantified, with defined client types |
| 2 | Task | One specific ask — not six |
| 3 | Context | Your background, level, constraints, and why this matters now |
| 4 | Examples | Show the exact output format you want |
| 5 | Constraints | Length, tone, what to exclude, what bad output looks like |
| 6 | Think first | Ask Claude to reason before answering — for complex or high-stakes tasks |

Minimum viable prompt = Role + Task + Context. Add the others only when the default output will miss.

The tool generates **XML-structured output** — wrapping each section in tags like `<role>`, `<task>`, `<context>`, `<before_answering>`, `<example>`, and `<constraints>` — which Anthropic's docs recommend for cleaner parsing and higher quality responses.

---

## Why it exists

Most people write weak prompts not because they don't know what they want, but because they don't know what information to include. A vague role, no context, no constraints — and the output is generic regardless of how capable the model is.

This tool makes the framework visible and forces the right questions before you send anything.

---

## How to use

No install. No account. No backend. No dependencies.

Open `index.html` in any browser and start building. Or visit the live site.

---

## Deploy your own (5 minutes)

1. Fork this repo
2. Go to **Settings → Pages**
3. Set source: `main` branch, `/ (root)` folder
4. Save — your site is live at `https://yourusername.github.io/promptforge`

GitHub Pages handles everything. No server, no build step.

---

## Stack

- Vanilla HTML, CSS, JavaScript — single file
- Zero npm, zero frameworks, zero dependencies
- Google Fonts: DM Sans + DM Mono
- Works offline once loaded

---

## Prompt examples included

The tool ships with real, domain-specific examples — not generic filler:

- **Coding** — SwiftUI debugging, architecture review
- **Study** — ACCA BT MCQ generation
- **Writing** — TikTok hook scripts for a fashion brand
- **Career** — STAR interview answer preparation
- **Analysis** — Business idea stress-test
- **Business** — 4-week organic content plan

Each example uses the full 6-technique structure and is designed to score 9/10 or above against the framework.

---

## Contributing

PRs welcome. Keep it a single `index.html` file — the zero-dependency constraint is intentional.

Ideas for contributions:
- More domain examples (legal, medical, finance, education)
- Save prompts to localStorage
- Export as `.txt` or `.md`
- Dark mode toggle
- i18n / language support

---

## License

MIT — use it, fork it, ship it.

---

Built with [Anthropic's prompting documentation](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/overview) as the reference standard.
