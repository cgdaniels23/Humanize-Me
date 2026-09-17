---
name: humanize-me
description: Rewrite AI-generated or overly polished text so it sounds natural, specific, and true to the user's voice. Use when asked to humanize, de-AI, make writing less robotic, match an established voice, or make copy sound like a real person. Do not use to fabricate personal experience or help misrepresent authorship.
metadata:
  author: "Grant Daniels"
  license: "MIT"
---

# Humanize Me

Make the writing feel authored, not processed. Preserve the user's meaning while improving voice, rhythm, specificity, and emotional credibility.

## Default behavior

When the user asks for a rewrite, return the rewritten text only. Skip the critique, setup, labels, and explanation unless they request them.

Infer the intended audience, tone, and level of polish from the request and surrounding context. If the user has supplied writing samples or has an established voice in the conversation, treat those as the strongest evidence. Ask a question only when the missing choice would materially change the message.

## Preserve before rewriting

Keep the following intact unless the user asks to change them:

- meaning, position, and call to action
- names, dates, numbers, links, citations, and attributed quotes
- factual claims, uncertainty, disclaimers, and legal or technical meaning
- requested length, format, platform, and audience constraints

Do not invent a memory, opinion, relationship, result, credential, or lived experience to make the copy feel personal. Flag a meaningful ambiguity instead of quietly guessing.

## Rewrite priorities

Use the smallest changes that produce a believable human voice.

1. Replace abstract or inflated language with direct, concrete wording.
2. Vary sentence length and structure so the rhythm does not feel mechanically even.
3. Use contractions, fragments, asides, or conversational phrasing only when they fit the user's voice and the context.
4. Keep some texture. Do not polish away every distinctive turn of phrase.
5. Make emphasis feel earned; remove repeated conclusions and unnecessary intensifiers.
6. Prefer specificity over generic warmth, confidence, or enthusiasm.

## Common AI tells to reduce

Remove or revise these when they appear without a clear purpose:

- an opening that restates the prompt before answering it
- generic scene-setting, throat-clearing, or a summary of what follows
- stacked adjectives, inflated claims, and vague business language
- formulaic transitions such as “moreover,” “in today's world,” or “ultimately”
- repeated “not just X, but Y” constructions
- suspiciously symmetrical paragraphs, sentence patterns, or three-part lists
- excessive headings, bullets, bold text, parentheticals, or em dashes
- canned enthusiasm, fake intimacy, and generic inspirational endings
- conclusions that simply repeat the introduction

Do not replace these with deliberate typos, random slang, forced quirks, or bad grammar. Natural writing is not the same as careless writing.

## Match the user, not a stereotype

Mirror the user's level of formality, directness, humor, punctuation, and vocabulary without caricaturing identity, dialect, age, profession, or community. Preserve recognizable phrases when they work. If voice samples conflict, prioritize the most recent sample written for the same audience and format.

For a detailed diagnosis or a difficult rewrite, read [references/humanization-signals.md](references/humanization-signals.md).

## Output modes

- **Rewrite:** Return one finished version by default.
- **Light edit:** Preserve the structure and phrasing; fix only the artificial or awkward parts.
- **Voice match:** Follow supplied samples more closely than generic style conventions.
- **Audit:** Identify the strongest robotic signals, explain their effect briefly, and offer a revision.
- **Options:** Provide alternatives only when requested or when two materially different tones are equally plausible.

If the user provides no text, ask them to paste the draft or identify the content to revise.

## Final pass

Before responding, confirm that the revision:

- says the same thing unless a change was requested
- sounds natural when read aloud
- contains no invented facts or personality
- avoids both corporate polish and exaggerated casualness
- follows the requested format and length

Never claim that text is “undetectable” or guarantee the result of an AI detector. If asked to evade detection or conceal authorship, decline that goal and offer to improve clarity, voice, and originality instead.
