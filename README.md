# Claude Marketing Skills

> A curated collection of production-grade [Claude Skills](https://www.anthropic.com/news/skills) for marketers, founders, and growth teams. Turn Claude into a copywriter, SEO strategist, brand strategist, email marketer, or landing page optimizer with a single skill install.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Skills](https://img.shields.io/badge/Skills-5-purple)](#the-skills)
[![Made for Claude](https://img.shields.io/badge/Made_for-Claude-orange)](https://claude.ai)

---

## What this is

This repository contains five professionally written Claude Skills focused on the core marketing disciplines that actually move revenue: copywriting, SEO, brand positioning, email marketing, and landing page optimization.

Each skill is a self-contained `SKILL.md` file built using the official Claude Skills format. Drop one into your Claude project and Claude will use the skill automatically when relevant tasks come up — no prompt engineering required, no copy-pasting templates into every chat.

If you've ever wished Claude defaulted to thinking like a senior marketer instead of a generic assistant, that's what these skills do.

## Why skills beat prompts

A good prompt lasts one conversation. A skill lives in your workspace permanently and triggers itself when relevant. That means:

- Consistent output quality across every project, every chat, every team member
- No more pasting the same 800-word system prompt into a new chat
- Skills compose — the copywriter skill knows when to defer to the brand-positioning skill
- Your team uses the same playbook automatically

## The skills

| Skill | What it does | Best for |
|-------|--------------|----------|
| [**copywriter**](./skills/copywriter) | Direct response copywriting using proven frameworks (PAS, AIDA, 4 Cs, hook-stack). Writes headlines, ad copy, CTAs, sales pages. | Founders writing sales pages, marketers writing ads, anyone selling something |
| [**seo-strategist**](./skills/seo-strategist) | Keyword research, content briefs, on-page SEO, SERP analysis, internal linking strategy. | Content marketers, SEO specialists, founders building organic channels |
| [**brand-positioning**](./skills/brand-positioning) | ICP definition, positioning statements, messaging hierarchy, category design, competitive differentiation. | Founders pre-launch, brands repositioning, agencies onboarding clients |
| [**email-marketer**](./skills/email-marketer) | Lifecycle sequences, subject lines, segmentation logic, broadcast structure, deliverability. | Ecommerce brands, SaaS marketers, newsletter operators |
| [**landing-page-optimizer**](./skills/landing-page-optimizer) | Page structure, conversion elements, hierarchy of attention, friction reduction, CRO audits. | Founders launching pages, growth marketers running paid traffic, designers |

## Installation

### Option 1: Claude.ai (Pro/Max/Team/Enterprise)

1. Open [Claude.ai](https://claude.ai) and create or open a Project
2. Click **Project settings** → **Skills**
3. Upload the `SKILL.md` file from any of the skill folders above
4. Start a new chat in that project — Claude will use the skill automatically when relevant

### Option 2: Claude Code

Clone this repo and reference the skills directory:

```bash
git clone https://github.com/YOUR_USERNAME/claude-marketing-skills.git
cd claude-marketing-skills
```

Then copy the skills you want into your Claude Code skills directory.

### Option 3: Anthropic API

Reference the skill files directly in your API calls. See [Anthropic's Skills documentation](https://docs.claude.com) for the current setup.

## How a skill works

Each skill is a markdown file with YAML frontmatter. Here's the structure:

```markdown
---
name: skill-name
description: What the skill does and when to trigger. Claude reads this to decide whether to consult the skill for a given task.
---

# Skill body

Imperative instructions, frameworks, examples, and guidance that Claude follows when the skill is active.
```

The `description` field is what triggers the skill. The body is what Claude reads once the skill is active. Skills can also include subfolders (`scripts/`, `references/`, `assets/`) for deeper context that's loaded only when needed.

## Skill design principles

Every skill in this repo follows the same writing principles:

1. **Imperative voice.** Skills tell Claude what to do, not what to consider.
2. **Frameworks over fluff.** Each skill loads Claude up with named, repeatable frameworks (PAS, AIDA, Jobs-to-be-Done, RACE, etc.) that produce consistent output.
3. **Output formats specified.** Skills define what the output should look like so you don't get a wall of text when you wanted a structured deliverable.
4. **Pushback baked in.** Skills instruct Claude to push back on weak briefs, ask for missing context, and refuse to produce vague work.

## Use cases

These skills were built with real marketing work in mind:

- **Founders writing their own copy** — copywriter + landing-page-optimizer turn a Saturday afternoon into a publishable sales page
- **Agencies onboarding new clients** — brand-positioning skill produces a positioning doc in 20 minutes that would normally take a 90-minute kickoff
- **SEO content production** — seo-strategist generates briefs your writers can execute against
- **Ecommerce lifecycle** — email-marketer plans a full welcome → abandoned cart → win-back sequence
- **Conversion rate audits** — landing-page-optimizer audits an existing page against modern CRO principles

## What's not in here (yet)

I'm intentionally keeping this collection focused. Skills I'm considering for future releases:

- `paid-ads-strategist` — Meta and Google Ads campaign structure, creative testing
- `content-strategist` — content pillars, calendars, repurposing workflows
- `social-media` — platform-specific content (LinkedIn, X, TikTok)
- `analytics-interpreter` — GA4, attribution modeling, cohort analysis
- `marketing-audit` — full-stack audit of an existing marketing operation

If you want to see one of these prioritized, open an issue.

## Contributing

PRs welcome. Before contributing a new skill:

1. Read [`CONTRIBUTING.md`](./CONTRIBUTING.md)
2. Make sure the skill has a clear, narrow scope (one job, done well)
3. Include at least one working example in the SKILL.md body
4. Test it in a real Claude project before submitting

## License

MIT — see [LICENSE](./LICENSE). Use these skills in client work, embed them in products, fork them, modify them, sell services around them. No attribution required (though it's appreciated).

## About

Built and maintained by a marketer who got tired of pasting the same system prompt into every Claude chat. If you found this useful, a star on the repo helps it reach other marketers.

---

**Keywords:** claude skills, claude ai marketing, marketing prompts, ai marketing tools, claude marketing, ai copywriting, ai seo, anthropic skills, claude prompts, marketing automation, ai brand strategy, ai email marketing, ai landing pages, conversion rate optimization, copywriting frameworks, direct response copywriting
