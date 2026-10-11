---
name: ai-honesty-badge
description: Adds an honest AI disclosure badge (No AI, AI Assisted or AI Generated, from aihonestybadge.com) to written work such as blog posts, READMEs, docs, articles and release notes, choosing the badge from what actually happened in the session. Use when the user asks to add an AI badge, AI disclosure or "AI honesty badge", asks which badge fits, says /ai-honesty-badge, or finishes a piece of content in a project that already uses aihonestybadge.com badges or an ai_badge-style frontmatter field.
metadata:
  author: "Steven Hylands"
  version: "1.3.0"
  homepage: "https://www.aihonestybadge.com"
---

# AI Honesty Badge

Label a piece of work with how much AI went into it. You're usually the AI in question, so you have first-hand evidence. Use it.

The badges only work because people are honest with them. Nobody verifies them. That makes accuracy your job.

## 1. Decide the badge from evidence

Decide per piece of content (one post, one README), based on what happened to *that* content.

**The badge says who led the work, not who typed it.** You will usually have produced most of the words or code. That alone does not make it AI Generated. The test between the two AI badges: did the person shape the work, or just accept it?

| Badge | Choose it when |
|---|---|
| **AI Assisted** | The person led. They decided what to make, directed it and shaped the result over rounds of feedback: rejecting output, changing the approach, deciding what stays. It stays AI Assisted even when you wrote the first draft or produced most of the words, code or images. Directing through prompts alone counts as shaping. |
| **AI Generated** | The person gave you a brief and published roughly what came back. They may have picked between versions, checked it and made light fixes, but didn't shape it. |
| **No AI** | No generative AI produced or rewrote any of the words, images or code. Spell check and basic grammar fixes are fine. |

**Judging it from the session:**

- The person gave direction beyond the first request (changed the approach, rejected something, made the design or editorial decisions, supplied the ideas and opinions) → **AI Assisted**.
- One request, and they took what you produced → **AI Generated**.
- Most of the work's history is outside this session, or you can't tell which it was → **ask one short question** rather than guess: "Did you direct and shape this, or is it mostly what I produced from your brief?"

**Rules:**

- **Never choose No AI for content you drafted, rewrote or edited in this session.** If you touched the substance, it's at least AI Assisted.
- Only apply No AI when the person tells you they made it without AI and you're just adding the badge.
- Don't round up to AI Generated out of caution. Calling a person's directed work "generated" is as inaccurate as calling your draft "No AI".
- Tricky cases:
  - AI translation of the person's own writing → AI Assisted.
  - AI made the images, the person wrote every word → AI Assisted for the piece. Suggest saying which part AI made.
  - A grammar tool rewrote sentences → AI Assisted. Pure spelling and grammar fixes → No AI.
  - AI coding help → AI Assisted if the person decided what to build, directed it and reviewed it, even if you wrote all the code. AI Generated if they described what they wanted and shipped what you built.
  - An AI image the person iterated on or edited → AI Assisted. An AI image taken as it first came → AI Generated.
  - You wrote the first draft and the person reworked it → AI Assisted.

Tell the person which badge you chose and why, in one line, e.g. "AI Assisted: you directed the design and decisions, I wrote the code." They can change it.

If they ask for a *less* AI badge than the evidence supports (e.g. No AI on something you drafted), say plainly that it wouldn't be accurate. It's their call after that, but don't change it silently.

## 2. Follow the project's convention

Look before you insert anything:

1. **Existing badges.** Search for `aihonestybadge.com/badges` in the project. If other posts or READMEs already use it, match their placement and format exactly.
2. **Frontmatter field.** If sibling content has a field like `ai_badge`, `aiBadge` or `ai_disclosure`, set that field (values: `no-ai`, `ai-assisted`, `ai-generated`) instead of pasting an image. The site template renders it.
3. **Otherwise, insert a snippet:**
   - Markdown files (`.md`, `.mdx`, READMEs): the Markdown snippet.
   - HTML, JSX or templates: the HTML snippet (use `className` instead of `class` in JSX, and a style object instead of the style string).
   - **Placement:** end of a blog post or article. In a README, put it with any existing badge row at the top, otherwise at the end.
4. **Size.** Use Small (`-small`, 20px tall) in READMEs and badge rows, where it matches shields.io badges. Use Large (`-large`, 28px) at the end of a post, in a footer or on a portfolio. One version works on light and dark pages.
5. **Older badges.** If the project already uses an older AI Honesty file (`no-ai.svg`, `ai-assisted-dark.svg` and so on), those still work. Match it, and mention that the current `-small`/`-large` version exists.

## 3. Snippets

Use these exactly. Don't restyle, recolour or rehost the badge unless the person asks.

**Markdown**

```markdown
[![No AI](https://www.aihonestybadge.com/badges/no-ai-small.svg)](https://www.aihonestybadge.com)
[![AI Assisted](https://www.aihonestybadge.com/badges/ai-assisted-small.svg)](https://www.aihonestybadge.com)
[![AI Generated](https://www.aihonestybadge.com/badges/ai-generated-small.svg)](https://www.aihonestybadge.com)
```

**HTML** (works in GitHub READMEs too)

```html
<a href="https://www.aihonestybadge.com" target="_blank" rel="noopener"><img src="https://www.aihonestybadge.com/badges/no-ai-small.svg" alt="No AI" height="20"></a>
<a href="https://www.aihonestybadge.com" target="_blank" rel="noopener"><img src="https://www.aihonestybadge.com/badges/ai-assisted-small.svg" alt="AI Assisted" height="20"></a>
<a href="https://www.aihonestybadge.com" target="_blank" rel="noopener"><img src="https://www.aihonestybadge.com/badges/ai-generated-small.svg" alt="AI Generated" height="20"></a>
```

For Large, swap `-small` for `-large` and `height="20"` for `height="28"`. Transparent PNGs exist at the same URLs with `.png` for places that don't take SVG.

## Don't

- Don't claim the badge is verified or certified. It's a self-declaration.
- Don't add a badge to content the person didn't ask you to label, unless the project clearly badges all its content.
- Don't add a second badge where one already exists. Update it if the answer changed.

Full guidance: https://www.aihonestybadge.com (badge pages have a comparison table and more tricky cases). Machine-readable rules: https://www.aihonestybadge.com/llms.txt
