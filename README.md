# Humanize Me

**Humanize Me** is an open-source agentic skill that rewrites stiff, generic, or obviously AI-shaped text into writing that sounds natural, specific, and true to the user's voice.

Created by **Grant Daniels** for people who want AI to strengthen their voice—not replace it.

## What it does

- Preserves meaning, facts, links, citations, and calls to action
- Matches the user's tone from context or supplied writing samples
- Reduces robotic structure, filler, repetition, and generic business language
- Supports full rewrites, light edits, voice matching, and writing audits
- Avoids fabricated experiences, forced slang, and intentional mistakes

## Use it

Copy this repository's skill files into a `humanize-me` skill folder in your agent's skills directory, or import the repository using your agent platform's supported skill workflow.

Example prompts:

```text
Use $humanize-me to rewrite this so it sounds like me.
```

```text
Use $humanize-me for a light edit. Keep my structure, but remove anything that sounds robotic.
```

```text
Use $humanize-me to audit this draft and show me the three strongest AI tells.
```

The skill can also activate automatically when someone asks to “humanize this,” “make this less robotic,” or “make this sound like a real person.”

## Structure

```text
SKILL.md
agents/openai.yaml
references/humanization-signals.md
```

## Philosophy

Human writing is not defined by typos, slang, or random quirks. It feels human when the language reflects a real point of view, uses concrete details, and moves with a believable rhythm. This skill improves expression without inventing a personality or hiding where ideas came from.

## License

MIT License. Free to use, adapt, and share.
