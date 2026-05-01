# Contributing to Claude Marketing Skills

Thanks for considering a contribution. This collection stays useful by being focused, so contributions are held to a real bar.

## What I'm looking for

- **New skills** in marketing disciplines not yet covered (paid ads, content strategy, social, analytics, marketing ops)
- **Improvements to existing skills** based on real-world use — especially places where the current skill produces weak output or misses important frameworks
- **Bug fixes** in skill descriptions, frontmatter, or examples
- **Translations** of existing skills into other languages

## What I'm not looking for

- Generic "AI marketing assistant" skills that overlap with the existing collection
- Skills that just wrap a public framework (Jobs-to-be-Done, RACE, etc.) without adding execution guidance
- Skills with descriptions that try to trigger on every conceivable phrase ("undertriggering" is real, but kitchen-sink descriptions don't help either)

## Before opening a PR

1. **Test the skill in a real Claude project for at least a week.** If you haven't actually used it on real work, the skill probably needs more iteration.
2. **Make sure the description is specific.** It should describe the situations the skill triggers in, not just the topic.
3. **Include at least one before/after example** in the SKILL.md body so users can see what the skill produces.
4. **Keep the SKILL.md under 500 lines** unless you have a strong reason. If it's longer, consider moving deep reference material into a `references/` subfolder.
5. **Use imperative voice.** Skills tell Claude what to do.

## Skill format

Every skill follows this structure:

```
skills/your-skill-name/
├── SKILL.md (required)
├── references/ (optional, for deep reference docs)
├── scripts/ (optional, for executable helpers)
└── assets/ (optional, for templates or examples)
```

The `SKILL.md` file uses YAML frontmatter:

```markdown
---
name: your-skill-name
description: What the skill does and when to trigger it. Specific phrases the user might say. Include both what it does AND when to use it.
---

# Your Skill Name

[Imperative-voice instructions, frameworks, examples, and guidance]
```

## PR checklist

- [ ] Skill name is lowercase-with-hyphens
- [ ] Frontmatter has both `name` and `description` fields
- [ ] Description includes specific trigger phrases
- [ ] SKILL.md uses imperative voice
- [ ] At least one before/after or input/output example included
- [ ] Tested in a real Claude project before submission
- [ ] Skill has clear, narrow scope (one job, done well)

## Code of conduct

Be useful, be specific, be honest. Disagreement is fine; condescension isn't. PR feedback should focus on the work, not the person.

---

Open an issue first if you're considering a major contribution so we can talk through scope before you put time in.
