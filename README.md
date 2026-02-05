# Analysis Plugin for Claude Code

A structured thinking framework for analysis and decision-making.

## Commands

| Command | Purpose |
|---------|---------|
| `analysis:analyze` | Plan your analysis: suggests persona, assesses complexity, recommends command sequence |
| `analysis:research` | Gather external context, industry trends, evidence base |
| `analysis:evaluate` | Five perspectives: Informed, Steelman, Skeptic, Practical, Contrarian |
| `analysis:critique` | Adversarial: find fatal flaws, assumptions, failure modes |
| `analysis:synthesize` | Structured output: summary, recommendation, tradeoffs, open questions |
| `analysis:quick` | Lightweight mode: compressed analysis in a single pass (under 300 words) |

## Usage

### Full Framework (complex, high-stakes decisions)

```
/analysis:analyze [your topic]
```

This will suggest a persona and output the commands to run:

```
/analysis:research [topic]. Approach as a [persona].
/analysis:evaluate [topic]. Approach as a [persona].
/analysis:critique [topic]. Approach as a [persona].
/analysis:synthesize
```

### Quick Mode (straightforward decisions)

```
/analysis:quick [your topic]. Approach as a [persona].
```

## Personas

Each command supports a persona that layers domain expertise onto the analysis:

- "Approach as a financial analyst"
- "Approach as a systems architect"
- "Approach as a product manager"
- "Approach as a cognitive systems designer"

The persona affects what evidence matters, what concerns arise, and how recommendations are framed.

## Installation

```bash
claude plugins add github:cyberswat/claude-plugin-analysis
```

## License

MIT
