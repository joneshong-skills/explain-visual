---
name: explain-visual
description: "explain, visual, visually, diagrams, explanation, flowcharts, architecture, 視覺化解釋, 用圖表說明, 畫圖解釋"
version: 0.1.0
disable-model-invocation: true
---

# Explain Visual

Transform technical explanations into visual-first responses using ASCII diagrams,
flowcharts, tables, and structured layouts — directly in conversation without generating files.

> Complements `diagram-gen` (file output). Use this for inline explanations;
> use `diagram-gen` when a standalone diagram file is needed.

## Core Principle

Minimize prose. Maximize structure. The goal is rapid comprehension, not exhaustive detail.

## Response Structure

Follow this layered pattern — readers can stop at any level:

```
Layer 1: One-sentence summary + overview diagram
Layer 2: Component breakdown with relationship arrows
Layer 3: Concrete examples / before-after comparisons
Layer 4: Trade-off table + recommendations
```

Always start with Layer 1. Go deeper only as needed by the topic's complexity.

## Visual Elements Toolkit

### ASCII Box Diagrams (Architecture, Components)

```
┌─────────────┐     ┌─────────────┐
│   Client     │────→│   Server    │
└──────┬──────┘     └──────┬──────┘
       │                    │
       ▼                    ▼
┌─────────────┐     ┌─────────────┐
│   Cache      │←───│   Database  │
└─────────────┘     └─────────────┘
```

### Flow Arrows (Processes, Sequences)

```
Request → Auth Check → Route Match → Handler → Response
                │                        │
                ▼                        ▼
            403 Error              DB Query → Transform → JSON
```

### Tree Structure (Hierarchies, File Trees)

```
System
├── Module A
│   ├── Sub-component 1
│   └── Sub-component 2
└── Module B
    └── Sub-component 3
```

### Comparison Tables (Trade-offs, Options)

| Approach | Speed | Complexity | Scalability |
|----------|-------|------------|-------------|
| Option A | Fast  | Low        | Limited     |
| Option B | Medium| Medium     | Good        |
| Option C | Slow  | High       | Excellent   |

### Timeline / Phase Diagrams

```
Phase 1          Phase 2          Phase 3
─────────── → ─────────── → ───────────
 Setup            Build           Deploy
 [2 days]        [5 days]        [1 day]
```

### Emphasis Markers

- `【Important】` for critical points
- `>>>` for key takeaways
- `═══` horizontal rules for major section breaks

## Rules

1. **No code** unless explicitly requested — focus on concepts and relationships
2. **Diagram first** — lead every major section with a visual, then explain below it
3. **Tables over lists** — when comparing 2+ items, always use a table
4. **Arrows over words** — "A sends data to B" → `A ──data──→ B`
5. **Progressive depth** — overview → details → examples → trade-offs
6. **Annotate diagrams** — add brief labels directly on arrows and boxes
7. **White space matters** — generous spacing improves readability

## When NOT to Use This Style

- Simple factual answers ("What version is X?" → just answer)
- Code-only requests ("Show me the implementation" → use code blocks)
- Very short explanations (1-2 sentences suffice → skip the diagrams)

Escalate to `diagram-gen` when the user needs a reusable, shareable diagram file (SVG/PNG).
