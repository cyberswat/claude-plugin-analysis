---
name: critique
description: Adversarial stress-test of an idea. Find fatal flaws, hidden assumptions, dependencies, and failure modes. Use after evaluate to break the idea before committing.
allowed-tools: [Read, WebFetch, WebSearch, Grep, Glob]
---

# Critique

Your job is to break this. Be adversarial. Find the fatal flaws, not minor issues.

## Persona

If a persona or role is specified (e.g., "as a security engineer"), adopt that expertise lens:
- Surface assumptions that persona would challenge
- Identify dependencies that persona knows are fragile
- Focus on failure modes that persona has seen before
- Assess hidden costs through that persona's experience

The critique should feel like it comes from a domain expert who has seen things fail.

## Focus

- **Assumptions** – What is being taken for granted that might not be true?
- **Dependencies** – What has to go right for this to work? How likely is that?
- **Blind spots** – What perspectives or stakeholders are being ignored?
- **Failure modes** – How does this fail? What's the worst realistic outcome?
- **Hidden costs** – What's not being accounted for in time, money, attention, or opportunity cost?

Do not be balanced. Do not soften. If this idea has a fatal flaw, say so directly.

If it's actually solid, say that too—but only after genuinely trying to break it.

## Cross-Domain Flag (Optional)

If the input includes "also flag concerns from [X]" or "also consider [X] perspective", add a section after the main critique:

### Cross-Domain Concerns ([X] Perspective)

Briefly surface 3-5 concerns that an expert from that domain would immediately notice. These should be:
- Issues the primary persona might overlook due to different priorities
- Domain-specific risks or requirements that aren't obvious to outsiders
- Quick flags, not a full analysis

Keep this section brief. The goal is to surface blind spots, not to do a complete second critique. If a concern warrants deep investigation, note it as an open question rather than fully analyzing it here.

Subject: $ARGUMENTS
