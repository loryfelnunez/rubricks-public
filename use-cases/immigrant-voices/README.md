# Immigrant Voices

Immigrant Voices is a hackathon prototype exploring how immigrant stories can be shared as practical learnings.

The prototype asks a simple question: if people have already lived through a process, made mistakes, found workarounds, and learned what they wish they had known earlier, can those stories be transformed into useful guidance for someone facing a similar situation?

Prototype repo:

https://github.com/loryfelnunez/immigrant_voices

## What This Prototype Explores

This use case explores how to technically collect, compare, and structure immigrant stories into reusable learnings.

The prototype uses public story sources, Tavily for web retrieval, and an LLM model to extract patterns, compare experiences, and identify possible learnings across stories.

> Model used: `Llama-3.3-70B-Instruct-Turbo`

## Technical Questions

This prototype is focused less on building a polished product and more on testing the underlying technical pattern:

- How do we collect relevant immigrant stories?
- How do we compare stories against one another?
- How do we identify repeated learnings across stories?
- How do we detect when there are too few stories to support a conclusion?
- How do we flag stale or outdated stories?
- How do we preserve attribution by linking back to the original stories?
- How do we evaluate the quality and trustworthiness of each story source?
- How do we decide when enough stories exist to form a reusable Rubrick?

## Rubricks Connection

This use case explores how stories can become a Rubrick.

Instead of treating each story as a one-off anecdote, Rubricks looks for reusable patterns:

- what people learned
- what mistakes they made
- what advice repeated across stories
- where stories disagree
- where the evidence is too thin
- where official sources or expert review are needed

The goal is not to turn community stories into legal advice. The goal is to structure lived experience in a way that is useful, attributed, source-aware, and honest about uncertainty.

## Current Approach

The current prototype uses:

- public immigrant stories as source material
- Tavily to retrieve relevant story sources
- an LLM to extract learnings from each story
- story-to-story comparison to identify recurring themes
- attribution links back to the original stories
- early trust and freshness checks

## Open Design Questions

Future work should improve:

- story comparison logic
- source quality scoring
- freshness detection
- consensus rules
- minimum story thresholds
- conflict detection across stories
- when to create a Rubrick from stories
- when to avoid creating a Rubrick because evidence is too weak

## Boundary

This is not legal advice.

Immigrant stories can surface practical, lived-experience insights, but high-risk guidance should be checked against official sources or expert review. Community experience is valuable, but Rubricks should make clear when a learning is well-supported, lightly supported, outdated, or source-limited.