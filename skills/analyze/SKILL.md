---
name: analyze
description: Use this skill when the user wants to analyze something and needs help choosing the right approach, persona, and command sequence. Suggests whether to use the full framework or lightweight /quick mode.
allowed-tools: [Read, WebFetch, WebSearch]
---

# Analyze

I need to analyze something. Help me figure out the right approach.

## Steps

1. **Identify the domain** - What kind of subject is this?

2. **Suggest personas** - Offer 2-3 persona options with brief rationale for each. Recommend one, but let the user see alternatives.

3. **Assess complexity** - Is this a full-framework situation (complex, high-stakes, ambiguous) or would `analysis:quick` suffice?

4. **Recommend the sequence** - Which commands, in what order?

## Output

Explain briefly why this combination makes sense.

Then output the exact commands to run, with the persona included. Format them so I can copy and execute them directly.

Example output format:
```
/analysis:research [topic]. Approach as a [persona].
/analysis:evaluate [topic]. Approach as a [persona].
/analysis:critique [topic]. Approach as a [persona].
/analysis:synthesize
```

If the analysis is straightforward, suggest `analysis:quick` instead:
```
/analysis:quick [topic]. Approach as a [persona].
```

Don't run anything yet—just give me the plan and the commands.

## Available Commands

- `analysis:research` – Gather external context, industry trends, evidence base
- `analysis:evaluate` – Five perspectives: Informed, Steelman, Skeptic, Practical, Contrarian
- `analysis:critique` – Adversarial: find fatal flaws, assumptions, failure modes
- `analysis:synthesize` – Structured output: summary, recommendation, tradeoffs, open questions
- `analysis:quick` – Lightweight mode: compressed analysis in a single pass

Subject: $ARGUMENTS
