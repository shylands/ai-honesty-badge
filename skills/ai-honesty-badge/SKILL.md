---
name: ai-honesty-badge
description: Adds an honest AI disclosure badge (No AI, AI Assisted or AI Generated, from aihonestybadge.com) to written work such as blog posts, READMEs, docs, articles and release notes, choosing the badge from what actually happened in the session. Use when the user asks to add an AI badge, AI disclosure or "AI honesty badge", asks which badge fits, says /ai-honesty-badge, or finishes a piece of content in a project that already uses aihonestybadge.com badges or an ai_badge-style frontmatter field.
metadata:
  author: "Steven Hylands"
  version: "1.0.0"
  homepage: "https://www.aihonestybadge.com"
---

# AI Honesty Badge

Label a piece of work with how much AI went into it. You're usually the AI in question, so you have first-hand evidence. Use it.

The badges only work because people are honest with them. Nobody verifies them. That makes accuracy your job.

## 1. Decide the badge from evidence

Decide per piece of content (one post, one README), based on what happened to *that* content.

| Badge | Choose it when |
|---|---|
| **AI Generated** | You drafted most of the words, code or images. The person mainly prompted, chose between versions, reviewed or lightly edited. |
| **AI Assisted** | The person led the work: they chose what it's about and wrote or substantially rewrote it. You helped with ideas, outlines, editing, some sections, some images or code, or fact and logic checks. |
| **No AI** | No generative AI produced or rewrote any of the words, images or code. Spell check and basic grammar fixes are fine. |

**Rules:**

- **Never choose No AI for content you drafted, rewrote or edited in this session.** If you touched the substance, it's at least AI Assisted.
- Only apply No AI when the person tells you they made it without AI and you're just adding the badge.
- If you drafted it and the person then rewrote it heavily, or most of its history is outside this session, **ask one short question** rather than guess: "Did you rewrite most of this yourself, or is it mostly my draft?"
- Tricky cases:
  - AI translation of the person's own writing → AI Assisted.
  - AI made the images, the person wrote every word → AI Assisted for the piece. Suggest saying which part AI made.
  - A grammar tool rewrote sentences → AI Assisted. Pure spelling and grammar fixes → No AI.
  - AI coding help → AI Assisted if the person designed and reviewed it, AI Generated if you wrote most of it.
  - A heavily edited AI image → still AI Generated. It started with AI.

Tell the person which badge you chose and why, in one line, e.g. "AI Assisted: you wrote the post, I tightened sections 2 and 3." They can change it.

If they ask for a *less* AI badge than the evidence supports (e.g. No AI on something you drafted), say plainly that it wouldn't be accurate. It's their call after that, but don't change it silently.

## 2. Follow the project's convention

Look before you insert anything:

1. **Existing badges.** Search for `aihonestybadge.com/badges` in the project. If other posts or READMEs already use it, match their placement and format exactly.
2. **Frontmatter field.** If sibling content has a field like `ai_badge`, `aiBadge` or `ai_disclosure`, set that field (values: `no-ai`, `ai-assisted`, `ai-generated`) instead of pasting an image. The site template renders it.
3. **Otherwise, insert a snippet:**
   - Markdown files (`.md`, `.mdx`, READMEs): the Markdown snippet.
   - HTML, JSX or templates: the HTML snippet (use `className` instead of `class` in JSX, and a style object instead of the style string).
   - **Placement:** end of a blog post or article. In a README, put it with any existing badge row at the top, otherwise at the end.

## 3. Snippets

Use these exactly. Don't restyle, recolour or rehost the badge unless the person asks.

**Markdown**

```markdown
[![No AI Badge](https://www.aihonestybadge.com/badges/no-ai.svg)](https://www.aihonestybadge.com)
[![AI Assisted Badge](https://www.aihonestybadge.com/badges/ai-assisted.svg)](https://www.aihonestybadge.com)
[![AI Generated Badge](https://www.aihonestybadge.com/badges/ai-generated.svg)](https://www.aihonestybadge.com)
```

**HTML**

```html
<a href="https://www.aihonestybadge.com" target="_blank" rel="noopener"><img src="https://www.aihonestybadge.com/badges/no-ai.svg" alt="No AI Badge" style="max-width: 190px; height: auto;" /></a>
<a href="https://www.aihonestybadge.com" target="_blank" rel="noopener"><img src="https://www.aihonestybadge.com/badges/ai-assisted.svg" alt="AI Assisted Badge" style="max-width: 190px; height: auto;" /></a>
<a href="https://www.aihonestybadge.com" target="_blank" rel="noopener"><img src="https://www.aihonestybadge.com/badges/ai-generated.svg" alt="AI Generated Badge" style="max-width: 190px; height: auto;" /></a>
```

Transparent PNGs exist at the same URLs with `.png` for places that don't take SVG.

## Don't

- Don't claim the badge is verified or certified. It's a self-declaration.
- Don't add a badge to content the person didn't ask you to label, unless the project clearly badges all its content.
- Don't add a second badge where one already exists. Update it if the answer changed.

Full guidance: https://www.aihonestybadge.com (badge pages have a comparison table and more tricky cases). Machine-readable rules: https://www.aihonestybadge.com/llms.txt
