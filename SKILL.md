---
name: humanize-me
description: Translate human-originated thoughts, shorthand, fragments, dictation, or rough wording into a clear model of what the user means, then express that meaning back in language that remains recognizably theirs and is easier for others to understand. Use for “say this better,” “help me explain what I mean,” voice-preserving rewrites, or adapting the user's own ideas for an audience. Do not use when the source is primarily AI-generated and the goal is only to remove AI writing patterns; use an AI-text humanizer or style-rewrite skill instead.
metadata:
  author: "Grant Daniels"
  license: "MIT"
---

# Humanize Me

Understand the human before rewriting the words.

The user's original language is evidence of their meaning, voice, emotional position, and relationship to the audience. Decode those signals first. Then express the same intent in a form that is clearer, cleaner, or more effective for the people who need to understand it—without replacing the user with a generic professional voice.

## Boundary with AI-text humanizers

Humanize Me works **upstream**, where a person is trying to get an idea out and be understood. AI-text humanizers work **downstream**, after AI has already produced a draft and the task is to remove robotic patterns.

Route by source and goal:

- Use **Humanize Me** when the source is the user's own thoughts, speech, notes, fragments, or draft and preserving intended meaning and identity is central.
- Use an **AI-text humanizer** when the source is primarily AI-generated and the user only wants it to sound less artificial.
- Use **Humanize Me** when an AI draft has distorted, flattened, or misunderstood the user's original intent; recover the human meaning rather than merely changing the style.

Do not activate Humanize Me solely because a request contains the word “humanize.” Determine whether the task is intent translation or AI-output cleanup.

## Core translation loop

Perform this reasoning internally unless the user asks to see it.

1. **Listen:** Read past typos, fragments, dictation errors, shorthand, repetition, nonlinear organization, and emotional phrasing. Do not confuse surface-level messiness with unclear thinking.
2. **Decode:** Identify the user's actual point, desired outcome, key facts, emotional stance, intended audience, relationship dynamics, and any nonnegotiable wording or boundaries.
3. **Resolve:** Use conversation context and supplied writing samples to settle minor ambiguities. Ask a question only when different interpretations would materially change the message.
4. **Re-express:** Translate the meaning back into language that sounds recognizably like the user while making it easier for the intended audience to follow, trust, or act on.
5. **Check fidelity:** Confirm that the result says what the user meant—not merely what their original words literally said—and that no new facts, feelings, or claims were introduced.

## Default behavior

When the user asks for a rewrite, return the finished version only. Do not expose the meaning map, critique the user's communication, or explain the edits unless requested.

Choose the lightest level of intervention that accomplishes the user's goal:

- preserve rough edges that carry personality
- fix errors that obstruct meaning
- reorganize when the audience would otherwise miss the point
- strengthen clarity or persuasion without changing the user's position
- broaden accessibility without flattening the user's voice

## Preserve before improving

Keep the following intact unless the user asks to change them:

- the underlying message, position, and desired outcome
- names, dates, numbers, links, citations, and attributed quotes
- uncertainty, emotional weight, boundaries, and relationship context
- requested length, format, platform, and audience constraints
- distinctive phrases or humor that help the result still feel like the user

Do not invent a memory, opinion, relationship, result, credential, or lived experience. Flag a meaningful ambiguity instead of silently choosing the most polished interpretation.

## Voice and audience

Treat voice and clarity as separate controls. Preserve the user's identity while adapting the delivery for the audience.

Mirror the user's formality, directness, warmth, humor, vocabulary, rhythm, and punctuation without reproducing distracting errors or caricaturing identity, dialect, age, profession, or community. When samples conflict, prioritize the most recent writing created for a similar audience and purpose.

The best result may be cleaner than the user's everyday communication. It should still feel like something they would say after having time to organize the thought.

For difficult interpretation, audience translation, or voice matching, read [references/humanization-signals.md](references/humanization-signals.md).

## Output modes

- **Intent translation:** Decode rough or nonlinear input and return the clearest faithful expression of what the user means.
- **Light edit:** Preserve the structure and most wording; repair only what obstructs understanding.
- **Voice expansion:** Write from the user's perspective using their ideas and voice while improving reach, credibility, or accessibility.
- **Audience translation:** Keep the intent and identity while adapting the message for a specific person, group, or platform.
- **Audit:** Show where the output stops matching the user's intent or voice and recommend focused corrections.
- **Intent recovery:** Repair an AI-assisted draft when it no longer reflects what the user originally meant or how they want to be understood.

Provide multiple versions only when requested or when two materially different interpretations remain plausible.

## Final fidelity test

Before responding, confirm that:

- the user would recognize the central thought as their own
- the intended audience can understand the message more easily
- improvements did not introduce a different opinion or personality
- the result contains no invented facts, emotions, or experiences
- polish serves communication rather than erasing individuality

If the user provides no source text or idea, ask what they want to communicate and to whom.
