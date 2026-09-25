# AI Honesty Badge

Free AI disclosure badges for your README, website or blog. Say whether your work was made with **no AI**, with **AI assistance**, or **mostly by AI**.

[![No AI Badge](https://www.aihonestybadge.com/badges/no-ai.svg)](https://www.aihonestybadge.com/no-ai-badge) [![AI Assisted Badge](https://www.aihonestybadge.com/badges/ai-assisted.svg)](https://www.aihonestybadge.com/ai-assisted-badge) [![AI Generated Badge](https://www.aihonestybadge.com/badges/ai-generated.svg)](https://www.aihonestybadge.com/ai-generated-badge)

Pick the one that honestly describes your project, copy the snippet, paste it into your README. That's it.

## The badges

| Badge | Use it when | Page |
|---|---|---|
| ![No AI](https://www.aihonestybadge.com/badges/no-ai.svg) | Made by people. No generative AI in the words, images or code. | [When to use it](https://www.aihonestybadge.com/no-ai-badge) |
| ![AI Assisted](https://www.aihonestybadge.com/badges/ai-assisted.svg) | A person led the work, and AI helped along the way. | [When to use it](https://www.aihonestybadge.com/ai-assisted-badge) |
| ![AI Generated](https://www.aihonestybadge.com/badges/ai-generated.svg) | AI made most of it, with a person directing and reviewing. | [When to use it](https://www.aihonestybadge.com/ai-generated-badge) |

Not sure where your project sits? The badge pages have a comparison and some tricky cases, like AI code assistants and AI translation.

## Markdown (READMEs, docs)

**No AI**

```markdown
[![No AI Badge](https://www.aihonestybadge.com/badges/no-ai.svg)](https://www.aihonestybadge.com)
```

**AI Assisted**

```markdown
[![AI Assisted Badge](https://www.aihonestybadge.com/badges/ai-assisted.svg)](https://www.aihonestybadge.com)
```

**AI Generated**

```markdown
[![AI Generated Badge](https://www.aihonestybadge.com/badges/ai-generated.svg)](https://www.aihonestybadge.com)
```

## HTML (websites, blogs, CMSs)

**No AI**

```html
<a href="https://www.aihonestybadge.com" target="_blank" rel="noopener"><img src="https://www.aihonestybadge.com/badges/no-ai.svg" alt="No AI Badge" style="max-width: 190px; height: auto;" /></a>
```

**AI Assisted**

```html
<a href="https://www.aihonestybadge.com" target="_blank" rel="noopener"><img src="https://www.aihonestybadge.com/badges/ai-assisted.svg" alt="AI Assisted Badge" style="max-width: 190px; height: auto;" /></a>
```

**AI Generated**

```html
<a href="https://www.aihonestybadge.com" target="_blank" rel="noopener"><img src="https://www.aihonestybadge.com/badges/ai-generated.svg" alt="AI Generated Badge" style="max-width: 190px; height: auto;" /></a>
```

## Let your AI tool add it

If AI helped make the thing you're publishing, the AI knows how much. Let it pick the badge.

**Claude Code:** install the plugin, then ask Claude to "add the AI honesty badge" when you finish a post, README or doc. It chooses from what actually happened in the session, follows your project's existing convention (including frontmatter fields like `ai_badge`), and won't label something it helped write as No AI.

```
/plugin marketplace add shylands/ai-honesty-badge
/plugin install ai-honesty-badge@ai-honesty-badge
```

**Any other agent (Cursor, Codex, Copilot…):** add this to your `AGENTS.md`, `CLAUDE.md` or rules file:

```markdown
When publishing written content (posts, READMEs, docs), add an AI disclosure badge following the rules at https://www.aihonestybadge.com/llms.txt. Choose it from how the content was actually made. Never mark content you drafted or edited as No AI.
```

## Hosting your own copy

The snippets load the badge from aihonestybadge.com, so there's nothing to install. If you'd rather host it yourself, the SVGs and transparent PNGs are in [`badges/`](badges/). The PNGs are 4× size, for docs, slides and tools that don't take SVG.

## Nobody checks

There's no verification. The badges work like an honesty box: they rely on the people using them to tell the truth. Readers generally forgive AI use. What they don't forgive is finding out you hid it.

## Used by

Game servers, open-source tools, developer blogs and more. See who's on the [AI Honesty Wall](https://www.aihonestybadge.com/#honesty-wall), and [get in touch](mailto:hi@aihonestybadge.com) to be added.

## Licence

[CC0 1.0](LICENSE). Free for any use, including commercial. No attribution required.

---

[![AI Assisted Badge](https://www.aihonestybadge.com/badges/ai-assisted.svg)](https://www.aihonestybadge.com/ai-assisted-badge)

AI helped write this README.
