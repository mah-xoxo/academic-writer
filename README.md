# acad-writer

A skill for Claude.ai that turns the assistant into a doctoral-level academic writing and research collaborator — critical, rigorous, and incapable of producing text that reads like it was written by a language model.

Built for researchers in the social sciences, but adaptable to any academic field.

---

## What it does

At the start of every session, the skill asks two things:

1. **Your research area and how you want to work** — writing partner, critical reviewer, methodologist, or a mix
2. **Your preferred citation style** — defaults to APA, but switches on request (ABNT, Chicago, Vancouver, MLA)

From there, it operates across four modes:

| Mode | When it activates |
|---|---|
| **Writing** | Drafting or co-writing sections of a paper |
| **Review** | You ask for feedback — it responds as a journal reviewer, not a cheerleader |
| **Data Analysis** | You share a dataset or statistical output |
| **Literature Review** | You need synthesis, not summaries |

---

## Why this skill exists

Most AI writing assistance fails academic work in two ways:

**It sounds like AI.** Uniform sentence structures, significance inflation ("pivotal," "groundbreaking"), fake analytical depth through -ing constructions, em dashes everywhere, generic conclusions. Any detector — and any experienced reader — catches it immediately.

**It agrees with everything.** A collaborator that never pushes back isn't a collaborator. It's a mirror that flatters. Good research needs friction.

This skill fixes both. It produces writing that builds arguments progressively, integrates citations as part of the logic rather than decoration, and varies rhythm the way a human writer does. And in reviewer mode, it behaves like a committee member who has read your work carefully and has notes.

---

## How to install

1. Download `acad-writer.skill`
2. In Claude.ai, go to **Settings → Skills**
3. Click **Install Skill** and upload the file
4. Start a new conversation — the skill will activate automatically

---

## How to adapt for your field

The skill is designed to be configured at runtime, not hardcoded. When you start a session, just tell the agent your area and role:

> *"I'm a PhD student in organizational sociology. I need a writing collaborator for my dissertation chapter on institutional logics."*

or

> *"I work in public health. Review this methods section as if you were a JAMA reviewer."*

or

> *"My area is educational psychology. Help me design a 2×2 experiment and write the methodology section."*

The skill adjusts accordingly. No editing required.

If you want to hardcode your own field permanently — for example, you're building a fork specifically for clinical psychology researchers — open `SKILL.md` and edit the **Initialization Protocol** section. Replace the open questions with fixed defaults for your context.

---

## What it will never do

- Produce prose with em dashes used as connectors mid-sentence
- Use vague attribution ("researchers suggest," "experts agree") without naming the source
- Write bullet points inside academic body text
- Open every paragraph with "Furthermore," "Moreover," or "Additionally"
- Approve work that doesn't meet the standard to avoid friction
- Conclude with "future research should explore this further" unless something specific follows

---

## Structure

```
acad-writer/
├── SKILL.md      — the skill itself
└── README.md     — this file
```

---

## Contributing

If you adapt this skill for a specific field and it works well, pull requests are welcome. Useful additions might include field-specific style guides, journal-specific reviewer personas, or language-specific variants (the skill currently supports PT and EN).

---

## Credits

Developed by Ana based on her experience as a postgraduate researcher in consumer behavior and data analysis. Style calibration draws on published work in the *Journal of Consumer Behaviour* and *Journal of Consumer Psychology*.
