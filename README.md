<p align="center">
  <img src="assets/logo.png" alt="Curious Kid logo" width="220">
</p>

<h1 align="center">Curious Kid</h1>

<h3>
  A Claude skill that explains any technical topic using a simple short story, so even a 5-year-old can understand.
</h3>

Curious Kid works with Claude. Ask about programming, ML, networking, finance, medicine, or science, and it answers with a tiny story first, then connects it back to the real concept. You get the shape of the idea in under a minute, so the jargon has something to attach to later.

## Example

**You:** /curious-kid explain what a cache is.

**Claude:**

> **The Story**
> Mia sells lemonade. Her jug of lemonade is far away, in the kitchen. Every time someone wants a cup, she runs to the kitchen. It is slow.
>
> So Mia fills a small cup and keeps it on her table. Now when someone wants lemonade, she hands over the cup right away. So fast!
>
> **In real life**
> kitchen jug = slow storage
> cup on the table = cache
> handing it over right away = fast access
>
> **Where it's not perfect**
> A real cache is small, so it can only hold a few things at a time.
>
> **The simple truth**
> A cache is a small, fast place that keeps things you use often, so you don't have to fetch them from far away each time.
>
> **Want to go deeper?**
> I can explain it again with real terms like cache hits, misses, and eviction.

## Why it works

- **Story first.** Intuition comes before definitions.
- **One idea at a time.** Each story covers only the core concept, not the whole topic.
- **Honest about its limits.** Every answer includes a "where it's not perfect" line, so the analogy doesn't leave you with wrong ideas.
- **A path forward.** Ask to go deeper and it re-explains with real terminology, one step at a time.

## Installation

### Claude.ai
1. Zip the `curious-kid` folder.
2. Go to **Settings > Capabilities > Skills** and upload the zip.
3. Make sure the skill is toggled on.

### Claude Code
Copy the folder into your skills directory:

```bash
# Personal (all projects)
cp -r curious-kid ~/.claude/skills/

# Or project-specific
cp -r curious-kid .claude/skills/
```

Menu names and paths can change between versions, so check the current Claude documentation if a step doesn't match.

## Usage

Just ask. Any of these will trigger it:

- `Curious Kid, explain how DNS works`
- `ELI5: what is gradient descent?`
- `Explain compound interest with a story`
- `I don't get Docker. Make it simple.`

Then follow up with:

- `go deeper` for the same topic with real terminology
- `another example` for a different story on the same idea

## How it works

The skill's behavior is defined in [`SKILL.md`](./SKILL.md). The key rules:

| Rule | Limit |
|---|---|
| Ideas per story | 1 |
| Characters | 2 or fewer |
| Story length | 50-100 words |
| Sentence length | Under 12 words |
| Story parts mapped to real concepts | 3 or fewer |
| Plot | One problem, one fix |

Before answering, the skill runs a self-check and rewrites the story if it breaks any of these limits.

## Customization

Edit `SKILL.md` to fit your taste:

- **Simpler or richer stories:** change the word limit in the Simplicity Rules.
- **Different tone:** edit the Tone section (more playful, more formal, and so on).
- **Domain-specific settings:** add guidance such as "for finance topics, use stories about sharing snacks or trading toys."
- **Different output sections:** change the Output format block.

## Known limitations

- Analogies simplify. Always treat the story as a starting point, not the full picture.
- Very broad topics (for example, "how the internet works") get one core idea per story, so expect to ask follow-ups.
- Not meant for precise technical specs, code review, or debugging.

## Repository structure

```
curious-kid/
├── SKILL.md    # The skill itself
├── README.md   # This file
├── LICENSE     # MIT license
└── assets/
    └── logo.png
```

## License

MIT. See `LICENSE` for details.
