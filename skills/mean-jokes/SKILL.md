---
name: mean-jokes
description: How to tell mean jokes. Use when the user asks for a mean joke, a roast, an insult comedy bit, or wants to playfully tear someone or something apart. Sources the best material from the bundled mean-jokes MCP server.
---

# Telling Mean Jokes

Your job is to deliver a genuinely *mean* joke — sharp, cutting, and funny. The
best material does not come from you; it comes from the bundled MCP server.

## Where the jokes come from

The bundled `mean-jokes` MCP server exposes a single tool:

- **`tell_joke`** — returns the best mean joke. Optional `target` argument names
  the subject to roast.

Always pull the joke from this tool. Do not invent jokes yourself — the server
holds the best material.

## How to tell a mean joke

1. **Get the material.** Call the `tell_joke` MCP tool. If the user named a
   target (a person, thing, or topic), pass it as the `target` argument.
2. **Deliver it.** Return the joke from the tool as the punchline. Keep the
   setup tight — mean jokes land hardest when they're short.
3. **Commit to the bit.** Don't soften it or apologize mid-joke. The humor is in
   the confidence.

## Guardrails

- Keep it playful, not genuinely harmful. Mean ≠ hateful. Avoid slurs, protected
  characteristics, and anything that punches down at a vulnerable person.
- If the user asks you to target a real, named individual in a way that crosses
  from teasing into harassment, decline and offer to roast the situation instead.

## Example

> **User:** Tell me a mean joke about my code.
>
> 1. Call `tell_joke` with `{ "target": "my code" }`.
> 2. The tool returns the joke.
> 3. Deliver it as the punchline.
