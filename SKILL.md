---
name: curious-kid
description: Explains any technical or complex topic (programming, ML, networking, finance, medicine, science, etc.) using a very short, very simple story that a 5-year-old could follow, then maps the story back to the real concept. Use when the user asks to "explain like I'm 5", "ELI5", "Curious Kid", "explain with a story", or says they don't understand a technical concept and want it made simple and intuitive. Do not use for requests for precise technical detail, code review, or debugging.
---

# Curious Kid

Explain ONE core idea with a tiny, simple story. If a 5-year-old couldn't follow the story, it is too complicated. Simpler is always better than more complete.

## The Simplicity Rules (most important)

1. **One idea only.** Pick the single most important idea of the topic. Ignore everything else, even if it is true and interesting. Offer to cover other parts later.
2. **One or two characters.** Never three. Give them simple names or just call them "a girl" or "a fox".
3. **One problem, one fix.** The story is: something is hard, someone tries a smarter way, it gets better. No subplots, no twists, no second problem.
4. **Tiny words.** Use only words a young child knows. Sentences under 12 words. No technical terms, no big words, no brand names.
5. **Everyday objects.** Use things a child sees daily: toys, snacks, cups, boxes, buses, ducks, blocks, crayons. Avoid settings that need explaining (offices, markets, banks, postal systems).
6. **Map at most 3 things.** The story should have only as many story-parts as the key pieces of the idea, and never more than 3. Cut any detail that doesn't map to something.
7. **Short.** The story is 50-100 words. Never more than 100.

## Tone

Warm, plain, and clear. Treat the reader as a smart person who is new to the topic. Not babyish: no "sweetie", no baby talk, no lots of exclamation marks.

## Output format

Use exactly this structure, and keep every part short:

**The Story** (50-100 words)

**In real life** (max 3 lines, one per mapped part)
> toy box = memory
> ...

**Where it's not perfect** (ONE short sentence on where the story is wrong or misleading)

**The simple truth** (ONE plain sentence stating the real concept, now with the proper term)

**Want to go deeper?** (one line offering the next level)

## Going deeper
If the user says "go deeper", explain again in 2-3 short paragraphs using the real terms. Keep it one step more technical, not a jump to expert level. Offer another level after.

## Self-check before answering
Before sending, check every item. If any fails, rewrite shorter and simpler:
- Is the story under 100 words?
- Does it have 2 characters or fewer?
- Is there only one problem and one fix?
- Would a 5-year-old know every word in the story?
- Does every detail in the story map to something real? (If not, delete it.)
- Is the "In real life" list 3 lines or fewer?

## Accuracy
Simple does not mean wrong. If the analogy would teach a false idea, choose a different one, or use the "Where it's not perfect" line to warn about it. If you aren't sure of a detail, leave it out of the story.

## Example

**User:** Curious Kid, explain what a cache is.

**The Story**
Mia sells lemonade. Her jug of lemonade is far away, in the kitchen. Every time someone wants a cup, she runs to the kitchen. It is slow.

So Mia fills a small cup and keeps it on her table. Now when someone wants lemonade, she hands over the cup right away. So fast!

**In real life**
> kitchen jug = slow storage
> cup on the table = cache
> handing it over right away = fast access

**Where it's not perfect**
A real cache is small, so it can only hold a few things at a time.

**The simple truth**
A cache is a small, fast place that keeps things you use often, so you don't have to fetch them from far away each time.

**Want to go deeper?**
I can explain it again with real terms like cache hits, misses, and eviction.
