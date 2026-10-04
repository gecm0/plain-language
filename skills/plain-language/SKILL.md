---
name: plain-language
description: Plain-language writing rules for English and Spanish, inspired by the ISO 24495-1 principles. Use when writing any text for people, and when asked to review or rewrite a text in plain language ("lenguaje claro").
---

# Plain language (EN/ES)

Apply these rules to all text written for people: replies, documentation, comments and commit messages.
They do not apply to code, commands, paths or direct quotes.

## Core rules

### Relevant
1. Start with the answer or conclusion. Add detail after it, only if needed.
2. Include only what the reader needs to understand or act.
3. Do not announce what you are going to say. Do not summarize what you just said.

### Findable
4. In long texts, use headings that say what each part contains.
5. Write steps as a numbered list. Put one step in each item and start it with a verb.
6. Write options as a bulleted list. Give every item the same structure.
7. Use a table to compare data.

### Understandable
8. Write one idea per sentence: about 20 words at most in English and about 25 in Spanish.
9. Use the active voice and say who does what.
10. Use verbs, not nouns made from verbs: "configure", not "perform the configuration".
11. Choose the common word over the technical one. If you need a technical term, define it the first time.
12. Use one term for each concept. Do not switch between synonyms.
13. Write in the positive. Avoid double negatives.
14. Do not hedge when you know the answer. If you do not know, say so once and say what is missing.
15. Spell out acronyms the first time, unless the reader already knows them.

### Usable
16. Give exact numbers, paths, commands and versions, formatted as code.
17. If the reader must act, say what to do, where to do it and what result to expect.
18. Put warnings before the step they apply to.
19. Add a concrete example when a rule alone is not enough.

## Spanish annex
20. Use the gerund only for simultaneous or immediately preceding actions. Do not use it for a later action: «Se instaló, reiniciándose el equipo» ✗.
21. Use one subordinate clause per sentence at most. Break up chains of «que».
22. If it matters who did something, do not hide the actor behind «se»: «el script borró el archivo», not «se borró el archivo».
23. Avoid anglicisms that have a common Spanish equivalent. Keep established technical terms such as «commit» or «branch».

## English annex
24. Prefer a one-word verb when a phrasal verb is ambiguous: "configure" rather than "set up".
25. Do not put more than three nouns in a row. Break up noun stacks with prepositions.
26. Keep articles and "that". Do not write in telegraph style.

## Review mode
When asked to review or rewrite a text:
- Keep its meaning and data.
- Apply these rules.
- Return the rewritten text.
- If asked, add a short list of changes.
