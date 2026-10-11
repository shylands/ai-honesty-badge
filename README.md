# AI Honesty Badge

Free AI disclosure badges for your README, website or blog. Say whether your work was made with **no AI**, with **AI assistance**, or **by AI from a brief**.

[![No AI](https://www.aihonestybadge.com/badges/no-ai-large.svg)](https://www.aihonestybadge.com/no-ai-badge) [![AI Assisted](https://www.aihonestybadge.com/badges/ai-assisted-large.svg)](https://www.aihonestybadge.com/ai-assisted-badge) [![AI Generated](https://www.aihonestybadge.com/badges/ai-generated-large.svg)](https://www.aihonestybadge.com/ai-generated-badge)

Pick the one that honestly describes your project, copy the snippet, paste it into your README. That's it.

## The badges

| Badge | Use it when | Page |
|---|---|---|
| ![No AI](https://www.aihonestybadge.com/badges/no-ai-small.svg) | Made by people, start to finish, without AI. | [When to use it](https://www.aihonestybadge.com/no-ai-badge) |
| ![AI Assisted](https://www.aihonestybadge.com/badges/ai-assisted-small.svg) | A person led the work, and AI helped along the way. | [When to use it](https://www.aihonestybadge.com/ai-assisted-badge) |
| ![AI Generated](https://www.aihonestybadge.com/badges/ai-generated-small.svg) | AI made it from a brief, with little shaping by a person. | [When to use it](https://www.aihonestybadge.com/ai-generated-badge) |

Not sure where your project sits? The badge pages have a comparison and some tricky cases, like AI code assistants and AI translation.

## Markdown (READMEs, docs)

**No AI**

```markdown
[![No AI](https://www.aihonestybadge.com/badges/no-ai-small.svg)](https://www.aihonestybadge.com)
```

**AI Assisted**

```markdown
[![AI Assisted](https://www.aihonestybadge.com/badges/ai-assisted-small.svg)](https://www.aihonestybadge.com)
```

**AI Generated**

```markdown
[![AI Generated](https://www.aihonestybadge.com/badges/ai-generated-small.svg)](https://www.aihonestybadge.com)
```

## HTML (websites, blogs, CMSs, and GitHub READMEs)

**No AI**

```html
<a href="https://www.aihonestybadge.com" target="_blank" rel="noopener"><img src="https://www.aihonestybadge.com/badges/no-ai-small.svg" alt="No AI" height="20"></a>
```

**AI Assisted**

```html
<a href="https://www.aihonestybadge.com" target="_blank" rel="noopener"><img src="https://www.aihonestybadge.com/badges/ai-assisted-small.svg" alt="AI Assisted" height="20"></a>
```

**AI Generated**

```html
<a href="https://www.aihonestybadge.com" target="_blank" rel="noopener"><img src="https://www.aihonestybadge.com/badges/ai-generated-small.svg" alt="AI Generated" height="20"></a>
```

## Sizes

Small (`-small`, 20px tall) sits alongside shields.io badges in a README. Large (`-large`, 28px) suits the end of a blog post, a footer or a portfolio. Swap `-small` for `-large` in any snippet, and `height="20"` for `height="28"` in the HTML. One version of each badge works on light and dark pages.

[![No AI](https://www.aihonestybadge.com/badges/no-ai-small.svg)](https://www.aihonestybadge.com) [![AI Assisted](https://www.aihonestybadge.com/badges/ai-assisted-small.svg)](https://www.aihonestybadge.com) [![AI Generated](https://www.aihonestybadge.com/badges/ai-generated-small.svg)](https://www.aihonestybadge.com)

[![No AI](https://www.aihonestybadge.com/badges/no-ai-large.svg)](https://www.aihonestybadge.com) [![AI Assisted](https://www.aihonestybadge.com/badges/ai-assisted-large.svg)](https://www.aihonestybadge.com) [![AI Generated](https://www.aihonestybadge.com/badges/ai-generated-large.svg)](https://www.aihonestybadge.com)

Already using an older badge (`no-ai.svg`, `ai-assisted-dark.svg` and so on)? It keeps working. Swap in the new URL whenever you like.

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

The snippets load the badge from aihonestybadge.com, so there's nothing to install. If you'd rather host it yourself, the SVGs and transparent PNGs are in [`badges/`](badges/): `-small` and `-large` are current, the rest are the older versions. The PNGs are 4× size, for docs, slides and tools that don't take SVG.

## Nobody checks

There's no verification. The badges work like an honesty box: they rely on the people using them to tell the truth. 

## Used by

Game servers, open-source tools, developer blogs and more. See who's on the [AI Honesty Wall](https://www.aihonestybadge.com/#honesty-wall), and [get in touch](mailto:hi@aihonestybadge.com) to be added.

## Licence

[CC0 1.0](LICENSE). Free for any use, including commercial. No attribution required.

---

[![AI Assisted](https://www.aihonestybadge.com/badges/ai-assisted-small.svg)](https://www.aihonestybadge.com/ai-assisted-badge)

AI helped write this README.
